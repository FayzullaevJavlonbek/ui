<script>
import Navbar from './components/Navbar.vue';
export default {
  name: 'app',
  components: {
    Navbar
  }
}
</script>

<template>
  <div id="app">
    <header>
      <Navbar /> 
    </header>

  </div>
</template>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body{
  font-family: 'montserrat', sans-serif;
}
header{
  width: 100wh;
  background-color:rgb(29, 32, 54);
  padding: 15px;
}
</style>
