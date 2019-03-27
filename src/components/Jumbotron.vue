<template>
  <v-jumbotron height="450px" :gradient="gradient" dark>
    <v-container fill-height>
      <v-layout align-center>
        <v-flex>
          <h3 class="display-3">About me!</h3>
   <v-avatar size="120" margin="">
      <img
        src="/imagini/11_027.webp"
        alt="MasterCalin"
      >
    </v-avatar>
          <span class="subheading"><h2>My name is Cozma Viorel Călin, I’m a highly motivated developer from Romania. I have a passion for web development and I love to create websites from scratch.</h2></span>

          <v-divider class="my-3"></v-divider>

          <div class="title mb-3"><p>Down below you can see more information about how I work.</p></div>

          <v-btn type='button' to="/contact"
            class="mx-0"  
            color="cyan"
            large
          >
            Contact
          </v-btn>
        </v-flex>
      </v-layout>
    </v-container>
  </v-jumbotron>
</template>

<style scoped>

@media screen and (max-width:760px) {
    h3, h2, p{
        font-size: 17px;
    }
  }

.v-avatar{
  padding: 0;
  margin-bottom: 10px;
}

</style>

<script>
  export default {
    data: () => ({
      gradient: 'to top, #00796B, #3F51B5'
    })
  }
</script>