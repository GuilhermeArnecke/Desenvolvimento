<template>
  <div class="pagina">
    <header>
      <img :src="dndIcon" alt="d&d">
    </header>

  </div>
</template>

<script setup>
import { onMounted, ref } from "vue";
import axios from "axios";

import dndIcon from "./assets/dndicon.png" 
</script>

<style>
header {
  height: 100px;
  width: 100%;

  display: flex;
  justify-content: center;
  align-items: center;
}

header img {
  max-height: 65px;
  max-width: 100%;
  object-fit: contain;
}
</style>


