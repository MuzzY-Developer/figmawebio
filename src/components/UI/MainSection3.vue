<script setup>
import SliderItem2 from "./Slider-item2.vue";
 const productCard =[
         { 
            id:1,
            name:"Product Design",
            comp:"Sprint",
            title:"A five-day workshop that will help you answer crucial business questions",
            links:"Read More"
         },
         { 
            id:2,
            name:"Scoping",
            comp:"Session",
            title:"A workshop aimed at shaping your business idea, answering questions regarding project planning",
            links:"Read More"
         },
         { 
            id:3,
            name:"UX",
            comp:"Review",
            title:"An evaluation which will help you radically improve your product.",
            links:"Read More",
            wd: "55px"
         },
         { 
            id:4,
            name:"Code",
            comp:"Review",
            title:"Do you know what one of the key secrets of success is what makes people successful in business",
            links:"Read More"
         }




 ]

</script>

<template>
   <div class="main__section-3">
      <h3 class="main__section-3-text">Deation & Evaluation - Best Way to Kick off Your Product Idea</h3>
     <div class="main__section-3-card">
        <div v-for="(item) in productCard" :key="item"   class="main__section-3-card-item">
          <h3 class="main__section-3-card-item-text-1">{{item.name}}<br><span>{{item.comp}}</span> </h3>
          <p class="main__section-3-card-item-text-2">{{ item.title}}</p>
          <p class="main__section-3-card-item-text-3"><a href="">{{ item.links }}</a></p>
        </div>
        <SliderItem2 />
     </div>


   </div>
</template>

<style>


</style>