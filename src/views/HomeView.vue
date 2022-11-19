<template>
  <h1>Sentakki</h1>
  <div class="main">
    <img :src="require(`@/assets/${logo}`)" alt="logo">
    <div class="content">
        <p>Sentakki w języku japońskim oznacza pralkę. Zespół programistów z <a href="https://www.fizyka.umk.pl/" target="_blank">Wydziału Fizyki, Astronomii i Informatyki Stosowanej</a> podjął się stworzenia 
            systemu zarządzania pralniami w akademikach
 <a href="https://www.umk.pl/" target="_blank">Uniwersytetu Mikołaja Kopernika</a> w Toruniu. Projekt jest realizowany w ramach przedmiotu Programowanie Zespołowe.</p>
    </div>
</div>
  </template>

<script>
export default {
    data(){
        return{
            logo:"logo.png",
        }
    }
}
</script>

<style>
img{
    width:350px;

}
.main{
    max-width: 50em;
	margin: 0 auto;
}
.content{
	margin: 6px;
    font-size:1rem;
}
a{
    text-decoration: none;
    color:#41b883;
}
h1{
    margin-top:30px;
    font-size:3rem;
}
p{
    margin-top:5px;
    font-size: 1.75em;
}
</style>