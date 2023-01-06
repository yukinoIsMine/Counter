<template>
  <main>
    <div>
      <h1>Mizu The Counter</h1>
      <p>{{count}}</p>
      <button @click="count--">-</button>
      <button @click="count++">+</button>
      <button id="restart" @click="count=0">Restart</button>
    </div>
  </main>
</template>

<script setup>
import { ref } from 'vue';
let count = ref(0);
</script>

<style scoped>
main{
  height: 100vh;
  width: 100vw;
  background-color: rgb(10, 10, 58);
  display: flex;
  justify-content: center;
  align-items: center;
}

div{
  text-align: center;
  border : 1px solid aliceblue;
  padding: 20px;
}

h1{
  color: aliceblue;
  margin: 10px;
  font-size: 60px;
}

p{
  color: aliceblue;
  font-size: 30px;
  margin-bottom: 20px;
}

button{
  background-color: rgb(10, 10, 58);
  outline: none;
  border: 1px solid aliceblue;
  color: aliceblue;
  font-size: 50px;
  width: 50%;
  transition: 0.3s;
}

button:hover {
  background-color: aliceblue;
  color: rgb(10, 10, 58);
}

#restart{
  font-size: 20px;
  margin-top: 10px;
  border-radius: 50%;
  width: 70px;
  height: 70px;
}
</style>