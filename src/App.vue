<<<<<<< HEAD
<template>
  <div>
    <button @click="increment">
      {{ count }}
    </button>
    <button @click="state.count++">
      {{ state.count }}
    </button>
    <button @click="counter++">Add 1</button>
    <p>The button above has been clicked {{ counter }} times.</p>
    <button @click="greet">Greet</button>
    <button @click="awesome = !awesome">toggle</button>
    <h1 v-if="awesome">Vue is awesome!</h1>
    <h1 v-else>Oh no 😢</h1>
  </div>
</template>

<script setup>
import { ref, reactive } from 'vue'

const count = ref(0)

function increment() {
  count.value++
}

const state = reactive({ count: 0 })

const counter = ref(0)

const name = ref('Vue.js')

function greet(event) {
  alert(`Hello ${name.value}!`)
  if (event) {
    alert(event.target.tagName)
  }
}

const awesome = ref(true)
</script>
=======
<script setup>
// 第一步：引入组件
import MyComponents from './components/MyComponents.vue';
</script>

<template>
  <!--第二步: 显示组件-->
  <MyComponents/>
</template>

<style scoped>

</style>
>>>>>>> a90c1cc982b9918260cdb2ad0c7242a8638b5fdb
