

<script setup> 
import { ref } from 'vue';

const count = ref(0)
 const addToCount = () => {
  console.log("add to count")
  count.value = count.value + 1
 }

 const subtractFromCount = () => {
  count.value = count.value - 1
 }


// import { ref } from 'vue'
//   export default({
//     data(){
//       return {
//       count: 0
//       }
//     },
//       methods: {
//         addToCount(){
//           this.count = this.count + 1
//         },
//         subtractFromCount(){
//           this.count = this.count - 1
//         }
//       }

//   })
</script>

<template>
 <main>
  <div class="main">
    <h4>the the current count is.... </h4>
    <h1> {{ count }} </h1>
    <button @click="subtractFromCount()">-</button>
    <button @click="addToCount()">+</button>
  </div>
 </main>
</template>

<style scoped>

main {
  width: 100vw;
  height: 100vh;
  background-color: lightblue;
  display: flex;
  align-items: center;
  justify-content: center;
}
 .main {
  text-align: center;
 }

 h4 {
  font-size: 1.5em;
  font-weight: bold ;
 }
</style>