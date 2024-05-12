<template>
  <div class="main">
    <label>Login</label>
    <input :value="login" aria-label="www"/>
    <label>Password</label>
    <input :value="password" aria-label="www"/>
    <button @click="click">Sign up</button>
  </div>
</template>

<script setup lang="ts">
import {ref} from "vue";

const login = ref('')
const password = ref('')

const click = () => {
  console.log('CLICK!')
}
</script>

<style scoped>
.main {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-items: center;
}
</style>
