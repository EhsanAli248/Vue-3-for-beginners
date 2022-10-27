<template>
    <div>
        <h2>Student Data:{{name}}</h2>
    </div>
</template>
<script>
    export default{
        name:"studentProp",
            props:{
                name:String
            }
        }
    
</script>
<style scoped>
    h2{
        color: blue;
        background-color: aqua;
    }
</style>