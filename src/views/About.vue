<template>
  <div class="about">
    <h1>WHO AM I!</h1>
   <div id="conts">
     <img src="../assets/about.jpg">

     <p> I am David Amartey, a Computer Engineering student of Ghana Commmunication Technology University. <br> 
      I am  junior Frontend Web Developre of VueJs, good in html, css and bootstrap; i also use other animations to make my work standout.<br>
      also, i am Backend beginner of Python Django. my qualities includes; logo making and graphic designing and i can adapt to any evnironment<br>
      i love to learn new things to make my work perfect. THANK YOU

     </p>
   </div>
   <div>
     <footer>
      <p>  &#169;2022 Legacy Inc</p>
         <div id="nav">
       <router-link to="/home">Home</router-link>
       <router-link to="contact">Contact Us</router-link>
         </div><br>
        <div >
      <a href="https://api.whatsapp.com/send?phone=233541714435" >
                        <i id="wsp" class="fab fa-whatsapp"> </i> 
       </a>
        <a id="fb" href="https://web.facebook.com/profile.php?id=100069469736791">
                        <i class="fab fa-facebook-square"></i>
                    </a>
        </div>
      
              
     </footer>
   </div>
  </div>
</template>
<script>


export default{
  
  data: () => {
    return {
      mobileView: true

    };
  },
  methods: {
    handleView() {
        this.mobileView = window.innerWidth <= 990;
    }
  },
  components: {
  
  },
  created() {
    this.handleView();
    window.addEventListener('resize', this.handleView);
}
}
  
</script>


<style  scoped>
img{
  height: 400px;
  width: 300px;
  border-radius: 20px;
 
}
.about{
  background: rgb(4, 4, 65);
  color: white;
  text-align: center;
  font-family: Arial, Helvetica, sans-serif;
  font-style: italic;
  font-size: larger;
  margin: -20px ;
}

footer{
  background: black;
  margin-bottom: -100px;
}
#wsp{
  color: green;
  font-size: 30px;
  

}

#wsp:hover{
  display: inline-block;
  margin: 0 0.5rem;

  animation: animate__flipOutX; /* referring directly to the animation's @keyframe declaration */
  animation-duration :2s;
}



#fb{
  color: blue;
  margin-left: 10px;
  font-size: 30px;
}
#nav a{
  margin-left: 10px;
  text-decoration: none;
  color: white;
}
</style>