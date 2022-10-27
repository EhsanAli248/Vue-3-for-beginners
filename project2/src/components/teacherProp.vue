<template>
    <div>
        <h2>Teacher Data:{{name}}</h2>
    </div>
</template>
<script>
    export default{
        name:"teacherProp",
            props:{
                name:String
            }
        }
    
</script>
<style scoped>
    h2{
        color: greenyellow;
        background-color: blanchedalmond;
    }
</style>