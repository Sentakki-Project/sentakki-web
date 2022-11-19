<template>
  <div class="content">
    <div v-for="i in info" :key="i.name" class="card">
        <p class="name">{{i.name}}</p>
        <p class="date">{{i.date}}</p>
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return{
            info:[
                {name:"Utworzenie Systemu Logowania i Rejestracji",date:"Grudzień 2022"},
                {name:"Utworzenie Modeli Bazodanowych",date:"Listopad 2022"},
                {name:"Utworzenie Strony Internetowej",date:"Listopad 2022"},
                {name:"Badanie Potrzeb Rynkowych",date:"Listopad 2022"},
                {name:"Pomysł Projektu",date:"Październik 2022"}
            ],
        }
    }
}
</script>

<style scoped>
.content{
    height:700px;
    padding:20px;
    margin:20px 10px;
    display: flex;
    justify-content: center;
    flex-wrap:wrap;
}
.card{
    border-radius:40px;
    background-color: white;
    width:300px;
    height:200px;
    margin:20px;
} 
.name{
    color: #41b883;
    padding:10px;
    font-size:21px;
    font-weight: 700;
}
.date{
    
    font-size:18px;
    color:#2c3e50;
}
</style>