<script setup lang="ts">

</script>


<template>
  <form class="form-container">
    <h1>Warehouse Management System</h1>
    <div class="form-group">
      <label for="username">Usuario:</label>
      <input id="username" type="text" placeholder="ingrese su usuario" />
    </div>
       <br>
    <div class="form-group">
      <label for="password">Contraseña:</label>
      <input id="password" type="password" placeholder="Ingrese su contraseña" />
    </div>
    <br>
    <button type="submit">Registrarse</button>
  </form>
</template>



<style>
.form-container {
  max-width: 350px;
  margin: 2rem auto;
  padding: 2rem 1.5rem 1.5rem 1.5rem;
  background: #191414;
  border-radius: 12px;
  box-shadow: 0 2px 20px rgba(30, 215, 96, 0.08);
  font-family: 'Circular Std', 'Helvetica Neue', Arial, sans-serif;
}

.form-group {
  margin-bottom: 1.3rem;
}

label {
  display: block;
  margin-bottom: 0.3rem;
  color: #ffffff;
  font-weight: 700;
  font-size: 1em;
  letter-spacing: 0.02em;
}

input[type="text"],
input[type="password"] {
  width: 70%;
  padding: 0.7rem 0.9rem;
  border: none;
  background: #121212;
  color: #fff;
  font-size: 1em;
  border-radius: 8px;
  margin-top: 0.2rem;
  transition: box-shadow 0.25s;
 text-align: center;
  box-shadow: 0 0 0 2px transparent;
}

input[type="text"]:focus,
input[type="password"]:focus {
  outline: none;
  box-shadow: 0 0 0 2px #1ed760;
}

button[type="submit"] {
  width: 100%;
  padding: 0.9rem 0;
  background: #1ed760;
  color: #191414;
  font-weight: bold;
  font-size: medium;
}
</style>
