<template>
    <button @click="onClick()" class="btn" :style="{ background: color }">
        {{text}}
    </button>
</template>

<script>
export default {
    name: 'Button-Comp',
    props: {
        text: String,
        color: String,
    },
    methods:{
        onClick(){
            console.log('Click')
        }
    }
}
</script>

<style scoped>

</style>