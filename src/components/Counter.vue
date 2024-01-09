<template>
  <div :style="[styleObj, { backgroundColor: ['blue', 'yellow', 'pink'] }]">
    Hi i am Niladri
  </div>
</template>

<script setup>

import { computed, reactive, ref } from "vue"

const color = ref("red");
const fontSize = ref(40);

const styleObj = computed(() => {
  return {
    color: color.value,
    fontSize: fontSize.value + 'px'
  }
})

setTimeout(() => {
  color.value = 'blue';
},2000)

</script>
