<template>

  <div>
    {{ obj.val }}
    <button @click="obj.val++">Click</button>
  </div>
  
</template>

<script setup>
import { computed, reactive, ref, watch } from "vue";

const obj = reactive({ val: 0, is: true, oj: { first: "first" , second: "second"} });

watch(obj.oj, (objNew) => {
  console.log(objNew.val);
})

</script>
