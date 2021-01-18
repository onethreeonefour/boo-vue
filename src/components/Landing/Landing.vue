<template>
  <div>
    <Hero />
    <About />
    <Contact />
  </div>
</template>

<script>
import Hero from "./Hero";
import About from "../About/About";
import Contact from "../Contact/Contact";
export default {
  components: {
    Hero,
    About,
    Contact,
  },
};
</script>
