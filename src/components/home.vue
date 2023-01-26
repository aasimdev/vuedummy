<template>

    <!----------------------1-------------------------------->
    <!-- <h1 v-on:mousemove="getConcole()">Hover me</h1>
    <button v-on:click="getData()">click me</button>
    <button v-on:dblclick="getData('Button double clicked')">double click here</button>
    <h2>{{ count }}</h2> -->


    <!----------------------2-------------------------------->
    <!-- <input type="email" placeholder="enter email" v-model="email">
    <br>
    <br>
    <input type="password" placeholder="enter password" v-model="password">
    <br>
    <br>
    <button v-on:click="getValue()" type="submit">Get data</button> -->


   
    
    <!----------------------3-------------------------------->
    
    <label for="checkbox1">checbox1</label>
    <input type="checkbox" value="checbox1" id="checkbox1" v-model="checkbox">
    <br>
    <label for="checkbox2">checbox2</label>
    <input type="checkbox" value="checbox2" id="checkbox2" v-model="checkbox">
    <br>
    <label for="checkbox3">checbox3</label>
    <input type="checkbox" value="checbox3" id="checkbox3" v-model="checkbox">
    
    <h4>Selected chexbox : {{ checkbox }}</h4>
</template>
<script>
export default {
    name: 'home',
    // <!----------------------1-------------------------------->
    // data() {
    //     return {
    //         count: 0
    //     }
    // },
    // methods: {
    //     getData() {
    //         this.count = this.count + 1
    //     },
    //     getConcole() {
    //         console.log('mouse move on h1')
    //     }
    // }




    // <!----------------------2-------------------------------->
    // data() {
    //     return {
    //         email: null,
    //         password: null
    //     }
    // },
    // methods:{
    //      getValue() {
    //         console.log('Value :',this.email,this.password)
    //      }
    // }
    



    // <!----------------------3-------------------------------->

    data() {
        return{
            checkbox:[]
        }
    }
 
}
</script>