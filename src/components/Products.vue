<script>
import imagenes from "./Img.vue";
import grid from "./Grid.vue";
export default {
    props: {
        url: {
            String
        },
        nombre: {
            String
        },
        descripcion: {
            String
        },
        precio: {
            String
        },
    },
    components: { grid, imagenes }
};
</script>
    
<template>
    <grid>
        <imagenes>
            <img v-bind:src="url" alt="Vue.js">
        </imagenes>
        <h2>{{nombre}}</h2>
        <p>{{precio}}</p>
        <p>{{descripcion}}</p>
    </grid>
</template>
    
<style scoped>

a {
    text-decoration: none;
    color: snow;
    background: #301675;
    padding: 0.3rem;
    border-radius: 5px;
    border: 1px solid #f2f2f2;
    font-size: small;
    margin: 0.5rem 0.25rem;
}
</style>