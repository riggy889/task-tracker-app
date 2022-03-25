<template>
    <div :key="task.id" v-for="task in tasks" >
        <Task @delete-task="$emit('delete-task',
        task.id)" :task="task" />
    </div>
</template>

<script>
import Task from './Task-Comp.vue'

export default {
    name: 'Tasks-Comp',
    props: {
        tasks: Array,
    },
    components: {
        Task,
    },
    emits: ['delete-task'],
}
</script>