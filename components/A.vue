
<template>
    <header class="header-box" 
        v-bind:style="{color: color, backgroundColor: bgColor}">
        <h1>{{title="Header component - May, 2022"}}</h1>
    </header>
</template>

<script>
export default {
    name: 'A',
    props: {
        title: String,
        color: String,
        bgColor: String
    }
}
</script>

<style scoped>

.header-box {
    display: flex;
    align-content: center;
    justify-content: center;
	min-height: 65px;
    margin-bottom: 5px;
    border-radius: 7px;
    font-family: DejaVu Sans-serif bold;
}
h1 {
    font-size: 3em;
    margin: 0;
}
</style>

