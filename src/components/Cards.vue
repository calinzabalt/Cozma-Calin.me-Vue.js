<template>
  <v-container grid-list-xl text-xs-center>
    <v-layout row wrap>
      <v-flex xs12 md4 sm4>
        <v-card>
        <v-img
          src="/imagini/responsive-2044932_1280.webp"
          aspect-ratio="1.2"
        ></v-img>

        <v-card-title primary-title>
          <div>
            <h3 class="headline mb-0">Responsive Design</h3>
            <h4 class="subheading" >My goals are to focus on aspect, content, speed and a fully responsive website that run on every device.</h4>
          </div>
        </v-card-title>

        <v-card-actions>
          <v-btn dark type='button' class="mx-1" color="#039BE5" href="/work">Portofolio</v-btn>
        </v-card-actions>
      </v-card>
        </v-flex>

      <v-flex xs12 md4 sm4>
        <v-card>
        <v-img
          src="/imagini/business-2987962_640.webp"
          aspect-ratio="1.2"
        ></v-img>

        <v-card-title primary-title>
          <div>
            <h3 class="headline mb-0">Solutions</h3> 
            <h4 class="subheading" >I will try to resolve your problems and provide new solutions for a better and competitive website.</h4>
          </div>
        </v-card-title>

        <v-card-actions>
          <v-btn dark type='button' class="mx-1" color="#039BE5" href="/work">Portofolio</v-btn>
        </v-card-actions>
      </v-card>
      </v-flex>

      <v-flex xs12 md4 sm4>
        <v-card>
        <v-img
          src="/imagini/pexels-photo.webp"
          aspect-ratio="1.2"
        ></v-img>

        <v-card-title primary-title>
          <div>
            <h3 class="headline mb-0">How I do the work</h3>
            <h4 class="subheading" >For a front-end website I use programming languages like: Javascript (React.js, Vue.js and Polymer).</h4>
          </div>
        </v-card-title>

        <v-card-actions>
         <v-btn dark type='button' class="mx-1" color="#039BE5" href="/work">Portofolio</v-btn>
        </v-card-actions>
      </v-card>
        
      </v-flex>
    </v-layout>
  </v-container>
</template>

<style scoped>

.layout{
  padding-top: 20px;
  padding-bottom: 40px;
}

@media screen and (min-width: 1200px) {
    .container {
      width: 70%;
  }
}

.v-card{
   border-radius: 3px;
   box-shadow: 1px 1px 5px 1px rgba(0, 0, 0, 0.5);
}


</style>
