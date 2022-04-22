<script setup>
//import WelcomeItem from './components/WelcomeItem'
import axios from "axios";
import {onMounted} from "vue";
const urlCard = "https://localhost:8000/card"
fetch(`${urlCard}` )
    .then(function(response) {
      return response.json();
    })
    .then(function(data) {
      console.log(data);
    });

  function test(){
    const card = axios.get('https://localhost:8000/card')
    console.log(card)
  }

  test();
</script>

<template>
</template>

<style lang="scss">
@import './assets/_mixin.scss';

#app {
  margin: 0 auto;
  padding: 0rem;
  font-weight: normal;
  }
</style>

