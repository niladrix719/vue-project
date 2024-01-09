<template>
  <div>
    {{ count }}
   <button @click.stop.prevent="count = $event.target">press</button>
  </div>
</template>

<script setup>
import { computed, reactive, ref } from "vue"

const count = ref("Test");

</script>
