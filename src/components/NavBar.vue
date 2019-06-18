<template>
  <nav>
    <v-toolbar flat height="110px">
      <v-img :src="require('../assets/cleaning-3934664_1920.jpg')"></v-img>
      <v-spacer></v-spacer>
      <v-toolbar-side-icon @click="drawer=!drawer"></v-toolbar-side-icon>
    </v-toolbar>
    <v-navigation-drawer v-model="drawer" app right class="#A5D8FF">
      <v-btn @click="drawer=!drawer" class="A5D8FF" flat right>
        <v-icon>exit_to_app</v-icon>
      </v-btn>
      <v-list>
        <v-list-tile>
          <v-list-tile-content>
            <v-list-tile-title></v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
  </nav>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      drawer: false
    };
  }
};
</script>

<style lang="scss" scoped>
.v-toolbar {
  background-color: #1f4f53;
  .v-img {
    position: relative;
    width: 200px;
    height: 100px;
    top: 0px;
    left: 0px;
  }
}
</style>
