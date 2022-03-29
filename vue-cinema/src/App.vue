<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>

    <div class="wrapper">

      <nav class="navbar navbar-light" style="background-color: #e3f2fd;">
        <a href="">Administrador</a>
        <RouterLink id="session" to="/">Sessiones</RouterLink>
        <RouterLink to="/about">About</RouterLink>
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
