<template>

<div>

<b-card>

title="Company data"

<b-card-text v-for="userdata in data" :key="userdata.id">

name:{{userdata.name}},

discription:{{userdata.description}}

</b-card-text>

</b-card>

</div>

</template>

<script>

export default{

name:'CardA',

data(){

return{

data : [{ "name" :" Agile CRM" ,"description" :" A company of excellence"},

{"name":"mantra technologies", "description":"500apps" },

{"name":"500apps Python","description":"Backend built using python" },

{"name":"500apps infinity","description":"Builtusing vue JS" }]

}

}

}

</script>