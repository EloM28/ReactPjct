<template>
    <h1>Hellooo {{ nom }} {{ prenom }}, welcome for using New-App.</h1>
    <h2 v-html="a" v-bind:style="linkStyle"></h2>
    <h2 v-html="s" v-bind:style="linkStyle"></h2>
    <h2 v-html="p" v-bind:style="linkStyle"></h2>
    <!-- <div v-html="lien" v-bind:style="link"></div> -->
</template>

<script>
    export default {
        name: 'Acc_bonjour',
        data(){
            return{
                //lien: '<span><a href="https://google.com">Visit Google</a></span>',
                a: '<a href="#">Accueil</a>',
                s: '<a href="#">Principals services</a>',
                p: '<a href="#">Informations</a>',
                linkStyle:{display:'inline',color:'blue', padding:'50px'},
                link:{ border:'2px solid cyan', marginTop:'300px',fontSize:'28px',color:'blue'}

            }
        },
        props:['nom','prenom'],
    }
</script>

<style scoped>

</style>

