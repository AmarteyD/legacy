<template>
  <div >
     <div>
    <img alt="student with backpack" src="../assets/hero.png">
    </div>
    <h2>HOME IS HERE ALREADY</h2>
    <div>
     <footer>
      <p>  &#169;2022 Legacy Inc</p>
      

       <router-link to="/about">About</router-link>
       <router-link to="contact">Contact Us</router-link>
       <br>
      <a href="https://api.whatsapp.com/send?phone=233541714435" >
                        <i id="wsp" class="fab fa-whatsapp"> </i> 
       </a>
       <a id="fb" href="https://web.facebook.com/profile.php?id=100069469736791">
                        <i class="fab fa-facebook-square"></i>
                    </a>
      
              
     </footer>
   </div>
  </div>
</template>

<script>


export default {
 
  components: {
   
  }
}
</script>
<style >


img{
  height: 400px;
  width: 800px;
  padding-top: 20px;
  box-shadow: 10px solid green;
}

footer{
  background: black;
  text-align: center;
}
#wsp{
  color: green;
  font-size: 30px;
}
</style>

