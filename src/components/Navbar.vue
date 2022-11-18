<template>
    <div id="nav">
        <div class="link">
            <router-link :to="{name:'home'}" class="navbar-button">Home</router-link> 
            <router-link :to="{name:'about'}" class="navbar-button">About</router-link>
            <router-link :to="{name:'team'}" class="navbar-button">Team</router-link>
        </div>
    </div>
</template>

<script>
export default {
}
</script>

<style>

#nav{
    display:flex;
    justify-content: center;
    background-color:#fff;
    padding:10px;
}
#nav a{
    font-weight: bold;
    color: #2c3e50;
    text-decoration: none;
    padding: 10px;
    font-size: 1.5em;
    
}
#nav a.router-link-exact-active {
    color: #41b883;
}
</style>