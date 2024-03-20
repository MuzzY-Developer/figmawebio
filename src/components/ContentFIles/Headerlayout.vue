<script setup>
import Navbar from "@/components/UI/Navbar.vue";
import SliderItem1 from "@/components/UI/Slider-Item1.vue";
</script>

<template>
    <div class="header">
        <div class="header__container">
            <Navbar/>
            <img class="header__container-bg" src="@/assets/images/logophoto.png" alt="">
            <article class="header__container-article-1">
            <p class="header__container-article-1-text-1">A place where</p>
            <p class="header__container-article-1-text-2">A creative agency for redemptive brands</p>
            <p class="header__container-article-1-text-3">Anteelo is a leading strategic design firm that builds powerful digital solutions for startups and enterprises.</p>
            <p class="header__container-article-1-text-4"><a href=""> Get in touch</a></p>
            </article>
            <SliderItem1/>
        </div>
    </div>

</template>
