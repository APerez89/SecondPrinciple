<template>
  <div id="app">
    <router-view/>
    <OurClients />
    <Industries />
    <About />
  </div>
</template>

<script>
import OurClients from '@/components/OurClients.vue';
import Industries from '@/components/Industries.vue';
import About from '@/components/About.vue';

export default {
  components: {
    OurClients,
    Industries,
    About,
  },
};
</script>


<style lang="scss">
:root {
  --header-font: 'Roboto Slab', serif;
  --subheader-font: Arial, Helvetica, sans-serif;
  --blue: #2c73d2;
}

* {
  box-sizing: border-box;
  margin: 0;
}

h4, h5 {
  font-family: var(--subheader-font);
  font-weight: 100;
}
</style>
