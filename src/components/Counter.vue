<template>
  <div>
    <button @click="incr()">+</button>
    {{ count }}
    <button @click="decr()">-</button>
    <div v-bind="attr" :[attrTitle]="ti" v-html="name"></div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const count = ref(0);
const name = "<h1>Niladri</h1>";
const vue_id = "vue-id";
const ti = "this title"
const attrTitle = "title";
const attr = {
  id: "this id",
  class: "this class"
}

function incr() {
  count.value++;
}

function decr() {
  count.value--;
}
</script>