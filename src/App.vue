<script setup lang="ts">
</script>

<template>
  <div class="heart" />
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
.heart {
  position: relative;
  width: 100px;
  margin: 0 auto;
  height: 100px;
  background-color: pink;
  transform: rotate(-45deg);
}
.heart::after {
  content: '';
  position: absolute;
  border-radius: 50%;
  background-color: pink;
  position: absolute;
  width: 100px;
  height: 100px;
  top: 0px;
  left: 50px;
}
.heart:before {
  background-color: pink;
  content: "";
  border-radius: 50%;
  position: absolute;
  width: 100px;
  height: 100px;
  top: -50px;
  left: 0px;
}
</style>
