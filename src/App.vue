<template>
  <Navbar :logo="logo_src" :alt="alt_name" />
  <router-view/>
  <Footer />
</template>

<script>
  import Navbar from "./components/Navbar.vue";
  import Footer from "./components/Footer.vue";
  
  export default{
    components:{
      Navbar,
      Footer
    },
    data(){
      return{
          alt_name: "Fare la pizza",
         logo_src: "/img/logo.png",
         app_name: "Faça sua pizza"
      }
    }
  }

</script>


<style>
*{
  font-family: Helvetica;
  padding: 0px;
  margin: 0px;
  box-sizing: border-box;
}

.main-container{
  margin: 50px;
  min-height: 250px;
}

h1{
  text-align: center;
  font-size: 42px;
  margin-bottom: 30px;
  color: #222;
}
</style>
