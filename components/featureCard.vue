<template>
  <div class="xl:w-1/3 md:w-1/2 p-4">
    <div class="flex flex-col items-center border border-gray-200 p-6 rounded-xl bg-white">
      <div
        class="w-10 h-10 inline-flex items-center justify-center rounded-full bg-green-100 text-green-500"
      >
        <svg
          fill="none"
          stroke="currentColor"
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="2"
          class="w-6 h-6"
          viewBox="0 0 24 24"
        >
          <path d="M22 12h-4l-3 9L9 3l-3 9H2"></path>
        </svg>
      </div>
      <h2 class="text-lg text-gray-900 font-medium title-font my-2">
        {{title}}
      </h2>
      <p class="leading-relaxed text-base text-center">
        Fingerstache flexitarian street art 8-bit waist co, subway tile poke
        farm.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  props: ['featureTitle'],
  data: function () {
    return {
      title: this.featureTitle
    }
  }
}
</script>

<style lang="scss" scoped></style>
