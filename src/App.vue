<template>
  <div class="organizaFooter">
    <Home />
    <Footer />
  </div>
</template>

<script>
import Home from './components/Home.vue';
import Footer from "./components/Footer.vue";

export default {
  name: 'App',

  components: {
    Home,
    Footer
  }
}
</script>

<style>
  /* ESTOU REMOVENDO AS MARGENS LATERAIS DA PAGINA QUE VEM POR PADRÃO */
  *{
    padding: 0;
    margin: 0;
  }
  
  /* USANDO AS FONTES QUE IMPORTEI DO GOOGLE FONTS, COLOQUEI O LINK DELAS NO INDEX.HTML */
  :root{ 
    --fonte1: Verdana, Geneva, Tahoma, sans-serif;
    --fonte2: 'Passion One', cursive;
    --fonte3: 'Sriracha', cursive;
  }

  /* VAI MANTER O FOOTER SEMPRE AO FINAL DA PAGINA, MESMO SE O CONTEÚDO FOR PEQUENO */
  .organizaFooter{
    display: flex;
    flex-direction: column;
    min-height: 100vh;
  }
</style>
