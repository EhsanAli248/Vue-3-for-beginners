<template>
    <h2>Lecture about reference</h2>
    <input type="text" ref="input"><br><br>
    <button @click="getdata">Click Me</button>
</template>
<script>
    export default{
        name:"refLec",
        data(){
            return{

            }
        },
        methods:{
            getdata(){
                this.$refs.input.focus();
                let val=this.$refs.input.value;
                this.$refs.input.style.color="green";
                console.warn(val);
            }
        }

    }

</script>