<template>
  <div class="container mt-3">
    <div class="row my-3">
      <div v-for="item in items" v-bind:key="item.date" class="col-md-6">
        <article class="card mb-2 my-3" style="max-width: 40rem;">
          <img :src="item.img_src" :alt="item.title" class="card-img-top" />
          <div class="card-body">
            <h3 class="card-title">{{ item.title }}</h3>
            <p class="card-text">{{ item.text }}</p>
            <a
              role="button"
              tabindex="0"
              target="_self"
              :href="item.href"
              class="btn mx-1 btn-primary"
              >GitHub Page</a
            >
            <span
              v-for="badge in item.badges"
              :key="badge.index"
              class="badge mx-1 badge-info"
            >
              {{ badge.text }}
            </span>
            <span class="badge ml-2 badge-secondary"> {{ item.date }} </span>
          </div>
        </article>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Portfolio",
  data() {
    return {
      items: [
        {
          title: "Portfolio Site",
          text: "当サイト",
          img_src: require("@/assets/Portfolio.png"),
          href: "https://github.com/m4oyu/portfolio",
          badges: [
            { text: "Vue.js" },
            { text: "Bootstrap" },
            { text: "GitHub Pages" },
          ],
          date: "2020.3",
        },
        {
          title: "Address List Application",
          text: "Udemy教材 成果物",
          img_src: require("@/assets/AddressList.png"),
          href: "https://github.com/m4oyu/vue_firebase_todo",
          badges: [{ text: "Vue.js" }, { text: "firebase" }],
          date: "2020.2",
        },
        {
          title: "迷路ゲーム",
          text: "大学のプログラミング講義 成果物",
          img_src: require("@/assets/MapGame.png"),
          href: "https://github.com/m4oyu/EscapeFromShizuokaUniv",
          badges: [{ text: "Java" }, { text: "JavaFx" }],
          date: "2020.1",
        },
        {
          title: "Tetoris",
          text: "株式会社エムティーアイ インターンシップ事前課題",
          img_src: require("@/assets/tetoris.png"),
          href: "https://github.com/m4oyu/class_java/tree/master/tetoris",
          badges: [{ text: "HTML" }, { text: "CSS" }, { text: "JS" }],
          date: "2019.7",
        },
      ],
    };
  },
};
</script>
