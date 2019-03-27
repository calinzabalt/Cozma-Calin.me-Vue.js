<template>

  <v-footer dark height="100%" color="teal">
    <v-layout justify-center row wrap>
    <v-flex xs12 sm4>
      <div class="social">
        <h2>Social media links:</h2>
        <v-btn aria-label="linkedn" type='button' href="https://www.linkedin.com/in/cozma-viorel-calin-947658145/" target="blank" large icon class="light-blue darken-3">
            <v-icon medium>fa-linkedin</v-icon>
        </v-btn>
        <v-btn aria-label="facebook" type='button' href="https://web.facebook.com/calinviorel.cozma" target="blank" large icon class="light-blue darken-4">
             <v-icon medium>fa-facebook</v-icon>
        </v-btn>
        <v-btn aria-label="youtube" type='button' href="https://www.youtube.com/channel/UCQ2N3yvA9bq0ZgXEK2m8pwA?view_as=subscriber" target="blank" large icon class="deep-orange darken-4">
            <v-icon medium>fa-youtube</v-icon>
        </v-btn>
         <v-btn aria-label="google plus" type='button' href="https://plus.google.com/u/0/112508366335698318230" target="blank" large icon class="deep-orange darken-4">
            <v-icon medium>fa-google-plus</v-icon>
        </v-btn>
      </div>
    </v-flex> 

    <v-flex xs12 sm4>
      <div class="available">
      <h2>I am available for work</h2>
       <v-btn type='button' to="/contact" class="mx-0" color="cyan" large>Message me  </v-btn> 
        
    </div>
    </v-flex> 

    <v-flex xs12 sm4>
      <div class="links">
        <h2>Useful links:</h2>

        <v-btn type='button' small color="indigo" dark to="/#">Home</v-btn>
        <v-btn type='button' small color="indigo" dark to="/work">Work</v-btn>
        <v-btn type='button' small color="indigo" dark to="/contact">Contact</v-btn>
        
      </div>
    </v-flex>  
    <div class="copy">
   <h3>&copy;2019 — <strong>All rights reserved</strong></h3>
    </div>
    </v-layout>
    <cookie-law theme="blood-orange--rounded"/>
  </v-footer>
  
  </template>

<script>
import CookieLaw from 'vue-cookie-law'
  export default {
    components: { CookieLaw }
  }
</script>

<style scoped>

.copy{
  margin-bottom: 10px;
}

.social{
  margin-top: 10px;
  padding: 20px;
}

.links{
  margin-top: 10px;
  padding: 20px;
}

.available{
  padding: 20px;
}
 
</style>
