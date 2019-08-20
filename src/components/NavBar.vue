<template>
  <nav app>
    <v-toolbar flat height="130px" app class="hidden-md-and-up">
      <div class="image-logo">
        <v-img :src="require('../assets/cleaning-3934664_1920.jpg')"></v-img>
      </div>
      <v-spacer></v-spacer>
      <v-toolbar-side-icon @click="drawer=!drawer" class="hidden-md-and-up"></v-toolbar-side-icon>
    </v-toolbar>
    <v-navigation-drawer v-model="drawer" app right class="hidden-md-and-up">
      <v-btn @click="drawer=!drawer" flat>
        <v-icon>exit_to_app</v-icon>
      </v-btn>
      <v-list>
        <v-list-tile v-for="item in items" :key="item.text" router :to="item.route">
          <v-list-tile-action>
            <v-icon>{{item.icon}}</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title>{{item.text}}</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    <v-toolbar flat height="130px" app class="hidden-sm-and-down">
      <div class="image-logo">
        <v-img :src="require('../assets/cleaning-3934664_1920.jpg')"></v-img>
      </div>
      <v-spacer></v-spacer>
      <v-toolbar-items>
        <v-btn flat v-for="item in items" :key="item.text"  router :to="item.route" class="title white--text">{{item.text}}</v-btn>
      </v-toolbar-items>
    </v-toolbar>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      drawer: false,
      items: [
        { icon: "dashboard", text: "Home", route: '/' },
        { icon: "person", text: "About Me", route: '/about' },
        { icon: "local_offer", text: "Offerts", route: '/offerts' },
        { icon: "monetization_on", text: "Prices", route: '/prices' },
        { icon: "contact_phone", text: "Contact", route: '/contact' }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.v-toolbar {
  background-color: #1f4f53;
}
.image-logo {
  position: relative;
  width: 200px;
  height: 130px;
  top: 0px;
  left: 0px;
}

.v-navigation-drawer {
  // z-index: 10;
  background-color: #a5d8ff;
  .v-btn {
    position: relative;
    left: 220px;
  }
}
</style>
