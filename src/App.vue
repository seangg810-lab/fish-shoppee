<template>
  <div class="login-container">
    <LoginHeader />
    <LoginForm />
    <RegisterLink />
  </div>
</template>

<script setup>
import LoginHeader from './components/LoginHeader.vue'
import LoginForm from './components/LoginForm.vue'
import RegisterLink from './components/RegisterLink.vue'
</script>

<style>
body {
  margin: 0;
  padding: 0;
  background-color: #f5f5f5;
  font-family: -apple-system, Helvetica Neue, Helvetica, Roboto, Arial, sans-serif;
}
</style>

<style scoped>
.login-container {
  width: 400px;
  margin: 50px auto;
  padding: 30px;
  background-color: white;
  border-radius: 4px;
  box-shadow: 0 3px 10px rgba(0,0,0,0.1);
}
</style>