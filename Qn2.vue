<template>

<div>

<table>

<thead>

<tr>

<th>Name</th>

</tr>

</thead>

<tbody>

<tr v-for="users in items" :key="users.id">

<td>{{users.name}}</td>

<td>{{users.index}}</td>

</tr>

</tbody>

</table>

</div>

</template>


<script>

export default {

name:"TABLEa23",

data() {

return {

fields:['name','description'],

items: [

{"name":" Agile CRM" , "description" :" A company of excellence"},

{"name":"mantra technologies", "description":"500apps" },

{"name":"500apps Python", "description":"Backend built using python" },

{"name":"500apps infinity", "description":"Built using vue JS" },

]

}

}

}

</script>