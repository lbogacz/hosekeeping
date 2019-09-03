<template>
  <div class="contact">
    <p>If you are interested in our cleaning services, please contact us. We are happy to answer all your questions.</p>
    <div class="contact__form">
      <form method="POST" action="https://formspree.io/lukas.bogacz@gmail.com">
        <span>
          <input type="text" name="name" id="name" placeholder="name" required />
        </span>
        <span>
          <input type="email" name="email" id="email" placeholder="email" required />
        </span>
        <span>
          <textarea name="message" id="message" placeholder="message" required></textarea>
        </span>
        <span>
          <input type="submit" value="send" id="button" />
        </span>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contact",
  data() {
    return {};
  }
};
</script>

<style lang="scss" scoped>
.contact {
  height: 100%;
  margin-top: -15px;
  background-image: url(../assets/contact-details-3381225_1920.jpg);
  background-size: cover;
  background-position: left;
}
p {
  font-size: 18px;
  text-align: center;
  margin: 15px auto;
  padding: 25px;
  color: honeydew;
}
.contact__form {
  // border: 1px solid black;
  max-width: 500px;
  min-width: 250px;
  text-align: center;
  margin: 100px auto;
  // box-shadow: 1px 1px 2px black;
  form {
    display: grid;
    grid-auto-rows: auto;
    // border: 1px solid black;
    input {
      height: 30px;
      &::placeholder {
        text-transform: uppercase;
        text-align: center;
      }
    }
    textarea {
      height: 200px;
      resize: none;
      &::placeholder {
        text-transform: uppercase;
        text-align: center;
      }
    }
    textarea,
    input {
      width: 100%;
      outline: none;
      background-color: honeydew;
      opacity: 0.7;
      font-weight: bold;
      border: 1px;
      border-radius: 10px;
    }
    input[type=submit] {
      text-transform: uppercase;
    }
  }
  span {
    padding: 2px;
  }
}
</style>