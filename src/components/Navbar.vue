<template>
    <div id="nav">
        <router-link to="/" id="logo-url">
            <img :src="logo" :alt="alt" id="logo">
        </router-link>
        <router-link to="/">Home</router-link>
        <router-link to="/pedidos">Pedidos</router-link>
    </div>
</template>
<script>
    export default{
       name: 'Navbar',
       props: ["logo", "alt"]
    }
</script>
<style scoped>
    #nav{
        background-color: #222;
        border-bottom: 4px solid #111;
        padding: 5px 20px;
        display: flex;
        justify-content: flex-end;
        align-items: center;
    }

    #nav #logo-url{
        margin: auto;
        margin-left: 0;
    }

    #logo{height: 60px;
        width: 60px;
        object-fit: cover;
    }

    #nav a{color: #FCBA03;
        text-decoration: none;
        margin: 12px;
        transition: .5s;
    }
    #nav a:hover{
        color: #fff;
    }
</style>