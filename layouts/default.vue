<template>
  <div v-if="alphineready">
      <h-nav />

      <nuxt />
        <cta />
      <h-footer />
  </div>
</template>


<script>
import Cta from '~/components/cta.vue';
import HFooter from '~/components/hFooter.vue';
import hNav from '~/components/hNav.vue';
export default {
  components: { hNav, HFooter, Cta },
      data() {
    return {
      alphineready: false,
    };
  },

  head() {
    return {
      title: "health equips", // Other meta information
      script: [
        {
          hid: "alphine",
          src: "https://cdnjs.cloudflare.com/ajax/libs/alpinejs/2.8.0/alpine.js",
          // Changed after script load
          callback: () => {
            this.alphineready = true;
          },
        },
      ],
    };
  },
}
</script>

<style>

</style>