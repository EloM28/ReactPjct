<template>
    <h3>{{ username }} : Je suis le troisieme</h3>
    <button @click="$emit('fermer')">On a Vu</button>
</template>

<script>
    export default {
        name: 'Component_Third',
        inject: ['username'],
        components:{
           
        },
        emits:['fermer']
    }
    
</script>

<style scoped>

</style>