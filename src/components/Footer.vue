<template>
  <footer>
    <v-footer height="250">
      <div class="footer">
        <p>Design by lbogacz &copy;{{new Date().getFullYear()}}</p>
      </div>
    </v-footer>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {};
  }
};
</script>

<style lang="scss" scoped>
.v-footer {
  background-image: url(..//assets/hse-3464155_1920.jpg);
  background-position: 30% 60%;
  background-size: cover;
  background-repeat: no-repeat;
}
.footer {
  position: absolute;
  bottom: 0;
  left: 0;
  color: #fff;
}
</style>
