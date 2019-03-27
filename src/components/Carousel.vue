<template>
<v-container>
  <v-layout row wrap>
    <v-flex xs12>
    <v-carousel>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src">
      <div class="title">
          {{ item.title}}
      </div>  
    </v-carousel-item>
  </v-carousel>
    </v-flex>
  </v-layout>  
</v-container>  
</template>

<script>
  export default {
    data () {
      return {
        items: [
          {
            src: '/imagini/Screenshot from 2018-10-25 10-33-08.webp', title: 'Find out the weather in your country'
          },
          {
            src: '/imagini/Screenshot from 2018-08-06 22-34-46.webp', title: 'This is a simple application that show how many days, hours, minutes and seconds are until your select date.'
          },
          {
            src: '/imagini/Screenshot from 2018-08-06 22-37-42.webp', title: 'This is an application where you can search for your favorite books.'
          },
          {
            src: '/imagini/Screenshot from 2018-08-28 10-43-23.webp', title: 'This is an app that is created with React Apollo.'
          },
           {
            src: '/imagini/reminder.webp', title: 'Why waste paper on a list. Build your own online with reminder'
          }
        ]
      }
    }
  }
</script>

<style scoped>

.title{
  position: absolute;
  margin-left: auto;
  margin-right: auto;
  left: 0;
  right: 0;
  bottom: 50px;
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
  font-size: 2em;
  padding: 30px;
}

</style>