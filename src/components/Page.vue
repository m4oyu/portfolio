<template>
  <div>
    <div class="jumbotron jumbotron-fluid mb-2">
      <p class="display-4 pt-5">Works</p>
      <hr class="my-3" color="#007bff" />
      <Portfolio></Portfolio>
    </div>
  </div>
</template>

<script>
import Portfolio from "@/components/Portfolio.vue";

export default {
  name: "Page",
  components: {
    Portfolio,
  },
};
</script>

<style scoped>
hr {
  max-width: 300px;
  width: 50%;
}
</style>
