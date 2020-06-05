import Vue from 'vue';
import NavbarCo from './components/Navbar.vue'

<template>
  <div>
    <NavbarCo />
    <router-view />
  </div>
</template>

<script>
import NavbarCo from "./components/NavbarCo.vue"; // eslint-disable-line

export default {
  name: "App", // eslint-disable-line
  components: {
    NavbarCo
  }
}; // eslint-disable-line
</script>
