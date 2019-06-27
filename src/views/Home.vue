<template>
  <div class="home">
    <h1>Lorem ipsum dolor sit</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis inventore consectetur architecto sapiente dolor vero, facilis, itaque laudantium debitis quis quia, odit optio amet ea praesentium iste a illo magni!</p>

    <h2>Lorem ipsum dolor, sit.</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores officiis quas ea quis vero quisquam reprehenderit dolorem consequatur similique architecto, beatae numquam, obcaecati quaerat ipsum excepturi eius doloremque aliquam laudantium!</p>
    <v-container>
      <v-layout justify-space-around row wrap>
        <v-flex xs12 sm12 pb-4>
          <div class="overlay-kitchen">
            <div class="text-kitchen">
              <p>kitchen</p>
            </div>
          </div>
          <v-img :src="require('../assets/cleanliness-2799459_1920.jpg')"></v-img>
        </v-flex>

        <v-flex xs12 sm12 pb-4>
          <div class="overlay-hoover">
            <div class="text-hoover">
              <p>hoover</p>
            </div>
          </div>
          <v-img :src="require('../assets/cleanliness-2799464_1920.jpg')"></v-img>
        </v-flex>

        <v-flex xs12 sm12 pb-4>
          <div class="overlay-gloves">
            <div class="text-gloves">
              <p>hoover</p>
            </div>
          </div>
          <v-img :src="require('../assets/cleanliness-2799470_1920.jpg')"></v-img>
        </v-flex>

        <v-flex xs12 sm12 pb-4>
          <div class="overlay-hob">
            <div class="text-hob">
              <p>hoover</p>
            </div>
          </div>
          <v-img :src="require('../assets/cleanliness-2799475_1920.jpg')"></v-img>
        </v-flex>

        <v-flex xs12 sm12 pb-4>
          <div class="overlay-bathroom">
            <div class="text-bathroom">
              <p>hoover</p>
            </div>
          </div>
          <v-img :src="require('../assets/cleanliness-2799496_1920.jpg')"></v-img>
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
.text-kitchen,
.text-hoover,
.text-gloves,
.text-hob,
.text-bathroom {
  display: none;
}
</style>

