<script setup>
const props = defineProps({
   comment:{
      type: String,
      default: "",
  },
    username:{
     type: String,
      default: "",
  },
  userprog:{
     type: String,
      default: "",
  },
  images:{
      type: String,
      default:"",
    },
 

});
</script>

<template>
  <div class="container__comment">
    <h3 class="container__comment-text-1">{{ comment }}</h3>

    <img :src="images" alt="" />
    <p class="container__comment-text-2">
      {{ username }}<br/><span>{{userprog}}</span>
    </p>
  </div>
</template>
