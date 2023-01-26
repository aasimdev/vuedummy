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




    <!-- --------------------3------------------------------
    
    <label for="checkbox1">checbox1</label>
    <input type="checkbox" value="checbox1" id="checkbox1" v-model="checkbox">
    <br>
    <label for="checkbox2">checbox2</label>
    <input type="checkbox" value="checbox2" id="checkbox2" v-model="checkbox">
    <br>
    <label for="checkbox3">checbox3</label>
    <input type="checkbox" value="checbox3" id="checkbox3" v-model="checkbox">
    
    <h4>Selected chexbox : {{ checkbox }}</h4> -->




    <!----------------------4------------------------------>

    <!-- loops in vue -->
    <!-- <ul>
        <li v-for="item in languages" :key="item">
            {{ item }}
        </li>
    </ul>
    <br>
    <br>
    <ul>
        <li v-for="item in user " :key="item.email">
            name: is {{ item.name }} email: is {{ item.email }}
        </li>
    </ul> -->



    <!----------------------5------------------------------>

    <!-- get data from child components -->

    <!-- <child name="userName" :user="user" :getData="getData"/> -->

    <!---------------------------6-------------------------------->
    <!-- html binding -->
    <!-- 
     <div v-html="tag"></div>
     <div v-html="tag + tag2 + tag3"></div> -->



     
    <!---------------------------7-------------------------------->
    <!-- css binding -->

    <h2 class="heading" :class="{active:applyclass}">
        Home Components
    </h2>
    <button v-on:click="applyclass=!applyclass">Apply Class</button>

</template>
<script>

import child from './child.vue';
export default {
    name: 'home',
    components: {
        child
    },
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

    // data() {
    //     return{
    //         checkbox:[]
    //     }
    // }


    // <!----------------------4-------------------------------->
    //                     Loops in vue


    // data() {
    //     return {
    //         languages: ['javascript', 'node', 'php', 'python',],
    //         user: [{
    //             name: 'umar',
    //             email: 'mail@mail.com',
    //         },
    //         {
    //             name: 'abdullah',
    //             email: 'mail@mail.com',
    //         },
    //         {
    //             name: 'rehman',
    //             email: 'mail@mail.com',
    //         },
    //         {
    //             name: 'rohan',
    //             email: 'mail@mail.com',
    //         }]
    //     }
    // }





    // <!----------------------5-------------------------------->
    // //               get data from child components

    // data() {
    //     return {
    //         user:{name: 'peter',email: 'peter@mail.com'}
    //     }
    // },
    // methods:{
    //     getData(){
    //         console.warn("function from home component")
    //     }
    // }



    // <!----------------------6-------------------------------->
    //  html binding


    // data() {
    //     return {
    //         tag: '<h1>data</h1>',
    //         tag2: '<h2>data</h2>',
    //         tag3: '<h3>data</h3>',
    //     }
    // }


    // <!---------------------------7--------------------------------->
    // css binding


    data(){
        return{
            applyclass: false
        }
    },
}
</script>
<style>
.active{
    color: blue;
}
</style>