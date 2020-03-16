<template>
<div class="mt-2 mx-2">
  <div class="jumbotron jumbotron-fluid mb-2">
    <h1 class="display-2 mt-5">Yuki Yamamoto</h1>
    <p class="lead my-4">Front-end Engineer from Shizuoka University</p>
    <hr class="my-5" color="#007bff">
    <p>各種ご連絡はこちらから</p>
    <a @click="$router.push({ name: 'Contact'  })" class="btn btn-primary btn-lg" href="#" role="button">Get in Touch</a>
  </div>
</div>
</template>