<template>
    <Banner />
    <div class="main-container">
    <H1>Faça seu pedido:</H1>
    <BurguerForm />
  </div>
</template>

<script lang="ts">
  import Banner from '../components/banner.vue'
  import BurguerForm from '../components/burgerForm.vue'
  export default{
    name: "Home",
    components: { 
      Banner,
      BurguerForm
    }
  }
</script>
