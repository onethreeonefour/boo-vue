<template>
  <div class="about-container">
    <div class="about-container-text">
      <h1>
        WELCOME TO BOOSTUDIO! <br />
        YOUR BRAND ACTIVATION PARTNER
      </h1>
      <h2>
        Helping you deliver unique, impactful brand experiences in retail,
        design, events, & technology.
      </h2>
      <h3>
        Established in February 2018 into the existing "BOO" family of
        companies, BOOStudio was founded as a service agency specialising in
        design & production, nationwide installations & events, warehousing &
        logistics and technology.
      </h3>
      <button>See Our Works</button>
    </div>
    <div>
      <img src="./collab.webp" alt="collaborate-office-ladies" />
    </div>
  </div>
  <div>
    <Showcase />
  </div>
</template>

<script>
import Showcase from "./Showcase";

export default {
  components: {
    Showcase,
  },
};
</script>

<style scoped>
.about-container {
  display: flex;
  margin: auto;
  background-color: #cf5727;
  padding: 5rem;
  color: white;
  gap: 2rem;
  place-content: center;
}
.about-container-text {
  display: grid;
  place-content: center;
}
img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 5px;
}
h1 {
  font-family: "Roboto Condensed", sans-serif;
  font-size: 2.4rem;
}
h2 {
  font-family: "Roboto Condensed", sans-serif;
  font-weight: 200;
  font-size: 1.4rem;
  margin-top: 2rem;
}
h3 {
  font-family: "Roboto Condensed", sans-serif;
  margin-top: 2rem;
  font-size: 1.1rem;
  font-weight: 300;
}
button {
  margin-top: 2rem;
  padding: 1rem 1.5rem 1rem 1.5rem;
  font-size: 1.1rem;
  background-color: #0c1820;
  color: white;
  cursor: pointer;
  border-color: #0c1820;
  border-radius: 2rem;
  width: 20%;
}
</style>
