<template>
  <div>
    <LandingPage />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import LandingPage from "~/components/LandingPage.vue";

export default Vue.extend({
  components: { LandingPage },
  name: "IndexPage",
});
</script>
