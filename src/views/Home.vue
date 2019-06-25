<template>
  <div>
    <h1>Lorem ipsum dolor sit</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis inventore consectetur architecto sapiente dolor vero, facilis, itaque laudantium debitis quis quia, odit optio amet ea praesentium iste a illo magni!</p>

    <h2>Lorem ipsum dolor, sit.</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores officiis quas ea quis vero quisquam reprehenderit dolorem consequatur similique architecto, beatae numquam, obcaecati quaerat ipsum excepturi eius doloremque aliquam laudantium!</p>
    <v-container>
      <v-layout justify-space-around>
        <v-flex xs12 sm12>
          <div class="overlay">
            <div class="text">
              <p>kitchen</p>
            </div>
          </div>
          <v-img :src="require('../assets/cleanliness-2799459_1920.jpg')"></v-img>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>
 <script>
export default {
  name: "Home",
  data() {
    return {};
  }
};
</script>

<style lang="scss" scope>
h1,
h2,
p {
  text-align: center;
  margin: auto;
  padding: 15px;
}

h1,
h2 {
  max-width: 250px;
}
p {
  max-width: 400px;
}
.text {
  display: none;
}
</style>

