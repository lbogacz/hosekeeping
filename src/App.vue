<template>
  <v-app>
    <NavBar></NavBar>
    <v-content>
      <router-view></router-view>
    </v-content>
  </v-app>
</template>

<script>
import NavBar from "./components/NavBar"
export default {
  name: "App",
  components: {NavBar},
  data() {
    return {
      //
    };
  }
};
</script>

<style lang="scss">
*, *::before, *::after{
  margin:0;
  padding:0;
  box-sizing: border-box;
}
body{
  background-color:#D9DCD6;
}
</style>
