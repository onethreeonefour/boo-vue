<template>
  <div class="showcase-container">
    <div class="showcase-images">
      <div v-for="el in projectData" v-bind:key="el" class="card">
        <img :src="getImgUrl(el.src)" alt="project-image" />
      </div>
    </div>
    <div class="showcase-text-container">
      <div>
        <h1>Design</h1>
        <h2>
          Our team will help you discover your ‘Brand Attraction' through
          creative design.
        </h2>
      </div>
      <div>
        <h1>
          Installation
        </h1>
        <h2>
          Expert break-fix, installation, and retail solutions to ensure your
          displays, storefronts and products are ready to meet your customers
        </h2>
      </div>
      <div>
        <h1>Production</h1>
        <h2>
          We like to get great sh*t done. And quickly. Through creative design,
          graphics, expert carpentry and fabrication we produce exciting brand
          experiences.
        </h2>
      </div>
      <div>
        <h1>
          Activation & Events
        </h1>
        <h2>
          Creating unique activations and events that capture attention, make
          lasting memories and drive genuine impact.
        </h2>
      </div>
      <div>
        <h1>
          Technology
        </h1>
        <h2>
          BOOHUB is a custom CRM we've developed to manage your business the
          correct way.
        </h2>
      </div>
    </div>
  </div>
  <!-- <div class="boohub-container">
    <h1>An Agency Trusted By</h1>
  </div> -->
</template>

<script>
export default {
  data() {
    return {
      projectData: [
        {
          src: "project-images/1.webp",
          name: "Don Julio",
        },
        {
          src: "project-images/15.webp",
          name: "Pixel Launch ",
        },
        {
          src: "project-images/21.webp",
          name: "Tanqueray Terrace",
        },
        {
          src: "project-images/22.webp",
          name: "Panhead Brewery",
        },
        {
          src: "project-images/7.webp",
          name: "Kirin",
        },
        {
          src: "project-images/14.webp",
          name: "Smirnoff",
        },
      ],
    };
  },
  methods: {
    getImgUrl(pic) {
      return require("../../assets/" + pic);
    },
  },
};
</script>
<style lang="scss" scoped>
.showcase-container {
  background-color: rgb(245, 245, 245);
  display: flex;
  gap: 3rem;
  padding: 4rem;
  place-content: center;
  .showcase-images {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1rem;
  }
  .card {
    img {
      height: 100%;
      width: 100%;
      display: block;
      object-fit: cover;
      border-radius: 5px;
    }
  }
}
.showcase-text-container {
  display: grid;
  place-content: center;
  h1 {
    font-size: 2.75rem;
    font-family: "Roboto Condensed", sans-serif;
  }
  h2 {
    font-size: 1.2rem;
    font-weight: 100;
    font-family: "Poppins", sans-serif;
    padding: 1rem 0 1rem 0;
  }
}
.boohub-container {
  background-color: #252e3a;
  color: white;
  display: flex;
  gap: 3rem;
  padding: 4rem;
  place-content: center;
}
</style>
