<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import HelloWorld from './components/HelloWorld.vue'
// import { faDiscord } from '@fortawesome/free-brands-svg-icons'


</script>

<template>
  <!-- these will work -->
  <font-awesome-icon icon="user-secret" size="5x"/>
  <font-awesome-icon :icon="['fab', 'discord']" size="5x" color="purple" />

  <!-- will work if you import the icon above -->
  <font-awesome-icon :icon="faDiscord" size="5x" color="orange" />

  <!-- these will NOT work -->
  <font-awesome-icon icon="discord" size="5x" color="red" />
  <font-awesome-icon :icon="discord" size="5x" color="green" />
  <font-awesome-icon icon="faDiscord" size="5x" color="aqua" />
  <font-awesome-icon icon="fab fa-discord" size="5x" color="blue" />

  <HelloWorld msg="Hello Vue 3 + Vite" />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
