<template>
  <div class="home">
    <div class="home-header">
      <h1>Lorem ipsum dolor sit</h1>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis inventore consectetur architecto sapiente dolor vero, facilis, itaque laudantium debitis quis quia, odit optio amet ea praesentium iste a illo magni!</p>

      <h2>Lorem ipsum dolor, sit.</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores officiis quas ea quis vero quisquam reprehenderit dolorem consequatur similique architecto, beatae numquam, obcaecati quaerat ipsum excepturi eius doloremque aliquam laudantium!</p>
    </div>
    <div class="main-content">
      <div class="images">
        <img v-for="picture in pictures" :key="picture.img " :src="picture.img" />
      </div>
    </div>
    <div class="home-header">
    <h3>Lorem ipsum dolor, sit.</h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores officiis quas ea quis vero quisquam reprehenderit dolorem consequatur similique architecto, beatae numquam, obcaecati quaerat ipsum excepturi eius doloremque aliquam laudantium!</p>
    </div>
  </div>
</template>
 <script>
export default {
  name: "Home",
  data() {
    return {
      pictures: [
        { img: require("@/assets/cleanliness-2799459_1920.jpg") },
        { img: require("@/assets/cleanliness-2799464_1920.jpg") },
        { img: require("@/assets/cleanliness-2799470_1920.jpg") },
        { img: require("@/assets/cleanliness-2799475_1920.jpg") },
        { img: require("@/assets/cleanliness-2799496_1920.jpg") }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.home-header {
  h1,
  h2,h3,
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
}

.images {
  img {
    width: 100%;
    padding-bottom: 15px;
  }
}

@media (min-width: 500px) {
  .home-header {
    font-size: 15px;
  }
}

@media (min-width: 600px) {
  .home-header {
    h1,
    h2 {
      max-width: 350px;
    }
    p {
      max-width: 500px;
    }
  }
}

@media (min-width: 700px) {
  .home-header {
    font-size: 16px;
    h1,
    h2 {
      max-width: 400px;
    }
    p {
      max-width: 550px;
    }
  }
}

@media (min-width: 800px) {
  .home-header {
    h1,
    h2 {
      max-width: 500px;
    }
    p {
      max-width: 650px;
    }
  }
}

@media (min-width: 950px) {
  .home-header {
    h1,
    h2,
    p {
      text-align: center;
      margin: auto;
      padding: 15px;
      font-size:140%;
    }
    h1,
    h2,
    p {
      max-width: 80%;
    }
  }

  .images {
    display: flex;
    flex-wrap: wrap;
    flex-direction: row;
    justify-content: center;
    max-height: 100vh;
  }
  img {
    max-width: 25vw;
    padding: 10px;
  }
}
</style>

