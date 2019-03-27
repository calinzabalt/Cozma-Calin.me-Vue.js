<template>
  <v-container>
      <div id="top"><h1>Here are some of my latest projects</h1></div>
      <LazyHydrate when-visible>
      <Carousel />
      </LazyHydrate>
       <LazyHydrate ssr-only>
      <Table slot-scope="{ hydrated }"
             v-if="hydrated"/>
       </LazyHydrate>
       <h2>Besides web development I have more skills. <br> One of these are 3D designing and another one is animation maker</h2>
        <LazyHydrate when-visible>
       <Galery />
        </LazyHydrate>
  </v-container>
  
</template>

<script>
import LazyHydrate from 'vue-lazy-hydration';

export default {
  name: 'work',
  metaInfo: {
    title: 'Work',
  meta: [
    {name: 'description', content:'Welcome!- Here you will find my latest projects that I built along the time'}
  ] 
  },
  components: {
   LazyHydrate,
    Carousel: () => import('../components/Carousel.vue'),
    Table: () => import('../components/Table.vue'),
    Galery: () => import('../components/Galery.vue'),
  }
}
</script>

<style scoped>
h1{
  padding-top: 70px;
  padding-bottom: 20px;
  color: white;
  
}

h2{
  padding-top: 25px;
  padding-bottom: 10px;
  color: white;
}


</style>


