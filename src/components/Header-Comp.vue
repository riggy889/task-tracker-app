<template>
    <header>   
        <h1>{{title}}</h1>
        <Button text="This is a button" color="green" />
    </header>
</template>

<script>
import Button from './Button-Comp.vue'

export default {
    name: 'Header-Comp',
    props: {
        title: String,
    },
    components: {
        Button,
    }
}
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>