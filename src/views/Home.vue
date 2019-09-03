<template>
  <div class="home">
    <div class="home-header">
      <h1>
        <span>
          <img src="../assets/diamond-158431_1280.png" />
        </span>
        Shine cleaning services
      </h1>
      <p>Welcome to the cleaning company website. We provide professional cleaning services, we adjust the range of our services to individual wishes and preferences of clients. We work both for private individuals and for various types of companies and institutions. Our professionalism and commitment to the work performed has already been appreciated by many customers.</p>

      <p>Our offer of cleaning services is directed to those people and companies who for various reasons need professional help in maintaining order and cleanliness.</p>
      <p>Only regular cleaning will ensure that the rooms are clean and user-friendly. A good alternative for indyvidual cleaning, which is usually lacking in time and willingness, is the employment of a cleaning lady who will take over your not liked duties related to cleaning.</p>
    </div>
    <div class="main-content">
      <div class="images">
        <img v-for="picture in pictures" :key="picture.img " :src="picture.img" />
      </div>
    </div>
    <div class="about-company">
      <h2>About company</h2>
      <img src="../assets/heather-ford-1270604-unsplash.jpg" />

      <p>
        We are a professional cleaning company with experience. We offer comprehensive cleaning of apartments and offices at favorable prices. We guarantee the highest standard of cleaning and additional services.
        You can often find the opinion that it is not easy to find a good and at the same time inexpensive cleaner or - in the case of companies and institutions - cleaning company. The fact is that there are many entities providing similar services on the market as we do, but not always clients of these companies are satisfied with their work. However, it is not worth spreading this unfavorable opinion to all cleaning companies, because on the other hand there are companies such as ours, for whom the highest quality of services and the satisfaction of each client are a priority. We believe that this is the only way to build a company's reputation and encourage new customers to cooperate with us. Words unsupported by deeds do not mean much - that's why, as cleaning specialists, we engage 100% in every job. The cleaning lady from our cleaning company guarantees a perfect work, with attention to every detail and property entrusted to us. It's not without reason that our services are so eagerly recommended by our existing customers.
      </p>
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
  @media (min-width: 500px) {
    font-size: 15px;
  }
  @media (min-width: 700px) {
    font-size: 16px;
  }
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
    @media (min-width: 600px) {
      max-width: 350px;
    }
    @media (min-width: 700px) {
      max-width: 400px;
    }
    @media (min-width: 800px){
      max-width: 500px;

    }
  }
  p {
    max-width: 400px;
    @media (min-width: 600px) {
      max-width: 500px;
    }
    @media (min-width: 700px) {
      max-width: 550px;
    }
    @media (min-width: 800px){

    }
  }

  span {
    img {
      height: 10vh;
      display: block;
      text-align: center;
      margin: auto;
    }
  }
}

.images {
  img {
    width: 100%;
    padding-bottom: 15px;
  }
}

.about-company {
  text-align: center;
  img {
    display: none;
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
    h1 {
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
    max-height: 100vh;
    max-width: 25vw;
    padding: 10px;
  }
  .about-company {
    max-width: 100%;
    background-color: rgb(196, 179, 179);
    margin-top: 20px;

    h2 {
      font-size: 200%;
      padding: 30px;
    }

    h2,
    p {
      text-align: center;
      margin: auto;
    }
    p {
      max-width: 80%;
      font-size: 140%;
      padding: 15px;
    }
  }
}

@media (min-width: 960px) {
  .about-company {
    h2 {
      margin-left: 20%;
    }
    img {
      display: inline-block;
      position: relative;
      left: 0;
      top: -100px;
      max-height: 100vh;
      max-width: 25vw;
    }
    p {
      font-size: 140%;
      display: inline-block;
      max-width: 70%;
      position: relative;
      left: 0;
      top: -20px;
    }
  }
}

@media (min-width: 1040px) {
  .about-company {
    margin-top: 20px;
    padding: 30px;

    h2 {
      margin-left: 40%;
      font-size: 200%;
      padding: 30px;
    }
    img {
      display: inline-block;
      position: relative;
      top: -20px;
      left: 0;
      max-height: 50vh;
      max-width: 25vw;
    }
    p {
      font-size: 140%;
      display: inline-block;
      max-width: 65%;
      position: relative;
      left: 10%;
    }
  }
}

@media (min-width: 1400px) {
  .home-header,
  .about-company {
    line-height: 30px;
  }
  .about-company {
    h2 {
      margin-left: 20%;
      font-size: 200%;
      padding: 30px;
    }
    img {
      left: 8%;
      max-height: 50vh;
      max-width: 25vw;
    }
    p {
      max-width: 60%;
      position: relative;
      top: -60px;
    }
  }
}
@media (min-width: 1600px) {
  .home-header,
  .about-company {
    line-height: 40px;
  }
  .about-company {
    p {
      top: -40px;
    }
  }
}

@media (min-width: 1900px) {
  .about-company {
    p {
      top: -80px;
    }
  }
}

@media (min-width: 2060px) {
  .about-company {
    p {
      top: -100px;
    }
  }
}
</style>