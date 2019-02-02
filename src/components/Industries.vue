<template>
  <div class="industries-container">
    <div class="industries-content">
      <h2>Industries</h2>
      <!-- eslint-disable -->
      <h4>Our services include concept development, idea generation, experience design, interaction design, systems design, education, workshops and more.</h4>
      <div class="industries-images">
        <span>
          <img src="../assets/Fintech.svg">
          Fintech
        </span>
        <span>
          <img src="../assets/Blockchain.svg">
          Blockchain
        </span>
        <span>
          <img src="../assets/Consumer.svg">
          Consumer
        </span>
        <span>
          <img src="../assets/Robotics.svg">
          Robotics
        </span>
        <span>
          <img src="../assets/Commerce.svg">
          Commerce
        </span>
        <span>
          <img src="../assets/AI.svg">
          A.I.
        </span>
      </div> <!-- Industries Images End -->
      <h5>Our global network of bright technical minds, entrepreneurs, scientists, creatives & operational experts allow us to solve even the most challenging design projects.</h5>
    </div> <!-- Industries Content End -->
  </div> <!-- Industries Container End -->
</template>

<script>
export default {
  name: 'industries',
};
</script>

<style lang="scss" scoped>
.industries-container {
  width: 100%;
  height: 100vh;
  background-color: #000;
  display: grid;
  grid-template-columns: 1fr 3fr 1fr;
  grid-template-rows: 1fr 4fr 1fr;
  grid-template-areas:
    ".    .     ."
    ".    info  ."
    ".    .     .";
  color: #fff;
  .industries-content {
    grid-area: info;
    display: grid;
    grid-gap: 50px;
    h2 {
      font-family: var(--header-font);
      font-size: 50px;
      align-self: end;
    }
    h4 {
      font-size: 35px;
      align-self: center;
    }
    .industries-images {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      grid-template-rows: repeat(2, 1fr);
      text-align: center;
      font-family: Arial, Helvetica, sans-serif;
      span {
        width: 100%;
        border: 0.1px solid #fff;
        display: grid;
        justify-content: center;
        align-items: center;
        padding: 100px 0;
      }
    }
    h5 {
      font-size: 30px;
      color: var(--blue);
    }
  }
}
</style>
