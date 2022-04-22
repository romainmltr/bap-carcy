<script>
import axios from "axios";
import {onMounted} from "vue";

/*createApp(App).mount('#app')

const url ="https://localhost:8000/card"
const getCard = () =>{
  return axios.get(url) .then (response => {
    let image = response.data.message;
    document.getElementById("image").src=image;
  })
}
document.querySelector('#app).innerHTML = `<img src =''

getCard();*/

onMounted(() => {
  const card = axios.get('https://localhost:8000/card')
  console.log(card);
})



</script>

<template>
  <div>
    <a>QR Code</a>
    <a href="file.doc">Download!</a>
  </div>

  <input v-model="message" placeholder="modifiez-moi">
  <p>Le message est : {{ message }}</p>

  <section class="testCard">
    <div class="test">
      <input v-model="message" placeholder="modifiez-moi">
      <p>Le message est : {{ message }}</p>
    </div>
  </section>
</template>

<style lang="scss" rel="stylesheet/scss">

</style>
