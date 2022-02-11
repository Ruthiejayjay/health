<template>
  <div>
     <hero-4 />
     <features-5 />
     <features-4 />
  </div>
</template>

<script>
import Features4 from '~/components/features4.vue'
import Features5 from '~/components/features5.vue'
import hero4 from '~/components/hero4.vue'
export default {
  components: { hero4, Features4, Features5 },

}
</script>

<style>

</style>