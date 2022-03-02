<template>
  <div id="app"  >


    <Navbar/>

    <router-view/>
  </div>
</template>




<script>
import Navbar from "./components/Navbar.vue"
     export default{
       components:{ Navbar
       }
     }
  
</script>

<style  scoped>
 #app{
   
   background:rgb(4, 4, 65);
   margin: -25px;
   height: 100%; 
   width: 100%;
  

 }

 

 


 

</style>

