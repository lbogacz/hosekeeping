<template>
  <v-app>
    <NavBar></NavBar>
    <v-content>
      <router-view></router-view>
    </v-content>
    <Footer></Footer>
  </v-app>
</template>

<script>
import NavBar from "./components/NavBar";
import Footer from "./components/Footer";
export default {
  name: "App",
  components: { NavBar, Footer },
  data() {
    return {

    };
  }
};
</script>

<style lang="scss" scoped>
@import url("https://fonts.googleapis.com/css?family=PT+Sans");
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "PT Sans", sans-serif;
}
* {
  background-color: #d9dcd6;
}
</style>
