<template>
  <div>
     <v-parallax
    height="500"
    src="/imagini/bulletin-board-3127287_1920.webp">
      </v-parallax>
      <div class="grid">
      <h1 class="subtitle">I’m currently available for freelance work.<br>
If you have a project that you want to get started, or if you want<br> my help to accomplish something you can contact me on this platform:</h1>
      </div>

      <v-container>
        <form method="post">
          <input type="hidden" name="form-name" value="contact" />
          <p>
            <label>Your Name: <input type="text" name="name"/></label>
          </p>
          <p>
            <label>Your Email: <input type="email" name="email"/></label>
          </p>
          <p>
            <label>Message: <textarea name="message"></textarea></label>
          </p>
          <p>
            <button type="submit">Send</button>
          </p>
        </form>
      
      </v-container>
  </div>
  
</template>  

<script>
export default {
  name: 'contact',
  metaInfo: {
    title: 'Contact',

  meta: [
    {name: 'description', content:'Welcome!- Here you can contact me for more information'}
  ] 
  }
}
  
</script>

<style scoped>

.grid {
      padding: 20px;
      color: white;
}

form{
    width:100%;
    max-width: 900px;
    margin:20px auto;
    margin-bottom: 40px;
}

@media screen and (max-width:996px) {
    form{
        width:100%;
        max-width: 500px;
        margin:20px auto;
        margin-bottom: 40px;
    }
  }

  @media screen and (max-width:550px) {
    form{
        width:100%;
        max-width: 280px;
        margin:20px auto;
        margin-bottom: 40px;
    }
  }

  form p{
      color: black;
      font-size: 22px;
  }

  input, textarea{
    width: 900px;
    max-width: 100%;
    resize: none;
    background-color: white;
    height: 30px;
    }

  @media screen and (max-width:996px) {
    input, textarea{
        width: 500px;
        max-width: 100%;
        resize: none;
    }
  }

  @media screen and (max-width:550px) {
    input, textarea{
        width: 280px;
        max-width: 100%;
        resize: none;
    }
  }

  textarea{
    height: 200px;
}

  label{
    text-align: left;
    font-weight: 400;
}

  form button{
    background: #4A96AD;
    font-weight: bold;
    text-transform: uppercase;
    padding: 20px 30px;
    font-size: 18px;
    border:none;
    color:#fff;
}

  form p{
    text-align: left;

}

</style>

