<template>
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
            github:"github-logo.png"
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
</style>