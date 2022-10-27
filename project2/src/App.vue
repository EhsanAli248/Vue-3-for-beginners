<template>
<img alt="Vue logo" src="./assets/logo.png">
<!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
<!-- <StudentProp name="Ehsan Ali" /> -->
<!-- <StudentProp :name="name" /> -->
<!-- <TeacherProp name="Dr Rashid " /> -->
<!-- <childProp :getuser="getuserName"/>
<h2>{{childName}}</h2> -->
<!-- <RefLec/> -->
<!-- <h1>This Lecture is about slots</h1>
<slotLec>
    <h1>slot component</h1>
</slotLec>
<SlotLec></SlotLec> 
<slotLec><a href="#">practice about slot component</a></slotLec><br><br>
<slotLec><img src="C:\Users\FLUXYSTEMS\Pictures\Saved Pictures" /></slotLec><br><br> -->
<!-- <MultipleSlot>
    <template v-slot:s1>
        <h1>Multiple slots info</h1>
    </template>
    <template v-slot:s2>
        <button>Touch me</button>
    </template>
    <template v-slot:s3>
        <p>Multiple slots info</p>
    </template>
</MultipleSlot> -->
<h1>Dynamic Components</h1>
<button @click="tab='DynmComp1'">Press D1</button>
<button @click="tab='DynmComp2'">Press D2</button>
<button @click="tab='DynmComp3'">Press D3</button>
<!-- <DynmComp1/>
<DynmComp2/>
<DynmComp3/> -->
<component :is="tab"/>
</template>

<script>
import DynmComp1 from './components/DynmComp1.vue';
import DynmComp2 from './components/DynmComp2.vue';
import DynmComp3 from './components/DynmComp3.vue';
// import RefLec from './components/refLec.vue';
// import StudentProp from './components/studentProp.vue';
// import TeacherProp from './components/teacherProp.vue';
// import childProp from './components/childProp.vue';
// import HelloWorld from './components/HelloWorld.vue'
// import slotLec from './components/slotLec.vue';
// import MultipleSlot from './components/multipleSlot.vue';

export default {
    name: 'App',
    components: {
    DynmComp1,
    DynmComp2,
    DynmComp3
},
    data() {
        return {
            // name:'',
            // name:"Baba",
            // childName:'',
            tab:'',
        }
    },
    // methods:{
    //     getuserName(name){
    //         this.childName=name;
    //     }
    // }
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
}
</style>
