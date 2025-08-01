<script setup lang="ts">
import { ref } from 'vue';
interface NavItem {
  name: string;
  link: string;
}

const navItems = ref<NavItem[]>([
  { name: 'Entrada', link: '../modules/entrada/Index.vue' },
  { name: 'Movimiento', link: '/movimiento' },
  { name: 'Stock', link: '/stock' },
  { name: 'Picking/Packing', link: '/picking-packing' },
  { name: 'Salida', link: '/despacho' },
]);
</script>


<template>
<div class="divnav">
  <nav class="navbar-vertical">
    <h4 class="usuario">Usuario: 'RIVO'</h4>
    <ul>
      <li v-for="(item, index) in navItems" :key="item.name">
        <a :href="item.link">
          {{ index + 1 }} - {{ item.name }}
        </a>
      </li>
    </ul>
  </nav>
</div>
</template>


<style scoped>
.usuario {
  text-align: center;
  color: #000000;
  border-radius: 10px;
 }

.divnav {
  display: flex;
  align-items: center;
  justify-content: center;
  max-width: 400px;
  font-family: 'Circular Std', 'Helvetica Neue', 'Arial', 'sans-serif';

}

.navbar-vertical {
  width: auto;
  background-color: #1ed760;
  height: auto;
  margin: 1rem auto;
  padding: 0rem 2.5rem 0rem 2.5rem;
  border-radius: 12px;
  text-align: left;
  box-shadow: 0 2px 20px rgb(30, 215, 95);
}

.navbar-vertical ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.navbar-vertical li {
  margin: 1rem 0;
}

.navbar-vertical a{
  color: #191414;
  text-decoration: none;
  font-weight: 600;
  display: block;
  padding: 0.5rem 1rem;
  border-radius: 4px;
  font-weight: bold;
}

.navbar-vertical a:hover {
  background-color: #097941;
}
</style>
