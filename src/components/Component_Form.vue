<template>
   <fieldset>
    <div><label for="name">Nom_Utilisateur :</label></div>
    <div><input type="text"></div>
    <div><label for="name">Mot de passe :</label></div>
    <div><input type="password"></div>
   </fieldset>
    
</template>

<script>
    export default {
        name: 'Component_Form',
        
    }
</script>

<style scoped>
    input[type='text']{
        display: inline;
        width: 300px;
        padding: 5px 10px;
        color: rgb(13, 14, 14);
        border-radius: 7px;
        border: 2px solid olive;
    }
    input[type='password']{
        display: inline;
        width: 300px;
        padding: 5px 10px;
        color: aqua;
        border-radius: 7px;
        border: 2px solid olive;
    }
    label{
        font-size: 24px;
        color: olive;
        font-family: Arial, Helvetica, sans-serif;
        font-style: italic;
        display: block;
        margin-left: 20px;
    }
    div{
        display: block;
        
    }
    fieldset{
        width: 400px;
        height: auto;
        border: 3px solid black;
    }
</style>