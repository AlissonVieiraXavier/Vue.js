<template>
   <header>
       <h1>
           <img src="../assets/logo.png" alt="">
       </h1>
   </header>

</template>
<script ls="ts">
 
 import { defineComponent } from 'vue'
 export default defineComponent({
     name: "BarraLateral",
 })


</script>
<style scoped>
 header{
     padding:1rem;
     background: #fcc34e;
     width: 100%;
     height:100vh;
     text-align: center;
 }

 @media only screen and (max-width:768px){
    header{
     padding: 2.5rem;
     height: auto;
    }
 }


</style>