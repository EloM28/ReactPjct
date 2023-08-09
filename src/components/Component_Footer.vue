 <template>
    <div>
        <h2 v-bind:style="link">Github : Bosconishi Password : nBosco711@</h2>
    </div>
</template>

<script>
    export default {
        name : 'Component_Footer',
        data(){
            return{
            link:{ border:'2px solid cyan', marginTop:'100px',fontSize:'28px',color:'blue'}}
        }
    }
</script>

<style scoped>

</style>