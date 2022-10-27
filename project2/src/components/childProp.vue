<template>
    <div>
        <h2>Child to parent</h2>
        <button v-on:click="getuser(name)">send User Name</button>
    </div>
</template>
<script>
    export default {
        name:"childProp",
        data(){
            return{
                name:"Ehsan Ali"
            }
        },
        props:{
            getuser:Function
        }
        
    }
</script>