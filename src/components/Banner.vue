<template>
    <div id="main-banner">
        <h1>Make Your Banner</h1>
    </div>
</template>
<script>
    export default{
        name: "Banner"
    }
</script>

<style scoped>

    #main-banner{
        background-image: url('/img/snorlax2.png');
        background-position: 0 -150px;
        background-repeat: no-repeat;
        background-size: cover;
        height: 550px;
        display: flex;
        align-items: center;
        justify-content: flex-start;
    }

    #main-banner h1{padding: 20px;
        color: #fff;
        text-align: center;
        font-size: 40px;
        background-color: #222;
    }
    /*RESPONSIVO:*/
    @media screen and (max-width: 960px){
        #main-banner{flex-wrap: wrap;}
    }
</style>