<script setup>
import HeaderCompVue from "@/components/template/HeaderComp.vue";
import RodapeCompVue from "./components/template/RodapeComp.vue";
</script>

<template>
  <HeaderCompVue />
  <main>
    <RouterView />
  </main>
  <RodapeCompVue />
</template>

<style>
@import "@/assets/base.css";
@import "@/assets/style.css";

#app {
  max-width: 1280px;
  margin: 0 auto;
  font-weight: normal;
  height: 100vh;
}
header {
  background-color: black;
  color: rgb(255, 255, 255);
  height: 15%;
  font-size: 1.3em;
  display: flex;
  align-items: center;
  padding-left: 2rem;
}
main {
  height: 70%;
}
a {
  color: inherit;
  text-decoration: none;
}
</style>
