<template>
  <div class="home">
    <div class="home-header">
      <h1>Shine Cleaning services</h1>
      <p>Welcome to the cleaning company website. We provide professional cleaning services, we adjust the range of our services to individual wishes and preferences of clients. We work both for private individuals and for various types of companies and institutions. Our professionalism and commitment to the work performed has already been appreciated by many customers.</p>

      <p>Our offer of cleaning services is directed to those people and companies who for various reasons need professional help in maintaining order and cleanliness.</p>
      <p>Only regular cleaning will ensure that the rooms are clean and user-friendly. A good alternative for indyvidual cleaning, which is usually lacking in time and willingness, is the employment of a cleaning lady who will take over your not liked duties related to cleaning.</p>
    </div>
    <div class="main-content">
      <div class="images">
        <img v-for="picture in pictures" :key="picture.img " :src="picture.img" />
      </div>
    </div>
    <div class="home-header">
      <h2>Lorem ipsum dolor, sit.</h2>
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
  h2,
  h3,
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
    h2 {
      font-size: 200%;
      text-align: center;
      margin: auto;
      padding: 15px;
      max-width: 80%;
    }

    p {
      text-align: center;
      margin: auto;
      padding: 15px;
      font-size: 140%;
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

