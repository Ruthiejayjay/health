<template>
  <div class="bg-gradient-to-r from-pink-500 to-purple-500">
    <nav
      x-data="{ mobile: false }"
      class="
        relative
        z-40
        py-10
        pt-6
        mx-auto
        md:pb-6
        max-w-7xl
        md:flex md:justify-between md:items-center
        w-full
      "
    >
      <div class="relative z-20 flex items-center justify-between">
        <div>
          <a href="/" class="md:text-xl">
            <img src="~/assets/logo.png" style="width: 70px; height: 50px" />
          </a>
        </div>

        <!-- Mobile menu button -->
        <div x-on:click="mobile = !mobile" class="flex md:hidden">
          <button
            type="button"
            class="
              text-gray-200
              hover:text-gray-100
              focus:outline-none focus:text-gray-100
            "
            aria-label="toggle menu"
          >
            <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
              <path
                fill-rule="evenodd"
                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
              ></path>
            </svg>
          </button>
        </div>
      </div>

      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <div
        x-bind:class="{ hidden: !mobile, flex: mobile }"
        class="
          left-0
          z-10
          items-center
          justify-center
          w-full
          font-semibold
          select-none
          md:flex
          lg:absolute
        "
      >
        <div
          class="
            flex flex-col
            justify-center
            w-full
            mt-4
            space-y-2
            md:mt-0 md:flex-row md:space-x-6
            lg:space-x-10
            xl:space-x-16
            md:space-y-0
          "
        >
          <div
            x-data="{ isOpen: false }"
            x-on:mouseenter="isOpen = true"
            x-on:mouseleave="isOpen = false"
            class="relative py-3"
          >
            <NuxtLink
              to="/medical"
              class="py-3 text-gray-300 hover:text-gray-100 hover:underline"
              >Medical Surgical</NuxtLink
            >
          </div>
          <NuxtLink
            to="/monitoring"
            class="py-3 text-gray-300 hover:text-gray-100 hover:underline"
            >Monitoring</NuxtLink
          >
          <NuxtLink
            to="/ultrasound"
            class="py-3 text-gray-300 hover:text-gray-100 hover:underline"
            >Ultrasound</NuxtLink
          >
          <NuxtLink
            to="/oncology"
            class="py-3 text-gray-300 hover:text-gray-100 hover:underline"
            >Oncolgy</NuxtLink
          >
        </div>
      </div>

      <div
        x-bind:class="{ flex: mobile, 'hidden md:flex': !mobile }"
        class="
          relative
          z-20
          flex-col
          justify-center
          pr-5
          mt-4
          space-y-8
          md:pr-3
          lg:pr-0
          md:flex-row md:space-y-0 md:items-center md:space-x-6 md:mt-0
        "
      ></div>
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style>
</style>