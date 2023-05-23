<script setup>
import {produtos} from '@/_data/produtos'
</script>

<template>
<h1>Taylor Swift Store</h1>
<div class="listagem-produtos">
<div v-for=" produto in produtos" :key="produto.id" class="card-produto">
  <img :src="produto.image" alt="imagem" class="produto imagem">
  <p class="produto-name">{{ produto.nome }}</p>
  <p class="produto-preco">{{ produto.price }}</p>

</div>

</div>


</template>

<style scoped>

.listagem-produtos{
  display: flex;
  flex-wrap: wrap;
  justify-content: stretch;
}
 .listagem-livros p{
  margin: 0;
 }

.card-produto{
  background-color: rgba(137, 43, 226, 0.719);
  padding: 10px;
  border-radius: 10px;
  width: 600px;
  margin: 10px;
}
.produto-imagem{
  width: 60px;
}






</style>
