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
    data(){
        return{
            items:[
                {title:'About Project',icon:'mdi-help-box'},
                {title:'Team',icon:'mdi-account-group'},
            ],
            right:null,
        }
    }
}
</script>

<style>

#nav{
    display:flex;
    justify-content: center;
    background-color:rgb(76, 175, 80);
    padding:10px;
}
#nav a{
    font-weight: bold;
    color: white;
    text-decoration: none;
    padding: 10px;
    font-size: 1.5em;
    
}
#nav a.router-link-exact-active {
    color: black;
}
body{
  background: red;
}
</style>