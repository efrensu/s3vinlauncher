<script setup>
import Navbar from './components/Navbar.vue';
import Applauncher from './components/Applauncher.vue';
import Workapps from './components/Workapps.vue';
import Pagenav from './components/Pagenav.vue';

</script>

<template>
    <Navbar/>
    <Applauncher/>
    <Workapps/>
    <Pagenav/>
</template>

<style>

#app{
  min-height: 100vh;
  position: fixed;
}

body{
  background-color: white;
}



</style>
