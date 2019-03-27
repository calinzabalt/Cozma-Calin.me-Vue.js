 <template>
     <div>
   <v-navigation-drawer
      v-model="drawer"
      fixed
      app
    >
      <v-list>
        <v-list-tile to="/">
          <v-list-tile-action>
            <v-icon>home</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Home</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile to="/work">
          <v-list-tile-action>
            <v-icon>work</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Work</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile to="/contact">
          <v-list-tile-action>
            <v-icon>school</v-icon>
          </v-list-tile-action>
           <v-list-tile-content>
            <v-list-tile-title>Blog</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
        <v-list-tile to="/contact">
          <v-list-tile-action>
            <v-icon>email</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>Contact</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar color="indigo" dark fixed app>
      <v-toolbar-side-icon @click.stop="drawer = !drawer"></v-toolbar-side-icon>
      <v-toolbar-title>Cozma Calin</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn flat to="/#">Home</v-btn>
        <v-btn flat to="/work">Work</v-btn>
        <v-btn flat href="https://calinzabalt.github.io/CozmaCalin-Blog/" target="blank">Blog</v-btn>
        <v-btn flat to="/contact">Contact</v-btn>
      </v-toolbar-items>  
    </v-toolbar>

</div>
</template>   

<script>

  export default {
    data: () => ({
      drawer: false
    }),
    props: {
      source: String
    }
  }
</script>