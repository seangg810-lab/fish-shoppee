<template>
  <form class="login-form" @submit.prevent="handleSubmit">
    <div class="input-group">
      <input
        v-model="username"
        type="text"
        placeholder="電話號碼 / 使用者名稱 / 電子郵件"
      />
    </div>

    <div class="input-group">
      <input
        v-model="password"
        type="password"
        placeholder="密碼"
      />
    </div>

    <button type="submit" class="login-btn">
      登入
    </button>
  </form>
</template>

<script setup>
import { ref } from 'vue'

const username = ref('')
const password = ref('')

const handleSubmit = () => {
  console.log('Logging in with:', username.value, password.value)
  // Add login logic here
}
</script>

<style scoped>
.login-form {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.input-group input {
  width: 100%;
  padding: 12px;
  border: 1px solid #dbdbdb;
  border-radius: 2px;
  box-sizing: border-box;
}

.input-group input:focus {
  outline: none;
  border-color: #ee4d2d;
}

.login-btn {
  background-color: #ee4d2d;
  color: white;
  border: none;
  padding: 12px;
  border-radius: 2px;
  cursor: pointer;
  font-size: 14px;
  text-transform: uppercase;
  font-weight: 500;
}

.login-btn:hover {
  background-color: #f05d40;
}
</style>