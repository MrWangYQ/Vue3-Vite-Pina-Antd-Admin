<script setup>
import { ref } from 'vue'
import TheWelcome from '../components/TheWelcome.vue'

const input = ref('')
const input2 = ref('')

</script>

<template lang="pug">
main
  //- TheWelcome
  div
    | {{ input }}
    a-input(id="input" v-model:value="input" placeholder="请输入文本")
    a-input(id="input1" v-model:value="input2" placeholder="请输入文本")
</template>
