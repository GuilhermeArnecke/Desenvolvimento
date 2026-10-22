
<template>
  <div class="pagina">
    <header class="cabecalho">
      <div class="barra barra-esquerda"></div>

      <img :src="dndIcon" alt="D&D" class="icone-dnd">

      <div class="barra barra-direita"></div>
    </header>

    <main class="conteudo">
      <!-- A área de conteúdo ficará aqui -->
    </main>
  </div>
</template>

<script setup>
import dndIcon from "./assets/dndicon.png";
</script>

<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
}


.cabecalho {
  position: relative;
  height: 75px;
  width: 100%;

  background-color: #292929;
  border: 2px solid #ff3b1f;

  display: flex;
  align-items: center;
  justify-content: center;
}

.icone-dnd {
  height: 50px;
  width: 50px;
  object-fit: contain;
  z-index: 1;
}

.barra {
  position: absolute;
  top: 0;
  bottom: 0;

  width: 3px;
  background-color: #ff3b1f;

  box-shadow:
    0 0 5px #ff3b1f,
    0 0 10px #ff2400;
}

.barra-esquerda {
  left: 25%;
  transform: skew(15deg);
}

.barra-direita {
  right: 25%;
  transform: skew(-15deg);
}


.conteudo {
  min-height: calc(100vh - 100px);
  background-color: #d9d9d9;
}
</style>


