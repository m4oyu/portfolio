<template>
  <div>
    
    <b-navbar toggleable="md" type="dark" variant="dark">
    <b-navbar-toggle target="nav-text-collapse"></b-navbar-toggle>

    <b-navbar-brand @click="$router.push({ name: 'Home' })">Yuki Yamamoto</b-navbar-brand>

    <b-collapse id="nav-text-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-text>from SuperEvilMegacorp</b-nav-text>
      </b-navbar-nav>
      <!--右側の要素-->
      <b-navbar-nav class="ml-auto">
        <b-nav-item-dropdown text="DownBelow">
          <b-dropdown-item @click="$router.push({ name: 'Test1' })">test1</b-dropdown-item>
          <b-dropdown-item @click="$router.push({ name: 'Test2' })">test2</b-dropdown-item>
          <b-dropdown-item href="#">test3</b-dropdown-item>
          <b-dropdown-item href="#">test4</b-dropdown-item>
        </b-nav-item-dropdown>
        <b-nav-item @click="$router.push({ name: 'About' })">About</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
  </div>
</template>

<script>
export default {
  name: 'HeaderComponent'
}
</script>