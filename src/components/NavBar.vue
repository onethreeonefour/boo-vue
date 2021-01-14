<template>
  <header>
    <div class="container">
      <div class="logo-box">
        <a href="/">
          <img src="../assets/logo.webp" />
        </a>
      </div>
      <nav>
        <ul>
          <li><a href="">home</a></li>
          <li><a href="">work</a></li>
          <li><a href="">product</a></li>
          <li><a href="">about</a></li>
          <li><a href="">contact</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script></script>

<style scoped>
body {
  margin: 0;
}
header {
  padding: 20px 0;
  position: absolute;
  top: 0;
  width: 100%;
}
.container {
  padding: 0 50px;
  max-width: 90vw;
  margin: 0 auto;
}
.logo-box {
  float: left;
  margin-right: 20px;
  height: 100%;
  display: grid;
}
.logo-box a {
  outline: none;
  display: block;
}
.logo-box img {
  display: block;
}
nav {
  overflow: hidden;
}
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  float: right;
}
nav li {
  display: inline-block;
  margin-left: 25px;
  height: 70px;
  line-height: 55px;
  transition: 0.5s linear;
}
nav a {
  text-decoration: none;
  display: block;
  position: relative;
  color: black;
  text-transform: uppercase;
  font-weight: 500;
  font-size: 1.1rem;
}
nav a:after {
  content: "";
  width: 0;
  height: 2px;
  position: absolute;
  left: 0;
  bottom: 15px;
  background: black;
  transition: width 0.5s linear;
}
nav a:hover:after {
  width: 100%;
}

@media screen and (max-width: 660px) {
  header {
    text-align: center;
  }
  .logo-box {
    float: none;
    display: inline-block;
    margin: 0 0 16px 0;
  }
  ul {
    float: none;
  }
  nav li:first-of-type {
    margin-left: 0;
  }
}
@media screen and (max-width: 550px) {
  nav {
    overflow: visible;
  }
  nav li {
    display: block;
    margin: 0;
    height: 40px;
    line-height: 40px;
  }
  nav li:hover {
    background: rgba(0, 0, 0, 0.1);
  }
  nav a:after {
    content: none;
  }
}
</style>
