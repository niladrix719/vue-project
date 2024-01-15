<template>
  <div :class="{[myStyle]: isTrue}">Hello World</div>
  <!-- <Counter class="upper" greet="Hi i am Niladri" /> -->
</template>

<script setup>
const myStyle = 'nice';
const isTrue = true;
</script>
