<template>

  <Acc_bonjour nom='NISHIME ' prenom="JEAN Bosco" />
  <h2>Utilisateur {{ surnom }} {{ nompropre }}</h2>
  <button @click="user=true">Commencer</button> <br>
  <Component_First v-if="user" @fermer="user=false"/> <br>
  <button @click="showpopup=true">Indication</button> <br>
  <Component_Popup v-if="showpopup" @close="showpopup=false"/> <br>
  <Component_Form />
  <Component_Slot > Developpeur</Component_Slot>
  <Component_Slot > <img src="bsc.jpeg" alt="my picture" style="height: 150px; width: 150px;"></Component_Slot>
  <Component_Footer />
</template>

<script>
import Acc_bonjour from './components/Acc_bonjour.vue';
import Component_First from './components/Component_First.vue';
import Component_Form from './components/Component_Form.vue';
import Component_Footer from './components/Component_Footer.vue'
import Component_Popup from './components/Component_Popup.vue';  
import Component_Slot from './components/Component_Slot.vue';
export default {
  name: 'App',
  components: {
    Acc_bonjour,
    Component_First,
    Component_Footer,
    Component_Popup,
    Component_Form,
    Component_Slot
},
  data(){
    return{
            showpopup: false,
            user:false,
            surnom:'Mignon', 
            nom: '',
            nompropre:"Bosco"
               
            }
        },
   provide() {
    return{
        username: this.surnom,
    }
    
   },    
   methods:{

   }
  }

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center; 
  color: #2c3e50;
  margin-top: 60px;
  display: block;
  justify-content: center;
  align-items: center;
  /* height: 100vh; */
  height: 90%;

}
body{
  background-color: rgb(88, 87, 84);
}
h1{
  border: 2px solid cyan;

}
button{
  display: block;
  width: 300px;
  border: 2px solid olive;
  margin: 10px;
  border-radius: 5px;
}

</style>
