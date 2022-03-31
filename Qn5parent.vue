<template>
    <div class ="parent">
        <child @my-message="capturemymessage"/>
        bose said me '{{ bosedialouge }}'
        <name></name>
    </div>
</template>
<script>
import child  from '@/components/Qn5.vue'

export default {
 name: "parentU",
 
 data()
 {
     return {
         bosedialouge:"",
     };
 },
 methods:
 {
     capturemymesssage(mess){
         console.log(mess);
     
     this.bosedialouge=mess;
     },
 },
 components:
 {
     child,
 },
};
</script>
