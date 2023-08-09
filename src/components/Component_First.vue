<template>
    <!-- <h3>Je suis le premier</h3> -->
    <Component_Second />
</template>

<script>
import Component_Second from './Component_Second.vue';

    export default {
         name: 'Component_First',
         components:{   
            Component_Second
}
    }
</script>

<style scoped>

</style>