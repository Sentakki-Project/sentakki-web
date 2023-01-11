<template>
    <h1>Backend</h1>  
    <div class="conteiner">
        <div class="element">
            <img :src="require(`@/assets/${ror}`)" alt="asp-net-logo">
            <p>Ruby on Rails</p>
        </div>         
    </div>
    <h1>Database</h1>  
    <div class="conteiner">
        <div class="element">
            <img :src="require(`@/assets/${postgresql}`)" alt="postgresql-logo">
        </div>
    </div>
    <h1>Frontend</h1>  
    <div class="conteiner">
        <div class="element">
            <img :src="require(`@/assets/${react}`)" alt="react-native-logo">
            <p>React Native</p>
        </div>
    </div>
    <h1>Web</h1>  
    <div class="conteiner">
        <div class="element">
            <img :src="require(`@/assets/${vue}`)" alt="vue-logo">
            <p>Vue.js</p>
        </div>
    </div>
    <h1>Other</h1>
    <div class="conteiner">
        <div class="element">
            <img :src="require(`@/assets/${docker}`)" alt="docker-logo">
            <p>Docker</p>
        </div>
        <div class="element">
            <img :src="require(`@/assets/${github}`)" alt="github-logo">
            <p>Github</p>
        </div>                
    </div>
</template>

<script>
export default {
    data(){
        return{
            vue:"vue-logo.png",
            github:"github-logo.png",
            ror:"ror-logo.png",
            postgresql:"postgresql-logo.png",
            docker:"docker-logo.png",
            react:"react-native-logo.png"
        }
    }
}
</script>

<style scoped>
img{
    width:150px;
}
p{
    font-weight: 700;
}
.conteiner{
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}
.element{
    padding: 5px;
    margin:15px;
}
img{
    width: 220px;
    height: 200px;
}
</style>