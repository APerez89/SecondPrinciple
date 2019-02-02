<template>
  <div class="clients-container">
    <div class="clients-content">
      <h2>Client & Partners</h2>
      <!-- eslint-disable -->
      <h4>We help entrepreneurs & corporations create category defining products around the world.</h4>
      <div class="client-images">
        <span class="google"><img src="../assets/google.svg" alt="Google"></span>
        <span class="skype"><img src="../assets/skype.svg" alt="Skype"></span>
        <span class="tata"><img src="../assets/tata.svg" alt="Tata"></span>
        <span class="alibaba"><img src="../assets/alibaba.svg" alt="Alibaba"></span>
        <span class="square"><img src="../assets/square.svg" alt="Square"></span>
        <span class="cedar"><img src="../assets/cedar.svg" alt="Cedar"></span>
        <span class="amazon"><img src="../assets/amazon.svg" alt="Amazon"></span>
        <span class="vodafone"><img src="../assets/vodafone.svg" alt="Vodafone"></span>
        <span class="nokia"><img src="../assets/nokia.svg" alt="Nokia"></span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'clients',
};
</script>

<style lang="scss" scoped>
.clients-container {
  width: 100%;
  height: 100vh;
  background-color: var(--blue);
  display: grid;
  grid-template-columns: 1fr 3fr 1fr;
  grid-template-rows: 1fr 4fr 1fr;
  grid-template-areas:
    ".    .     ."
    ".    info  ."
    ".    .     .";
  color: #fff;
  .clients-content {
    grid-area: info;
    display: grid;
    grid-template-rows: 1fr 1fr 4fr;
    h2 {
      font-family: var(--header-font);
      font-size: 50px;
      align-self: end;
    }
    h4 {
      font-size: 35px;
      align-self: center;
    }
    .client-images {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      grid-template-rows: repeat(3, 1fr);
      span {
        width: 100%;
        border: 0.1px solid #fff;
        display: grid;
        justify-content: center;
        align-items: center;
        padding: 100px 0;
      }
    }
  }
}
</style>
