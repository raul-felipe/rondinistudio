<template>
  <div class="hello">
    <div class="herovideo parallax">
      <div class="imgoverlay">
        <img class="heroimg" src="../assets/black.png" />
      </div>
      <video id="video" autoplay muted loop v-rellax="{ speed: 4 }">
        <source
          src="../assets/Rondini Studio - Demoreel - v2.mp4"
          type="video/mp4"
        />
      </video>
      <div class="overlay">
        <div class="">
          <div class="my-auto col-md-4 text-center" v-rellax="{ speed: 4 }">
            <h1>Bem vindo ao<br /><b>Rondini Studio</b></h1>
          </div>
        </div>
      </div>
    </div>
    <div class="parabody">
      <div
        class="hero z3 parallax"
        v-rellax="{ speed: 2, center: true }"
      >
        <div class="page-container">
          <h2>AQUI É BLACKWAII!</h2>
        </div>
        <div class="w-100 row h-100">
          <div class="my-auto">
            <h1
              class="d-flex justify-content-end"
              v-rellax="{ speed: 6, center: true }"
            >
              Bem vindo ao Rondini Studio!
            </h1>
          </div>
        </div>
      </div>

      <div class="parabody">
        <div
          class="hero z1 parallax"
          v-rellax="{ speed: 2, center: true }"
        ></div>
      </div>
      <div class="parabody">
        <div
          class="hero z2 parallax"
          v-rellax="{ speed: 2, center: true }"
        ></div>
      </div>
      <div class="parabody">
        <div
          class="hero z3 parallax"
          v-rellax="{ speed: 2, center: true }"
        ></div>
      </div>

      <div class="page-container">
        <h2>Venice</h2>

        <p>
          Venice is a city in northeastern Italy and the capital of the Veneto
          region. It is situated on a group of 118 small islands that are
          separated by canals and linked by over 400 bridges.
        </p>
        <p>
          Venice has been known as "La Dominante", "La Serenissima", "Queen of
          the Adriatic", "City of Water", "City of Masks", "City of Bridges",
          "The Floating City", and "City of Canals". The lagoon and a part of
          the city are listed as a UNESCO World Heritage Site. Parts of Venice
          are renowned for the beauty of their settings, their architecture, and
          artwork.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "HelloWorld",
    props: {
      msg: String,
    },
  };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
@font-face {
  font-family: "gotham-bold";
  src: url("../font/gotham-bold.otf") format("otf");
}

h1 {
  color: white;
  text-shadow: black 0.1em 0.1em 0.2em
  /* font-size: 350% !important; */
}

.overlay {
  width: 100%;
  position: absolute;
}

.imgoverlay {
  z-index: -1;
  width: 100%;
  background-image: linear-gradient(
    to top right,
    rgba(43, 0, 197, 0.404),
    #f06b0600
  );
}

.heroimg {
  width: 100%;
  z-index: -1;
  visibility: hidden;
}

.herovideo {
  width: 100%;
  min-height: 80vh;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}
@media screen and (orientation: portrait) {
  video {
    width: auto !important;
    height: 100%;
  }
}
video {
  top: 0;
  width: 100%;
  position: fixed;
  z-index: -2;
}

.parabody {
  width: 100%;
  min-height: 100vh;
}

.paraimg {
  width: 100%;
  position: fixed;
  z-index: -1;
}

div {
  font-family: "gotham-bold";
}
p {
  font-family: "gotham-bold";
}

body {
  padding-bottom: 50px;
  background-color: white;
}
.page-container {
  align-self: flex-start;
  padding: 10vh 0vw;
  width: 100%;
  background-color: white;
}

.parallax {
  background-attachment: fixed;
}

.hero {
  margin-top: -15vh;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  width: auto;
  height: 100vh;
  justify-content: center;
  align-items: center;
  position: relative;
}

.z1 {
  background-image: url("../assets/z1.png");
}

.z2 {
  background-image: url("../assets/z2.png");
}

.z3 {
  background-image: url("../assets/z3.png");
}


</style>
