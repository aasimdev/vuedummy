<template>

<h2>{{name}}</h2>
<h2>
    {{ user.name }}
</h2>
<button v-on:click="getData()">press btn</button>

</template>

<script>
export default{

    name : 'child',
    props : {
        name : String,
        user : Object,
        getData: Function
    }

}
</script>