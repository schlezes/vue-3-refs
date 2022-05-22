<template>
    <A color="white" bgColor="blue"/>
    <B />
</template>

<script>
    import A from './components/A.vue'
    import B from './components/B.vue'

    export default {
        name: 'App',
        components: {
        A,
        B
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style>
    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        background-color: #CCCCFF;
    }

</style>
