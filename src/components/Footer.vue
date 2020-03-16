<template>
<div class="bg-secondary text-white py-5">
    <button @click="$router.push({ name: 'Home'  })" type="button" class="btn btn-outline-light btn-lg mt-4 mb-2">Back to Home</button>
    <hr color="007bff" id="bar">
    <span style="3em">
        <a class="icon" href="#"><font-awesome-icon :icon="['fab', 'twitter']"  class="fa-3x px-2" /></a>
        <a class="icon" href="#"><font-awesome-icon :icon="['fab', 'github']" class="fa-3x px-2" /></a>
        <a class="icon" href="#"><font-awesome-icon icon="envelope" class="fa-3x px-2" /></a>
    </span>
    <p class="pb-4">© 2020 · All Rights Reserved</p>
</div>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="scss">
#bar {
    width: 200px;
    height: 2px;
}
.icon {
    color: white;
}
</style>