<script setup>

</script>

<template>
  <div class="app">
    <div class="container">
    <h1>Wheater App</h1>
        <input type="text" id="search-input" placeholder="Ingresa un lugar">
        <button id="search-button">Buscar</button>
        <p id="city-element"></p>
        <div id="temperature-display"></div>
        <img id="weather-icon">
        <p id="city-time"></p>
        <p id="error"></p>
        <div id="additional-info"></div>
    </div>
  </div>
</template>

<style scoped>
.container{
  border-radius: 10px;
  padding: 30px;
  text-align: center;
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: 400px;
}
.app {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

h1 {
  font-size: 2em;
  margin-bottom: 20px;
}

#search-input {
  padding: 10px;
  font-size: 1em;
  width: 80%;
  border: 2px solid #ccc;
  border-radius: 5px;
  margin-bottom: 15px;
  transition: border-color 0.3s;
}

#search-input:focus {
  border-color: #3498db;
  outline: none;
}

#search-button {
  background-color: #3498db;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  font-size: 1em;
  cursor: pointer;
  transition: background-color 0.3s;
}

#search-button:hover {
  background-color: #2980b9;
}

#city-element, #city-time, #error, #additional-info {
  font-size: 1.2em;
  margin-top: 20px;
  color: #555;
}

#temperature-display {
  font-size: 2em;
  font-weight: bold;
  margin-top: 15px;
  color: #e74c3c;
}

#city-time {
  font-size: 1em;
  color: #7f8c8d;
}

#error {
  font-size: 1em;
  color: #e74c3c;
  margin-top: 20px;
}

#additional-info {
  margin-top: 20px;
}
</style>