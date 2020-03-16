<template>
  <div class="sticky-top">
    
    <b-navbar toggleable="md" type="dark" variant="dark">
    <b-navbar-toggle target="nav-text-collapse"></b-navbar-toggle>

    <b-navbar-brand class="py-4 pl-5 pr-2" @click="$router.push({ name: 'Home' })">Yuki Yamamoto</b-navbar-brand>

    <b-collapse id="nav-text-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-text>Front-end Engineer</b-nav-text>
      </b-navbar-nav>
      <!--右側の要素-->
      <b-navbar-nav class="ml-auto">
        <b-nav-item @click="$router.push({ name: 'Home'  })">Home</b-nav-item>
        <b-nav-item @click="$router.push({ name: 'About' })">About</b-nav-item>
        <b-nav-item @click="$router.push({ name: 'Portfolio' })">Portfolio</b-nav-item>
        <b-nav-item @click="$router.push({ name: 'Contact' })">Contact</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>