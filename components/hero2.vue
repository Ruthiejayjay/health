<template>
  <!-- Section 1 -->
  <section class="relative w-full bg-center bg-cover h11">
    <div
      class="
        absolute
        inset-0
        bg-gradient-to-br
        from-pink-900
        via-pink-700
        to-pink-400
        opacity-70
      "
    ></div>

    <div class="mx-auto max-w-7xl">
      <div class="flex flex-col items-center px-10 pt-20 pb-40 lg:flex-row">
        <div class="relative w-full max-w-2xl bg-cover lg:w-7/12">
          <div
            class="
              relative
              flex flex-col
              items-center
              justify-center
              w-full
              h-full
              lg:pr-10
            "
          >
            <div class="flex flex-col items-start space-y-8">
              <div class="relative">
                <h1
                  class="
                    text-2xl
                    font-extrabold
                    leading-tight
                    text-gray-100
                    sm:text-5xl
                    md:text-6xl
                  "
                >
                  Design, Build, and Create
                </h1>
              </div>
              <p class="text-xl text-blue-300">
                Handcrafted templates and components to help you design, build,
                and create easier than ever before.
              </p>
              <a
                href="#_"
                class="
                  inline-block
                  px-6
                  py-3
                  text-base
                  font-medium
                  tracking-wide
                  text-center text-blue-500
                  transition
                  duration-200
                  bg-white
                  rounded-lg
                  hover:bg-red-100
                  ease
                "
                >Learn More</a
              >
            </div>
          </div>
        </div>

        <div class="relative z-10 w-full max-w-2xl mt-20 lg:mt-0 lg:w-5/12">
          <div
            class="
              flex flex-col
              items-start
              justify-start
              p-10
              shadow-2xl
              rounded-xl
            "
          >
          <!-- <img src="~/assets/glider.png"> -->
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.h11 {
  background-image: url("~/assets/doctors3.jpg");
}
</style>