<script setup lang="ts">
import Login from './components/Login.vue';
import HeaderBar from './components/HeaderBar.vue';
import Home from './components/Home.vue';
import FooterBar from './components/FooterBar.vue';
import Salida from './components/Salida.vue';
import Stock from './components/Stock.vue';
import Picking_Packing from './components/Picking_Packing.vue';
import Almacenaje from './components/Almacenaje.vue';
import Entrada from './components/Entrada.vue';
</script>


<template>
<Login></Login>

<div class="estilo">
<HeaderBar></HeaderBar>
<Home></Home>
<FooterBar></FooterBar>
</div>

<div class="estilo">
<HeaderBar></HeaderBar>
<Entrada></Entrada>
<FooterBar></FooterBar>
</div>

<div class="estilo">
<HeaderBar></HeaderBar>
<Almacenaje></Almacenaje>
<FooterBar></FooterBar>
</div>

<div class="estilo">
<HeaderBar></HeaderBar>
<Stock></Stock>
<FooterBar></FooterBar>
</div>

<div class="estilo">
<HeaderBar></HeaderBar>
<Picking_Packing></Picking_Packing>
<FooterBar></FooterBar>
</div>

<div class="estilo">
<HeaderBar></HeaderBar>
<Salida></Salida>
<FooterBar></FooterBar>
</div>

</template>


<style>
.estilo {
  text-align: left;
  color: #ffffff;
  background-color: #000000;
  max-width: 350px;
  margin: 2rem auto;
  padding: 1rem 1.5rem 1rem 1.5rem;
  border-radius: 10px;
  background: #191414;
  box-shadow: 0 2px 20px rgba(30, 215, 96, 0.08);
  font-family: 'Circular Std', 'Helvetica Neue', 'Arial', 'sans-serif';
}
</style>|