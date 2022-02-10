<template>
  <div>
    <div class="relative h-32 w-32 ...">
      <div
        class="
          fixed
          bottom-0
          right-0
          h-16
          w-36
          bg-gradient-to-br
          from-purple-500
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
