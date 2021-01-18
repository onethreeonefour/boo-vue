<template>
  <div class="contact-container">
    <h1>Get in touch today, we’d love to hear from you!</h1>
    <div class="contact-container-flex">
      <div class="details">
        <img src="./team.webp" alt="team-cartoon" />
        <h2>Our Office</h2>
        <p>
          101-103 Illawarra Road <br />
          Marrickville, NSW 2204 <br />
          Sydney, Australia
        </p>
        <h2>Phone Us At</h2>
        <p>1800 957 466</p>
        <div className="trading-hours">
          <p>Mon-Fri: 9pm - 5pm</p>
          <p>Sat-Sun: Only By Special Request</p>
        </div>
      </div>
      <div class="form">
        <h1>Email Us</h1>
        <label for="name">Name</label>
        <input type="text" />
        <label for="email">Email</label>
        <input type="text" />
        <label for="enquiry">Enquiry</label>
        <textarea name="enquiry" id="enquiry" cols="30" rows="10"></textarea>
        <button>Submit</button>
      </div>
    </div>
  </div>
</template>
<script>
export default {};
</script>

<style lang="scss" scoped>
.contact-container {
  display: grid;
  align-items: center;
  justify-content: center;
  place-content: center;
  padding: 4rem;
  color: white;
  font-family: "Roboto Condensed", sans-serif;
  text-transform: uppercase;
  background-color: #cf5727;
}
.contact-container-flex {
  display: flex;
  gap: 1rem;
}
.details {
  color: black;
  background-color: white;
  padding: 4rem;
  margin-top: 2rem;
  border-radius: 0.5rem;
  box-shadow: 4px 4px 10px rgba(0, 0, 0, 0.2);
  h2 {
    padding: 1rem 0 1rem 0;
  }
  .trading-hours {
    background-color: rgba(0, 0, 0, 0.884);
    margin: 2rem auto auto auto;
    color: white;
    padding: 1.75rem;
    border-radius: 5px;
  }
}
.form {
  width: 50vw;
  display: grid;
  color: black;
  background-color: white;
  padding: 4rem;
  margin-top: 2rem;
  border-radius: 0.5rem;
  box-shadow: 4px 4px 10px rgba(0, 0, 0, 0.2);
  label {
    padding: 1rem 0 1rem 0;
  }
  input,
  textarea {
    padding: 0.5rem;
    cursor: pointer;
  }
  button {
    font-family: "Poppins", sans-serif;
    margin-top: 2rem;
    font-size: 1rem;
    padding: 1rem 1.5rem 1rem 1.5rem;
    color: white;
    background-color: black;
    border-color: #0c1820;
    border-style: solid;

    transition: 0.2s ease-in-out all;
    border-radius: 2rem;
    font-weight: 800;
    z-index: 9000;
  }
  button:hover {
    background-color: white;
    color: black;
    border-color: black;
  }
}
</style>
