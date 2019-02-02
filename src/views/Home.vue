<template>
  <div class="home">
    <div class="info">
      <h2>Second Principle<span class="copy">&copy;</span></h2>
      <h1>We Start, Help & Fund Even More Fantastic Businesses</h1>
      <!-- eslint-disable -->
      <h3>We are a design based Venture Studio, based in New York City & led by industry veterans.</h3>
      <button>Let's Talk &rarr;</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'home',
};
</script>

<style lang="scss" scoped>
.home {
  width: 100%;
  height: 100vh;
  display: grid;
  grid-template-columns: 1fr 3fr 1fr;
  grid-template-rows: 1fr 4fr 1fr;
  // align-items: center;
  grid-template-areas:
    ".    .     ."
    ".    info  ."
    ".    .     .";
  color: #fff;
  background-color: #000;
  .info {
    grid-area: info;
    display: grid;
    grid-template-rows: 1fr 2fr repeat(2, 1fr);
    align-items: center;
    grid-gap: 20px;
    h2 {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
      font-size: 50px;
      .copy {
        font-size: 11px;
        color: var(--blue);
      }
    }
    h1 {
      font-family: var(--header-font);
      font-size: 65px;
      font-weight: 100;
      align-self: end;
    }
    h3 {
      font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
      font-size: 38px;
      font-weight: 100;
      color: #2c73d2;
    }
    button {
      align-self: start;
      width: 170px;
      height: 65px;
      background-color: rgba(0, 0, 0, 0);
      border: 3px solid var(--blue);
      border-radius: 50px;
      font-size: 15px;
      color: #2c73d2;
      transition: all 0.2s ease;
      &:hover {
        background-color: var(--blue);
        color: #fff;
        cursor: pointer;
      }
    }
  }

}
</style>
