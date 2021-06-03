<template>
  <div class="row py-2 border-bottom bg-info text-white px-5">
    <div class="col-6 d-flex align-items-center">
      <img
        src="./assets/slaycer.webp"
        width="70"
        height="70"
        class="rounded-circle"
      />
      <h1 class="title fs-1 mx-2" id="nome">{{ botName }}</h1>
    </div>
    <div class="col-6 d-flex align-items-center justify-content-end">
      <div id="nav" class="fs-3 btn-group" role="group">
        <router-link class="btn btn-outline-primary " to="/">Homepage</router-link>
        <router-link class="btn btn-outline-primary " to="/about">Sobre</router-link>
      </div>
    </div>
  </div>
  <router-view />
</template>

<script>

export default {
  data() {
    return {
      botName: "Slaycer"
    }
  }
}
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Lobster&display=swap");
.title {
  font-family: "Lobster", cursive;
}
</style>
