<template>
    <div>

      <nav>
            <ul ref="nav">
             

                  <img src="../assets/LOGO1.jpg" alt="" @click="toggleNav" >

           
           
            <li>
                <router-link to="/home">Home</router-link>
                <router-link to="/contact">Contact</router-link>
                <router-link to="/about">About</router-link>
            </li>
            </ul>
        </nav>
    </div>
</template>

<script>
    export default {
        methods: {
            toggleNav () {
                const nav = this.$refs.nav.classList
                nav.contains('active') ? nav.remove('active') : nav.add('active')
            }
        }

    }
</script>

<style scoped>

nav {
    
    justify-content: space-between;
    background: black;
    align-content: center;
    height: 100px;
   
  

}
nav ul{
    
    display: flex;
    justify-content: space-between;
    list-style: none;
    margin-right: 20px;
    height: 100%;
   
}
ul li{
    margin-top: 35px;
    

}
nav ul li a{
    margin-right: 10px;
    align-items: center;
    margin-bottom: 10px;
    
    
}
nav a{
    color: aqua;
    text-decoration: none;
   
    
    
    
}

#bars{
    color: antiquewhite;
    margin-top: 20px;
    font-size: 40px;
}
a:hover{
    
    background: white;
}

img{
    height: 40px;
    width: 200px;
    
}
i{
    color: white;
    font-size: 100px;
}

@media screen and (max-width: 970px){
    nav{
       position: absolute;
       height: 300px;
       width: 200px;
        
    }
    nav ul{
       flex-direction: column;
       
       
      
    }
    li a{
        display: flex;
        
        
    }

    ul li{
        margin-bottom: 35px;
        border-bottom: solid white;
        
    }
    
   
  img{
      height: 60px;
      width: 80px;
      border-bottom: solid white;
  } 
  i{
      font-size: 150px;
      color: white;
  }
}

</style>