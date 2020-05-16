<template>
  <div class="sticky-top">
    <b-navbar toggleable="md" type="dark" variant="dark">
      <b-navbar-toggle target="nav-text-collapse"></b-navbar-toggle>

      <b-navbar-brand class="py-4 pl-5 pr-2">Maoyu</b-navbar-brand>

      <b-collapse id="nav-text-collapse" is-nav>
        <!--右側の要素-->
        <b-navbar-nav class="ml-auto">
          <b-nav-item @click="onClickTop">Home</b-nav-item>
          <b-nav-item @click="onClickWork">Works</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "Header",
  methods: {
    onClickTop: function() {
      const hash = "#app";
      if (hash && hash.match(/^#.+$/)) {
        this.$scrollTo(hash);
      }
    },
    onClickWork: function() {
      const hash = "#works";
      if (hash && hash.match(/^#.+$/)) {
        this.$scrollTo(hash);
      }
    },
  },
};
</script>
