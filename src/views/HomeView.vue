<script setup>
import TheWelcome from '../components/TheWelcome.vue'

</script>
<script>
import axios from "axios";

const options = {
  method: 'GET',
  url: 'https://the-sneaker-database.p.rapidapi.com/sneakers',
  params: {limit: '100'},
  headers: {
    'X-RapidAPI-Key': 'e73b51d1b1msh1d2a8c31ce46df0p109b0ejsn56d02db82093',
    'X-RapidAPI-Host': 'the-sneaker-database.p.rapidapi.com'
  }
};

axios.request(options).then(function (response) {
	console.log(response.data);
}).catch(function (error) {
	console.error(error);
});
console.log("kuy");
</script>
<template>
  <main>
    <TheWelcome />
  </main>
</template>
