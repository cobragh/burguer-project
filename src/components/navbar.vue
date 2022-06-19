<template>
    <div class="nav">
        <router-link to="/" id="logo_url">
            <img :src="logo" :alt="alt" id="logo">
        </router-link>
        <router-link to="/">Home</router-link>
        <router-link to="/pedidos">Pedidos</router-link>
    </div>
</template>
 
<script>
export default {
    name: "Navbar",
    props: ["logo", "alt"]
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Anek+Malayalam:wght@300&family=Lato:ital,wght@0,300;0,400;1,400&display=swap');

    .nav{
        background-color: #222;
        border-bottom: 4px solid #111;
        padding: 15px 50px;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }
    #logo_url{
        margin: auto;
        margin-left: 0;
    }
    #logo{
        width: 40px;
        height: 40px;
    }
     .nav a{
        color: #FBCA03;
        text-decoration: none;
        margin: 12px;
        transition: 0.9;
     }
     .nav a:hover{
        color: #fff;
     }
     
</style>