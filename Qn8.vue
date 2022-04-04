<template>

<div>
<p>Question8</p>
<p @click="result()">p tag</p>


<textarea id="sample"> </textarea>

</div>

</template>




<script>

export default {

name: "QuesEight",


data() {

return {

text: "",

};

},


methods: {

result() {

this.text = document.write("" + document.getElementById("sample").value);

},

},

};

</script>