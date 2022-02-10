<template>
  <div>
  
    <hero />
    <features-2 />
    <features-3 />
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
        Contact Us!
      </div>
    </div>
  </div>
</template>

<script>
import Features2 from '~/components/features2.vue'
import Features3 from '~/components/features3.vue'
import hero from '~/components/hero.vue'
export default {
  components: { hero, Features2, Features3 },

}
</script>

<style>

</style>