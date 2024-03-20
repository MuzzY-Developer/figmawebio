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
        <img  src="./Logo.svg" alt="">
        <img  class="fiks" src="./webovio.png" alt="">
       
       </div>
       <div class="navbar__burger">
        <img @click="modal = !modal" src="./NavBurger.svg" :class="{'df' : modal}" alt="">
        <div :class="{ 'activemodal': modal }" class="navbar__burger-modal">
        <button class="navbar__burger-modal-btn" @click ="modal = false" >X</button>
           <ul class="navbar__burger-modal-ul">
            <li :class="{ 'activemodaltext': modal }" @click="modal = false" class="li">Stratedy</li>
            <li :class="{ 'activemodaltext': modal }" @click="modal = false" class="li">Desinger</li>
            <li :class="{ 'activemodaltext': modal }" @click="modal = false" class="li">Books</li>
            <li :class="{ 'activemodaltext': modal }" @click="modal = false" class="li">Webserver</li>
            <li :class="{ 'activemodaltext': modal }" @click="modal = false" class="li">Digital book</li>
           </ul>

        </div>
       </div>
      
     </nav>
</template>
