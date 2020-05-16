<template>
  <div class="my-3 mx-3">
    <div class="jumbotron jumbotron-fluid mb-3">
      <h1 class="display-2 mt-5">Maoyu</h1>
      <p class="lead my-4">Engineer from Nokin.</p>
      <hr class="my-5" color="#007bff" />
      <p>
        こんにちは、Maoyuです！<br />現在、地方国公立大学の2年生で情報学を学んでいます。<br />また、Nokin.という団体でプログラミングを学習しています。
      </p>
      <button
        class="btn btn-primary btn-lg mt-3"
        @click="onClick"
        role="button"
      >
        View Page
        <font-awesome-icon :icon="['fas', 'angle-down']" class="fa" />
      </button>
    </div>
    <Page id="works"></Page>
  </div>
</template>

<script>
import Page from "@/components/Page.vue";

export default {
  name: "Home",
  components: {
    Page,
  },
  methods: {
    onClick: function() {
      const hash = "#works";
      if (hash && hash.match(/^#.+$/)) {
        this.$scrollTo(hash);
      }
    },
  },
};
</script>
