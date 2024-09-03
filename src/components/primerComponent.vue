<template>
    <div>
    <h1>{{ titulo }}</h1>
    <h1>El nombre es:
        {{ nombre }}</h1>
    <h1>La edad es:
        {{ edad }}</h1>
    <img v-bind:src="src" v-bind:alt="cosmonauta" :style="imagenStyle"/>
    <div v-bind:style="{ color: textColor }">{{ userdata }}</div>
    <input type="text" v-model="userdata"/>
    </div>
</template>

<script>
    export default {
        name: 'PrimerComponent',
        props: {
            titulo: String,
            nombre: String,
            edad: Number,
            src: String,
            alt: String,
            imagenStyle: Object
        },
        data() {
            return {
                userdata: "un valor",
                textColor: "blue"
            };
        }
    };
</script>

<style>

</style>