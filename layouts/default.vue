<template>
  <div v-if="alphineready">
      <h-nav />

      <nuxt />
        <cta />
      <h-footer />
       <div class="relative h-32 w-32 ...">
      <div
        class="
          fixed
          bottom-0
          right-0
          h-16
          w-36
          bg-gradient-to-br
          from-purple-700
          via-red-500
          to-pink-600
          px-3
          py-4
          font-medium
          text-white
          rounded-lg
        "
      >
        Contact Us
      </div>
    </div>
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