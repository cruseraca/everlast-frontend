<template>
  <div>
    <Home />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import Home from "~/pages/home.vue";

export default Vue.extend({
  components: { Home },
  name: "IndexPage",
});
</script>
