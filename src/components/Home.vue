<template>
  <div class="home">
    <header>
      <h1>Cordel Moderno</h1><br>
      <!-- Obrigatório dar o crédito ao autor para poder usar o seu poema -->
      <p>Por <a href="https://www.recantodasletras.com.br/poesias/3186743" target="_blanck">Milton Duarte</a></p><br>
    </header>
    
    <section class="normal">
      <p>
        Estou ficando cansado <br>
        Da tal tecnologia<br>
        Só se fala por e-mail<br>
        Mensagem curta e fria<br>
        Twitter e Facebook<br>
        Antes que eu caduque<br>
        Vou dizer tudo em poesia.
      </p>
    </section>

   
    <section class="imagem" id="img1">
      <p>
        Não é mais como era antes<br>
        É tudo abreviado<br>
        "Você" só tem duas letras<br>
        O "O" e o "E" foi riscado<br>
        Para declarar o amor<br>
        Basta botar uma flor<br>
        E um coração desenhado.
      </p>
    </section>

   
    <section class="normal">
      <p>
        Arroba agora não pesa<br>
        É parte de um endereço<br>
        Ponto final nem se usa<br>
        Ou vai até no começo<br>
        Agora é .com<br>
        Se o saite é muito bom<br>
        Ele vale um alto preço.<br>
      </p>

      <p>
        Pra piorar a liguagem<br>
        O emoticom é um risco<br>
        Tem símbolo para tudo<br>
        Ponto e vírgula e um asterisco<br>
        Um beijo significa<br>
        Pra entender como fica<br>
        Decifre esse rabisco.
      </p>
    </section>

   
    <section class="imagem" id="img2">
      <p>
        Tenho saudade das cartas<br>
        Escritas com a própria mão<br>
        Mandava no mês de Junho<br>
        Só chegava no Verão<br>
        Mas matava a saudade<br>
        Era texto de verdade<br>
        Nas linhas do coração.
      </p>
    </section>

   
    <section class="normal">
      <p>
        Agora, escrevo e envio<br>
        Chegando na mesma hora<br>
        Mas quando vou prosear<br>
        A pessoa foi embora<br>
        Abriu outro aplicativo<br>
        O mundo ficou cativo<br>
        Da tecnologia do agora.<br>
      </p>

      <p>
        Felizmente, pra orar<br>
        Não precisa de internet<br>
        Deus escuta todo mundo<br>
        Se quiser, faça esse teste<br>
        Dois pontos são dois joelhos<br>
        Seus lábios são aparelhos<br>
        Deixe que Deus interprete.
      </p>
    </section>

   
  </div>
</template>

<script>

export default {
  name: "Home",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .home{
    min-height: 100vh;
    background-color: darkgray;
    font-family: var(--fonte1);
  }

  header{
    background-color: black;
    color: white;
    text-align: center;
  }

  header h1{
    padding-top: 50px;
    text-transform: uppercase; /*  deixar toda letra em maiuscula */
    font-family: var(--fonte2);
    font-size: 4vw; /* com vh vai ajustar o tamanho do texto de acordo com a tela na horizontal */
  }

  header p{
    padding-bottom: 50px;    
  }

  a{
    color:  white;
    text-decoration: none;
    font-weight: bolder;
  }

  a:hover{
    text-decoration:  underline;
  }

  .normal{
    background-color: white;
    color: black;
  }

  .imagem{
    background-color: rgb(51, 51, 51);
    color: white;
    box-shadow: inset 6px 6px 13px 0 rgba(0, 0, 0, 0.468); /* coloquei sombra interna na div */
  }

  .imagem p{ /* criando um fundo quadrado para uma melhor leitura */
    display: inline-block; /* vai ajustar o quadrado de acordo com o tamanho dos textos */
    padding: 10px;
    background-color: rgba(0, 0, 0, 0.447);
    text-shadow: 1px 1px 0px black;
  }

  section{
    padding-top: 5vh;
    padding-bottom: 5vh;
    line-height: 2em; /* aumentando o espaçamento das letras na vertical */
    padding-left: 30px;
    font-family: var(--fonte3);
    font-size: 2vw; /* com vh vai ajustar o tamanho do texto de acordo com a tela na horizontal */
  }

  section p{
    padding-bottom: 2em;
  }

  #img1{
    background-image: url("../publico/imagens/background001.jpg");
    background-position: right center; /* alterando o ponto de ancoragem de inicio da imagem */
    background-size: cover; /* enquadrando o tamanho da imagem dentro da div */
    background-attachment: fixed; /* deixei a imagem fixa para ter o efeito parallax */
  }

  #img2{
    background-image: url("../publico/imagens/background002.jpg");
    background-position: right center;
    background-size: cover;
    background-attachment: fixed; /* deixei a imagem fixa para ter o efeito parallax */
  }
</style>
