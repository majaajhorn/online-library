<template>
  <div class="home">
    <h1>Online Library</h1>
    <p>Welcome to the Online Library!</p>
    <router-link to="/login">Login</router-link> | 
    <router-link to="/register">Register</router-link>
  </div>
</template>

<script>
export default {
  name: 'Home',
}
</script>

<style scoped>
.home {
  text-align: center;
  margin-top: 50px;
}
</style>
