<template>
  <Navbar :logo="logo_src" :alt="app_name" />
  <router-view/>
    <Footer />
</template>


<script>
import Navbar from './components/navbar.vue';
import Footer from './components/footer.vue';

export default {
  components: {
    Navbar,
    Footer
  },
  data(){
    return {
      logo_src: "/img/logo.png",
      app_name: "Make Your Burguer"
    }
  }
}
</script>


<style>
@import url('https://fonts.googleapis.com/css2?family=Anek+Malayalam:wght@300&family=Lato:ital,wght@0,300;0,400;1,400&display=swap');

* {
    padding: 0;
    margin: 0;
    font-family: 'Anek Malayalam', sans-serif;
    font-family: 'Lato', sans-serif;
    box-sizing: border-box;
}
h1{
    text-align: center;
}
.main-container{
  margin: 50px;
  min-height: 250px;
}
</style>
