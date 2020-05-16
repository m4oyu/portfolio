<template>
  <div class="bg-secondary text-white py-5">
    <button
      @click="onClickTop"
      type="button"
      class="btn btn-outline-light btn-lg mt-4 mb-2"
    >
      To PageTop
    </button>
    <hr color="007bff" id="bar" />
    <span style="3em">
      <a class="icon" href="https://twitter.com/ai_SO_late_"
        ><font-awesome-icon :icon="['fab', 'twitter']" class="fa-3x px-2"
      /></a>
      <a class="icon" href="https://github.com/m4oyu">
        <font-awesome-icon :icon="['fab', 'github']" class="fa-3x px-2" />
      </a>
      <a class="icon" href="mailto:ajidesu9015@gmail.com">
        <font-awesome-icon icon="envelope" class="fa-3x px-2" />
      </a>
    </span>
    <p class="pb-4">© m4oyu · 2020</p>
  </div>
</template>

<script>
export default {
  name: "Footer",
  methods: {
    onClickTop: function() {
      const hash = "#app";
      if (hash && hash.match(/^#.+$/)) {
        this.$scrollTo(hash);
      }
    },
  },
};
</script>

<style lang="scss">
#bar {
  max-width: 200px;
  height: 2px;
}
.icon {
  color: white;
}
</style>
