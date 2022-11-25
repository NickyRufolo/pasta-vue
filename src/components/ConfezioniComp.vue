<template>
    <div class="Confezioni-card">
        <img :src="propsConfezione.img" alt="">
        <h2>{{propsConfezione.name}}</h2>
    </div>
    </template>
    
    
    
    <script>
    export default {
        name: 'ConfezioniComp',
        props: {
            propsConfezione : Object
        }
    }
    </script>
    
    <!-- Add "scoped" attribute to limit CSS to this component only -->
    <style scoped lang="scss">
    .Confezioni-card {
    width: calc(( 100% / 5 ) - 20px );
    border: 1px solid rgb(255, 0, 0);
    text-align: center;
    margin: 10px 10px;
    }
    .Confezioni-card > img {
    width: 100%;
    }
    </style>