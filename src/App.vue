<template>
  <div id="app">
    <home></home>
  </div>
</template>

<script>
import home from './views/Home.vue'

export default {
  name: 'App',
  components: {
    home
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Gothic+A1:wght@300;400;500;600;700;800;900&display=swap');
:root{
  --bg-opacity: 1;
}
*{
  margin: 0;
  padding: 0;
}
html {
    scroll-behavior: smooth;
}
body{
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
/* SCROLL BAR */
.section-header{
  display: none;
}
/* width */
::-webkit-scrollbar {
  width: 10px;
}

/* Track */
::-webkit-scrollbar-track {
  background: #f1f1f1;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #888;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #555;
}
@media (max-width:991.98px) {
  .section-header{
    padding: 24px 0px;
    display: block;
    font-size: 12px;
    text-transform: uppercase;
    letter-spacing: 3px;
    z-index: 999999;
  }
}
</style>
