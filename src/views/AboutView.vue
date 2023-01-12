<template>
  <h1>Panel Administracyjny</h1>
  <div v-for="item in adminItems" :key="item.text">
    <li>{{ item.text }}</li>
  </div>
  <h1>Panel Użytkownika</h1>
  <div v-for="item in userItems" :key="item.text">
    <li>{{ item.text }}</li>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        tab: null,
        adminItems: [
          { text: 'Logowanie'},
          { text: 'podgląd stanu rezerwacji pralek'},
          { text: 'ustawienie godzin otwarcia pralni'},
          { text: 'ustawienie liczby dostępnych pralek'},
          { text: 'ustawienie po ilu zarezerwowanych, ale niewykorzystanych praniach użytkownik zostanie zablokowany i na ile czasu'},
          { text: 'ustawienie ile czasu przed można odwołać pranie'},
          { text: 'ustawienie maksymalnej liczby aktywnych rezerwacji na użytkownika'},
          { text: 'edytowanie rezerwacji'},
        ],
        userItems:[
        { text: 'logowanie kontem USOS'},
        { text: 'wybór akademika'},
        { text: 'podgląd stanu rezerwacji pralek'},
        { text: 'rezerwacja slotu na pralkę'},
        { text: 'podgląd rezerwacji użytkownika'},
        { text: 'anulowanie rezerwacji'},
        { text: 'powiadomienie poprzedniego użytkownika pralki by wyjął rzeczy'},
        { text: 'otrzymanie powiadomienia o tym że skończyło się pranie'},
        { text: 'płatność za pranie'},
        ]
      }
    },
  }
</script>
<style scoped>

h1{
  font-size:35px;
}
li{
  font-size:20px;
}
</style>