<script setup>
import Header from "./components/ContentFIles/Headerlayout.vue";
import Main from "./components/ContentFIles/Mainlayout.vue";
import Footer from "./components/ContentFIles/Footerlayout.vue";
</script>

<template>
  <div class="wrapper">
    <Header/>
    <Main/>
    <Footer/>
  </div>
</template>
<style>
.wrapper{
  max-width: 1440px;
  margin:0 auto;
  width: 100%;
}</style>