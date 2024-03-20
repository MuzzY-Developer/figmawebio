<script >
export default {
    data(){
        return{
            modal:false,
        }
    }
}

</script>

<template>
     <nav class="navbar">
       <div class="navbar__logo">
        <img  src="@/assets/images/Logo.svg" alt="">
        <img  class="fiks" src="@/assets/images/webovio.png" alt="">
       
       </div>
       <div class="navbar__burger">
        <img @click="modal = !modal" src="@/assets/images/NavBurger.svg" :class="{'df' : modal}" alt="">
        <div :class="{ 'activemodal': modal }" class="navbar__burger-modal">
        <button class="navbar__burger-modal-btn" @click ="modal = false" >X</button>
           <ul class="navbar__burger-modal-ul">
            <li :class="{ 'activemodaltext': modal }" class="li">Stratedy</li>
            <li :class="{ 'activemodaltext': modal }" class="li">Desinger</li>
            <li :class="{ 'activemodaltext': modal }" class="li">Books</li>
            <li :class="{ 'activemodaltext': modal }" class="li">Webserver</li>
            <li :class="{ 'activemodaltext': modal }" class="li">Digital book</li>
           </ul>

        </div>
       </div>
      
     </nav>
</template>
