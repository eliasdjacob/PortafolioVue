<script setup>

import { ref } from 'vue';
import FondoIntereses from './FondoIntereses.vue';
const intereses = ref([
    'Nuevos conocimientos: Estoy en una búsqueda continua de nuevos conocimientos, especialmente en el campo de la ciencia de datos, para poder satisfacer las necesidades de mis clientes de la mejor manera posible.',
    'Trabajo en equipo: Para mí, es fundamental que siempre prime el trabajo en equipo y la buena predisposición de todos los integrantes, creando así un clima de trabajo ameno.',
    'Perfeccionamiento de mis habilidades: A través del aprendizaje constante mediante la educación formal y autodidacta, busco ser un mejor profesional y crecer en mi rubro.',
]);

</script>


<template>

 <div class="intereses-contenedor">
        <FondoIntereses />
        <ul class="contenedor-lista">
            <li class="item" v-for="interes in intereses" :key="interes">
                {{ interes }}
            </li>
        </ul>
    </div>

</template>

<style scoped>

.intereses-contenedor {
    display: flex;
    position: relative;
    margin: 0 auto;
    max-width: 85%;
    padding: 1rem;
    z-index: 1;
}

.contenedor-lista {
    list-style-type: none;
    padding: 1rem;
    margin-bottom: .5rem;
    color: var(--vt-c-white-soft);
    font-size: 1.4rem;
    text-shadow: 3px 3px 6px rgba(0, 0, 0, 1);
    z-index: 1;
}

.item {
    margin-bottom: 1rem;
}

</style>