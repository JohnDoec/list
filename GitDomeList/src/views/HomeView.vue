<template>
  <main>
    <h2>TS 泛型的应用2024年9月6日23:01:17</h2>
    {{ car }}

  </main>
</template>



<script setup lang="ts">
import { reactive } from 'vue'


let car = reactive({ baoma: '宝马' });

function student<T, T>(value: T, message: T) {
  console.log(message)
  return value;
}

console.log(student<number, string>(68, '小明'))

</script>
