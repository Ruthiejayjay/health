<template>
  <div>
      <hero-2 />
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
import hero2 from '~/components/hero2.vue'
export default {
  components: { hero2 },

}
</script>

<style>

</style>