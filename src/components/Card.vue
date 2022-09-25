<template>
    <div>
        <img v-bind:src ="url" alt="nombre">
        <h1>{{ nombre }}</h1>
        <h4>${{precio}}</h4>
        <p>{{ descripcion }}</p>
        <a v-bind:href="url" target="_blank"> ¡ $ COMPRAME!</a>
    </div>
</template>

<style scoped>
    
    div{
        display: inline-block;
        text-align: center;
        border: .5px solid #6e3415;
        background: #e8cea0;
        padding: 1%;
        border-radius: 13px;
        margin: 3px;
        margin-left: 15px;
        margin-bottom: 20px;
        margin-block: 15px;
        width: 380px;
        height: 400px;
        
    }
    img{
        width: 15rem;
        height: 15rem;
        padding: 0.8rem;
    }
    a{
        text-decoration: none;
        color: snow;
        background: #FFAC41;
        padding: 0.3rem;
        border-radius: 5px;
        border: 1px solid #c8bca8;
    }
</style>

<script>
    export default{
        props:{
            url:{
                String,
            },
            nombre:{
                String,
            },
            descripcion:{
                String,
            },
            precio:{
                String,
            },
        },
    };
</script>