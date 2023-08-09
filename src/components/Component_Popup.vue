<template>
    <h2 v-bind:style="css">Naviguer entre les liens</h2>
    <button v-bind:style="css" @click="$emit('close')">ClosePopup</button>
</template>

<script>
    export default {
        name: 'Component_Popup',
        css:{alignText:'left', color:'red', fontStyle:'italic'},
        emits:['close']
    }
</script>

<style scoped>

</style>