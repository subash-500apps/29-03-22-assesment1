<template>
    <div class ="parent">
        <child @my-message="capturemymessage"/>
        bose said me '{{ bosedialouge }}'
    </div>
</template>
<script>
import child  from '@vue/composition-api'

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
