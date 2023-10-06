<!-- src/components/Header.vue -->
<template>
  <div class="home">
    <h1 class="title"> Welcome to the IE Bank Server </h1>
    <h2 class="subtitle"> Please Select </h2>
    <h3 class="subtitle"> Ana Sauras </h3>
    <div class="button-container">
      <router-link to="/skull" class="button">Skull</router-link>
      <router-link to="/accounts" class="button">Accounts</router-link>
      <img src="../assets/IE-University-logo.png" alt="IE Logo" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomePage'
}
</script>

<style scoped>
html, body{
  margin: 0;
  padding: 0;
  height: 100%;
}

.home {
  background-image: url("../assets/ie-tower_9.png");
  background-size: cover;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.title {
  color: white;
  font-size: 3rem;
  margin-bottom: 2rem;
  font-family: 'Georgia', sans-serif;  
  background-color:  grey; 
  border-radius: 10px; 
  padding: 0.5rem 1rem; 
  animation: bounce 1s infinite;
}

.subtitle {
  color: white;
  font-size: 2rem;
  margin-bottom: 1rem;
  font-family: 'Georgia', sans-serif; 
  background-color: grey; 
  border-radius: 10px; 
  padding: 0.5rem 1rem; 
  animation: bounce 1s infinite;
}

@keyframes bounce {
  0% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
  100% {
    transform: translateY(0);
  }
}

.button-container {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: 2rem;
}

.button {
  background-color: white;
  color: black;
  border: none;
  padding: 1rem 2rem;
  margin: 0 1rem;
  border-radius: 5px;
  font-size: 1.4rem;
  font-family: 'Copperplate Gothic Bold', sans-serif;
  text-decoration: none;
  cursor: pointer;
}

.button:hover {
  background-color: blue;
  color: white;
}

img {
  width: 100px;
  height: 100px;
  margin: 100px 0 0 100px;
  position: absolute; 
  top: 0; 
  left: 0;
}

</style>
  