<script setup>
import CategoriasComp from "../components/CategoriasComp.vue";
</script>

<template>
  <div id="home">
    <div id="recomendados">
      <header>
      <h2>Recomendados</h2>
    </header>
      <div class="filmes">
        <img
          src="https://m.media-amazon.com/images/I/61EJd9oPopL.jpg"
          alt=""
          class="img"
        />
      </div>
    </div>
    <div id="categorias">
      <CategoriasComp />
    </div>
  </div>
</template>

<style scoped>
#home {
  display: grid;
  color: rgb(226, 35, 35);
  height: 100vh;
  grid-template-columns: 80% 20%;
  grid-template-areas: "recomendados categorias";
  text-align: left;
}

#recomendados {
  grid-area: recomendados;
  display: flex;
  flex-direction: column;
  height: 100vh;
  justify-content: center;
}
.filmes {
  width: 100px;
  height: 500px;
}
h2{
  color:white;
  text-align: center;
  font-size: 2em;
  height: 100px;
  width: 50px;
  padding: 10px ;

}
header{
  
}
</style>
