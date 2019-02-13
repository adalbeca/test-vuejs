<template>
    <div id="app">
        <notas />
    </div>
</template>

<script>
    import notas from './components/Notas.vue'

    export default {
        name: 'app',
        components: {
            notas
        }
    }
</script>

<style>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;

        color: #2c3e50;
        margin-top: 20px;
    }
</style>
