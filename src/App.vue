<template>
  <Landing />
  <NavBar />
</template>

<script>
import NavBar from "./components/NavBar";
import Landing from "./components/Landing/Landing";
export default {
  name: "App",
  components: {
    NavBar,
    Landing,
  },
};
</script>

<style>
@import "./Style.scss";
</style>
