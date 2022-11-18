<template>
    <div class="content">
        <div v-for="p in people" :key="p.name" class="card">
            <p class="name">{{p.fname}}<br>{{p.lname}}</p>
            <img :src="require(`@/assets/${p.icon}`)" class="icon" alt=""/>
            <p class="job">{{p.job}}</p>
            <p class="gh">
                <svg xmlns="http://www.w3.org/2000/svg" width="18" height="18" fill="currentColor" class="bi bi-github" viewBox="0 0 16 16">
                    <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
                </svg>
                <a :href="`https://github.com/${p.github}`" target="_blank">@{{p.github}}</a></p>
        </div>
    </div>
</template>

<script>
export default {
    data(){
        return{
            people:[
                {fname:"Agnieszka",lname:"Piszcz",icon:"photo.png",job:"Project Manager",github:"AgnieszkaPiszcz"},
                {fname:"Mikołaj",lname:"Czurłowski",icon:"photo.png",job:"Fullstack Developer",github:"mikolajczu"},
                {fname:"Mateusz",lname:"Różański",icon:"photo.png",job:"Backend Developer",github:"matthewrosse"},
                {fname:"Damian",lname:"Maza",icon:"photo.png",job:"Frontend Developer",github:"x4trm"},
            ]
        }
    }
}
</script>

<style>
svg{
    vertical-align: middle;
    margin-right: 4px;
}
.job,.gh{
    font-size:18px;
    color:#2c3e50;
}
.name{
    color: #41b883;
    padding:10px;
    font-size:30px;
    font-weight: 700;
}
.icon{
    width:150px;
    height:150px;
    border-radius: 50%;
}
.content{
    height:700px;
    padding:20px;
    margin:20px 10px;
    display: flex;
    justify-content: center;
    flex-wrap:wrap;
}
.card{
    
    border-radius:20px;
    background-color:white;
    height: 450px;
    width: 300px;
    padding:20px;
    margin: 20px;
}
</style>