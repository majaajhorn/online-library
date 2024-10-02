<template>
    <div class="register">
      <h2>Register</h2>
      <form @submit.prevent="handleRegister">
        <div>
          <label for="username">Username:</label>
          <input type="text" v-model="username" required />
        </div>
        <div>
          <label for="email">Email:</label>
          <input type="email" v-model="email" required />
        </div>
        <div>
          <label for="password">Password:</label>
          <input type="password" v-model="password" required />
        </div>
        <button type="submit">Register</button>
      </form>
      <p>Already have an account? <router-link to="/login">Login here</router-link></p>
    </div>
  </template>
  
  <script>
  export default {
    name: 'UserRegister',
    data() {
      return {
        username: '',
        email: '',
        password: '',
      };
    },
    methods: {
      handleRegister() {
        // Implement registration logic here
        console.log('Register:', this.username, this.email, this.password);
      },
    },
  };
  </script>
  
  <style scoped>
  .register {
    text-align: center;
    margin-top: 50px;
  }
  </style>
  