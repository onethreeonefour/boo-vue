<template>
  <div class="hero" id="hero">
    <div class="hero-cta-container">
      <div>
        <h1><span>boo</span>studio</h1>
        <h2>Bringing Your Product To New Heights</h2>
        <h3>Design, Activation, Digital & Events Agency - Sydney, Australia</h3>
        <div class="cta-button-container">
          <button>Free Evaluation</button>
          <button>Our Works</button>
        </div>
      </div>
      <div class="hero-image-container">
        <img src="../assets/2.webp" alt="hero" />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  mounted() {
    window.nakerback.render({
      container: document.getElementById("hero"),
      particle: {
        life: 5,
        power: 0.055,
        texture:
          "https://res.cloudinary.com/naker-io/image/upload/v1610674163/rvhkybxfzw8aoko5kpby.png",
        number: 165,
        colorStart: [255, 0, 0, 0.3],
        colorEnd: [255, 255, 255, 0.8],
        sizeStart: 0.5,
        sizeEnd: 1,
        direction1: { x: 10, y: 120, z: 0 },
        direction2: { x: 0, y: 0, z: 0 },
        waterMark: false,
      },
      environment: {
        sensitivity: 0.8,
      },
    });
  },
};
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped style="scss">
@font-face {
  font-family: Roboto-Bold;
  src: url("../fonts/Roboto/RobotoCondensed-Bold.ttf");
}
@font-face {
  font-family: Roboto-Thin;
  src: url("../fonts/Roboto/RobotoCondensed-Light.ttf");
}
canvas {
  z-index: 5000;
  width: 100%;
  height: 100%;
}
.hero {
  background-color: rgb(252, 250, 250);
  display: grid;
  align-items: center;
  justify-content: center;
  height: 100vh;
}
.hero-cta-container {
  display: flex;
  color: black;
  gap: 3rem;
  align-items: center;
}
.cta-button-container {
  display: flex;
  gap: 1rem;
}
button {
  margin-top: 2rem;
  background-color: #cf5727;
  padding: 1rem 1.5rem 1rem 1.5rem;
  color: white;
  font-size: 1.1rem;
  border-color: #cf5727;
  border-style: solid;
  outline-color: #cf5727;
  cursor: pointer;
  transition: 0.2s ease-in-out all;
  border-radius: 2rem;
}
button:hover {
  background: transparent;
  color: black;
}
button:nth-child(2) {
  background-color: transparent;
  border-color: #0c1820;
  color: black;
}
button:nth-child(2):hover {
  background-color: #0c1820;
  color: white;
}
span {
  color: rgba(0, 0, 0, 0.8);
  font-family: Roboto-Bold;
  letter-spacing: -2.5px;
}
h1 {
  color: rgba(0, 0, 0, 0.6);
  font-family: Roboto-Thin;
  font-size: 5.25rem;
}
h2 {
  font-family: Roboto-Thin;
  font-size: 2.5rem;
  padding-bottom: 1rem;
}
.hero-image-container {
  display: flex;
  gap: 1rem;
}

img {
  display: block;
  width: auto;
  height: 50vh;
  object-fit: cover;
}
</style>
