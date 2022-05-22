<template>
    <div ref="id=0" style="background-color: rgb(255, 153, 0);" v-bind:style="{width: 50 + 'px', height: 50 + 'px'}" v-on:click="expand($event, 'id=0')" ></div>
    <div ref="id=1" style="background-color: rgb(204, 255, 0);" v-bind:style="{width: 50 + 'px', height: 50 + 'px'}" v-on:click="expand($event, 'id=1')" ></div>
    <div ref="id=2" style="background-color: rgb(51, 255, 0);"  v-bind:style="{width: 50 + 'px', height: 50 + 'px'}" v-on:click="expand($event, 'id=2')" ></div>
    <div ref="id=3" style="background-color: rgb(0, 255, 102);" v-bind:style="{width: 50 + 'px', height: 50 + 'px'}" v-on:click="expand($event, 'id=3')" ></div>
    <div ref="id=4" style="background-color: rgb(0, 255, 255);" v-bind:style="{width: 50 + 'px', height: 50 + 'px'}" v-on:click="expand($event, 'id=4')" ></div>
    <div ref="id=5" style="background-color: rgb(0, 102, 255);" v-bind:style="{width: 50 + 'px', height: 50 + 'px'}" v-on:click="expand($event, 'id=5')" ></div>
    <div ref="id=6" style="background-color: rgb(51, 0, 255);"  v-bind:style="{width: 50 + 'px', height: 50 + 'px'}" v-on:click="expand($event, 'id=6')" ></div>
    <div ref="id=7" style="background-color: rgb(204, 0, 255);" v-bind:style="{width: 50 + 'px', height: 50 + 'px'}" v-on:click="expand($event, 'id=7')" ></div>
    <div ref="id=8" style="background-color: rgb(255, 0, 153);" v-bind:style="{width: 50 + 'px', height: 50 + 'px'}" v-on:click="expand($event, 'id=8')" ></div>
    <div ref="id=9" style="background-color: rgb(255, 0, 0);"   v-bind:style="{width: 50 + 'px', height: 50 + 'px'}" v-on:click="expand($event, 'id=9')" ></div>
</template>

<script>
    export default {
        name: 'B',
        data: function () {
            return {
                hi: "hi"
            }
        },
        methods: {
            expand(e, y) {
                console.log(this.$refs)
                const z = this.$refs
                const w = Reflect.get(z, y)
                w.style.width = parseInt(w.style.width) * 1.25 + "px"
                w.style.height = parseInt(w.style.height) * 1.25 + "px"
            },
        }
    }

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>

div {
    display: inline-block;
    margin: 1%;
    border-radius: 5px;
    transition: all 0.5s ease 0s;

}
</style>