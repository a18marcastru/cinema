<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>

    <div class="wrapper">

      <nav>
        <button class="btn btn-primary"><RouterLink id="session" to="/">Home</RouterLink></button>
        <button><RouterLink to="/about">About</RouterLink></button>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style>
@import "@/assets/base.css";
nav {
  text-align: center;
}
#session {
  margin: 5px;
}
</style>
