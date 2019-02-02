<template>
  <div class="about-container">
    <div class="about-content">
      <h2>About</h2>
      <!-- eslint-disable -->
      <h4>First Principle was founded by Thomas Petersen who previously led design across multiple product teams at Square for almost five years. During that time, he developed some of the core products and services that exist there today, taking it from start-up through an incredibly successful IPO.</h4>
      <h4>Thomas has worked with more than a 100 different organizations spanning from large Fortune 500 companies to early stage startups. Thomas co-founded Hello Group in 2006 which was sold to NOA Group in 2018 and spent some time with the internationally acclaimed 80/20 before they were acquired by Square in 2012</h4>
    </div> <!-- About Content End -->
  </div> <!-- About Container End -->
</template>

<script>
export default {
  name: 'about',
};
</script>

<style lang="scss" scoped>
.about-container {
  width: 100%;
  height: 100vh;
  background-color: var(--blue);
  display: grid;
  grid-template-columns: 1fr 3fr 1fr;
  // grid-template-rows: 1fr 4fr 1fr;
  grid-template-areas:
    ".    .     ."
    ".    info  ."
    ".    .     .";
  color: #fff;
  .about-content {
    grid-area: info;
    display: grid;
    grid-template-rows: 1fr 3fr;
    h2 {
      font-family: var(--header-font);
      font-size: 50px;
      align-self: end;
    }
    h4 {
      font-size: 35px;
      align-self: center;
    }
  }
}
</style>
