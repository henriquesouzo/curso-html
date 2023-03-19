<template>
    <footer>
        <p>Site criado por <a href="https://github.com/henriquesouzo" target="_blanck">Henrique Souzo</a> para estudos de VueJS 3 com HTML 5 e CSS 3</p>
    </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style scoped>
    footer{
        margin-top: auto;
        background-color: black;
        color: white;
        text-align: center;
        padding: 20px;
    }

    a{
    color:  white;
    text-decoration: none;
    font-weight: bolder;
  }

  a:hover{
    text-decoration:  underline;
  }
</style>