<template>
  <div id="app">
    <helloworld></helloworld>
  </div>
</template>

<script>
import helloworld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    helloworld
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Gothic+A1:wght@300;400;500;600;700;800;900&display=swap');

*{
  margin: 0;
  padding: 0;
}
html {
    scroll-behavior: smooth;
}
body{
  --bg-opacity: 1;
  font-size: 14px;
  box-sizing: border-box;
  font-family: 'Gothic A1', sans-serif;
  background-color: rgba(21,21,21,var(--bg-opacity));
  color: white;
  height: 100vh;
  scroll-behavior: smooth;
  width: 100%;
  position: relative;
}
a{
  color: white;
  text-decoration: none;
}
</style>
