<template>
  <div
    class="sticky top-0 z-50 h-24 border-b border-gray-200 select-none md:overflow-visible bg-white "
  >
    <div
      class="container sticky flex flex-wrap border-b border-gray-200 items-center justify-between h-24 mx-auto overflow-hidden font-medium lg:justify-center sm:px-4 md:px-2"
    >
      <div class="flex items-center justify-start w-1/4 h-full pr-4">
        <a href="#_" class="inline-block py-4 md:py-0">
          <span class="p-1 text-xl font-black leading-none text-gray-900"
            ><span
              >everlast<span class="text-green-600">.link</span></span
            ></span
          >
        </a>
      </div>
      <div
        class="flex top-0 left-0 items-start w-full h-full p-4 text-sm bg-gray-900 bg-opacity-50 md:items-center md:w-3/4 md:absolute lg:text-base md:bg-white md:p-0 md:relative md:flex"
        v-bind:class="{ 'flex fixed': showMenu, hidden: !showMenu }"
      >
        <div
          class="flex-col w-full h-auto overflow-hidden bg-white rounded-lg md:bg-transparent md:overflow-visible md:rounded-none md:relative md:flex md:flex-row"
        >
          <a
            href="#_"
            class="inline-flex items-center block w-auto h-16 px-6 text-xl font-black leading-none text-gray-900 md:hidden"
            ><span class="p-1 text-xl font-black leading-none text-gray-900"
            ><span
              >everlast<span class="text-green-600">.link</span></span
            ></span
          ></a
          >
          <div
            class="flex flex-col items-start justify-center lg:w-full space-x-6 text-center lg:space-x-8 md:w-2/3 md:mt-0 md:flex-row md:items-center"
          >
            <a
              href="#_"
              class="inline-block w-full py-2 mx-0 ml-6 font-medium text-left text-gray-700 md:w-auto md:px-0 md:mx-2 hover:text-green-600 lg:mx-3 md:text-center"
              >Fitur</a
            >
            <a
              href="#_"
              class="inline-block w-full py-2 mx-0 font-medium text-left text-gray-700 md:w-auto md:px-0 md:mx-2 hover:text-green-600 lg:mx-3 md:text-center"
              >Tutorial</a
            >
            <a
              href="#_"
              class="inline-block w-full py-2 mx-0 font-medium text-left text-gray-700 md:w-auto md:px-0 md:mx-2 hover:text-green-600 lg:mx-3 md:text-center"
              >Harga</a
            >
            <a
              href="#_"
              class="inline-block w-full py-2 mx-0 font-medium text-left text-gray-700 md:w-auto md:px-0 md:mx-2 hover:text-green-600 lg:mx-3 md:text-center"
              >Kontak</a
            >
          </div>
          <div
            class="flex flex-row items-start justify-end pt-4 md:items-center md:w-1/3 md:py-0"
          >
            <a
              href="#"
              class="w-full px-6 py-2 mr-0 text-gray-700 md:px-0 lg:pl-2 md:mr-4 lg:mr-5 md:w-auto"
              >Masuk</a
            >
            <a
              href="#_"
              class="inline-flex items-center w-full px-6 py-3 text-sm font-medium leading-4 text-white bg-green-600 md:px-3 md:w-auto lg:px-5 hover:bg-green-500 focus:outline-none md:focus:ring-2 focus:ring-0 focus:ring-offset-2 focus:ring-green-600 lg:rounded-xl"
              >Buat Sekarang!</a
            >
          </div>
        </div>
      </div>
      <div
        v-on:click="showNavbar()"
        class="absolute right-0 flex flex-col items-center items-end justify-center w-10 h-10 bg-white rounded-full cursor-pointer md:hidden hover:bg-gray-100"
      >
        <svg
          class="w-6 h-6 text-gray-700"
          v-show="!showMenu"
          fill="none"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path d="M4 6h16M4 12h16M4 18h16"></path>
        </svg>
        <svg
          class="w-6 h-6 text-gray-700"
          v-show="showMenu"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
          style="display: none"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M6 18L18 6M6 6l12 12"
          ></path>
        </svg>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data: function () {
    return { showMenu: false };
  },
  methods: {
    showNavbar: function () {
      this.showMenu = !this.showMenu;
    },
  },
};
</script>

<style lang="scss" scoped></style>
