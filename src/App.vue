<template>
  <Hero />
  <NavBar />

  <About />
</template>

<script>
import Hero from "./components/Hero";
import About from "./components/About";
import NavBar from "./components/NavBar";
export default {
  name: "App",
  components: {
    NavBar,
    Hero,
    About,
  },
};
</script>

<style>
@import "./Style.scss";
</style>
