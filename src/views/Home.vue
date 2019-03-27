<template>
  <div class="home">
    <LazyHydrate ssr-only>
    <Parallax slot-scope="{ hydrated }"
              v-if="hydrated"/>
    </LazyHydrate>

    <LazyHydrate when-visible>
    <Jumbotron />
    </LazyHydrate>

    <LazyHydrate ssr-only>
    <Cards slot-scope="{ hydrated }"
           v-if="hydrated"/>
    </LazyHydrate>
  </div>
</template>

<script>
// @ is an alias to /src
import LazyHydrate from 'vue-lazy-hydration';

export default {
  name: 'home',
  metaInfo: {
    title: 'Home',
    
  meta: [
    {name: 'description', content:'Welcome!- Here you will find the information about me and how I do the work'}
  ]  
  },
  components: {
    LazyHydrate,
    Parallax: () => import('../components/Parallax.vue'),
    Jumbotron: () => import('../components/Jumbotron.vue'),
    Cards: () => import('../components/Cards.vue'),
  }
}
</script>
