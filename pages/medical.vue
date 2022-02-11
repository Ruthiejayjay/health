<template>
  <div>
  
    <hero />
    <features-2 />
    <features-3 />
    
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