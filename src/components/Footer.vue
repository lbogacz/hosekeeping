<template>
  <footer>
    <v-footer height="400">
      <div class="footer">
        <p>Design by lbogacz &copy;{{new Date().getFullYear()}}</p>
      </div>
      <!-- <div class="img">
        <v-img :src="require('../assets/hse-3464155_1920.jpg')"></v-img>
      </div>-->
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
// .img{
//   width: 400px;
//   height: 400px;
// }
.v-footer {
  background-image: url(..//assets/hse-3464155_1920.jpg);
  background-position:center;
  background-size:cover;
  background-repeat: no-repeat;

}
.footer {
  position: absolute;
  bottom: 0;
  left: 0;
  color: #fff;
}
</style>
