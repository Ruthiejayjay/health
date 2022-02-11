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
        opacity-40
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
                <h4
                  class="
                    text-sm
                    font-medium
                    leading-tight
                    text-left
                    text-gray-100
                    sm:text-xl
                    md:text-2xl
                  "
                >
                  The Rules Have Changed
                </h4>
              </div>
              <h2 class="text-4xl font-bold text-white text-left">See Lastest PM Guidelines.</h2>
              <a
                href="#_"
                class="
                  inline-block
                  px-8
                  py-4
                  text-xl
                  font-medium
                  tracking-wide
                  text-center text-white
                  transition
                  duration-200
                  border border-pink-700
                  rounded-lg
                  hover:bg-pink-300
                  ease
                  uppercase
                "
                >Learn More now</a
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
              shadow-xl
              rounded-xl
            "
          ></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
.h11 {
  background-image: url("~/assets/o.jpg");
}
</style>