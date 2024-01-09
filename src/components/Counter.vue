<template>
  <div>
   <ul>
    <li v-for="(x,k) in persons">
      {{ k }} - {{ x.name }}
    </li>
   </ul>
  </div>
</template>

<script setup>
import { computed, reactive, ref } from "vue"

const persons = reactive({
  team1: {
    name: "niladri"
  },
  team2: {
    name: "mouma"
  }
})

</script>
