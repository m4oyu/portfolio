<template>
<div class="container">
    <div class="container col-md-6">
        <h1 class="mt-5 mb-3">Get in Touch</h1>
        <hr class="mb-4" color="007bff" id="bar">
        <input type="text" class="form-control my-3" placeholder="name">
        <input type="text" class="form-control my-3" placeholder="name@example.com">
        <input type="text" class="form-control my-3" placeholder="phone number">
        <textarea class="form-control my-3" rows="3" placeholder="text something"></textarea>
        <b-button class="mt-3 mb-5 px-4 btn-lg align-self-end" variant="primary">Send</b-button>
    </div>
</div>
</template>

<style lang="scss">
#bar {
    width: 400px;
    height: 3px;
}
.container {
    margin-right: auto;
    margin-left: auto;
}
</style>