<template>

  <div>
    {{ obj.val }}
    <button @click="obj.val++">Click</button>
    {{ obj.oj.first }}
    {{ greet }}
    <input type="text" v-model="obj.oj.first">
  </div>
  
</template>

<script setup>
import { computed, reactive, ref, watch } from "vue";

const obj = reactive({ val: 0, is: true, oj: { first: "first" , second: "second"} });

watch(() => obj.oj.first, (objNew) => {
  console.log(objNew);
})

defineProps({
  greet: String
})

</script>
