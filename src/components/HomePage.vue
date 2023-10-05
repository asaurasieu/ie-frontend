<!-- src/components/Header.vue -->
<template>
    <header>
      <h1>My Homepage</h1>
        




      <nav>
        <router-link to="/skull">Skull</router-link>
        <router-link to="/accounts">Accounts</router-link>
        <!-- Add more navigation links here -->
      </nav>
    </header>
  </template>
  
  <script>
  export default {
    name: 'Header'
  }
  </script>
  
  <style scoped>
  /* Add CSS styles for your header here */
  </style>
  