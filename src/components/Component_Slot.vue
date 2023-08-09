<template>
    <div class="card">
        <slot> </slot>      
    </div>
</template>

<script>
    export default {
        name:'Component_Slot',
        props:['contenu']
        
    }
</script>

<style scoped>
.card{
    box-shadow: 0px 24px 12px 0px rgb(79, 79, 80);
    padding: 10px;
    margin-left: 70%;
    width: 200px;
    
}
.card:hover{
    box-shadow: 0px 12px 6px 0px rgb(86, 94, 107);
}

</style>