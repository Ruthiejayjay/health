<template>
  <div>
    
    <h-header />
    <features-1 />
  </div>
</template>

<script>
import Features1 from "~/components/features1.vue";
import hHeader from "~/components/hHeader.vue";
export default {
  components: { hHeader, Features1 },
  name: "IndexPage",
};
</script>
