<script setup>
import NavBar from './components/NavBar.vue';
import ComponenteProyectos from './components/ComponenteProyectos.vue';
import ComponenteEducacion from './components/ComponenteEducacion.vue';
import ComponenteContacto from './components/ComponenteContacto.vue';
import ComponenteAbout from './components/ComponenteAbout.vue';
</script>

<template>
 <header>
    <NavBar />
  </header>
  <main>
    <section id="about">
      <h2>Sobre mí</h2>
      <ComponenteAbout />
    </section>
    <section id="educacion">
      <h2>Educación</h2>
      <ComponenteEducacion />
    </section>
     <section id="proyectos">
      <h2>Proyectos</h2>
      <ComponenteProyectos />
    </section>
    <section id="contacto">
      <h2>Contacto</h2>
      <ComponenteContacto />
    </section>
  </main>

  <footer>
    <a href="#top">
      <button class="botonInicio">Inicio</button>
    </a>
    <p>© Elias Jacob - Portafolio Web - UTN FRSR 2024</p>
  </footer>
</template>

<style scoped>

h2, p, li, button {
  background-color: rgba(0, 0, 0, 0.5); /* Dark background, 50% transparency */
  color: white; /* Texto blanco para contraste */
  padding: 10px; /* agrega padding al texto */
  border-radius: 5px; /* Bordes rondeados */
}


section {
  padding: 20px;
}
</style>