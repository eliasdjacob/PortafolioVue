<script setup>
</script>

<template>
  <ul class="navbar">
    <li><a href="#about">Sobre mi</a></li>
    <li><a href="#educacion">Educación</a></li>
    <li><a href="#proyectos">Proyectos</a></li>
    <li><a href="#habilidades">Habilidades</a></li>
    <li><a href="#contacto">Contacto</a></li>
  </ul>
</template>

<style scoped>
body, html {
  margin: 0;
  font: bold 14px/1.4 'Open Sans', arial, sans-serif;
  background: #000;
}

ul { 
  margin: auto; 
  padding: 0; 
  list-style: none; 
  display: table;
  width: 600px;
  text-align: center;
  display: flex;
  justify-content: space-between;
}

li { 
  display: table-cell; 
  position: relative; 
  padding: 15px 0;
}

a {
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
  text-transform: uppercase;
  text-decoration: none;
  letter-spacing: 0.15em;
  display: inline-block;
  padding: 15px 20px;
  position: relative;
  border-radius: 5px;
  white-space: nowrap; /* Prevent "Sobre mi" from breaking into two lines */
}

a:after {    
  background: none repeat scroll 0 0 transparent;
  bottom: 0;
  content: "";
  display: block;
  height: 2px;
  left: 50%;
  position: absolute;
  background: #fff;
  transition: width 0.3s ease 0s, left 0.3s ease 0s;
  width: 0;
}

a:hover:after { 
  width: 100%; 
  left: 0; 
}

a:hover {
  background-color: rgba(0, 0, 0, 0.7);
}

.navbar {
  position: relative;
  z-index: 100; /* Set a high number to ensure it stays on top */
}

@media screen and (max-height: 300px) {
  ul {
    margin-top: 40px;
  }
}
</style>