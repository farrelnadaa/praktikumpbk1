<!-- src/App.vue -->
<script setup>
import Biodata from './components/Biodata.vue'
</script>

<template>
  <div class="app-container">
    <div class="personal-photo-container">
      <img src="./assets/Gambar WhatsApp 2024-06-09 pukul 00.12.23_0f63f046.jpg" class="personal-photo" alt="Personal Photo" />
    </div>
    <Biodata 
      name="MUHAMMAD FARREL ANANDA PUTRA" 
      :age="20" 
      location="PEKANBARU, RIAU" 
      profession="Software Developer" 
      Hobies="Play games"
      Social Media="Farrelnadaa"
    />
  </div>
</template>

<style scoped>
.app-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  background: linear-gradient(135deg, #525354, #434547, #444648);
  padding: 20px;
  box-sizing: border-box;
}

.personal-photo-container {
  margin-bottom: 20px;
}

.personal-photo {
  height: 150px;
  width: 150px;
  border-radius: 50%;
  object-fit: cover;
  border: 4px solid #1e201f;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.personal-photo:hover {
  transform: scale(1.1);
  box-shadow: 0 0 15px rgba(36, 38, 37, 0.7);
}

.biodata {
  background: #ffffff;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  text-align: center;
  max-width: 300px;
}

.biodata h2 {
  margin: 0;
  color: #191c1b;
  font-size: 24px;
}

.biodata p {
  margin: 10px 0;
  font-size: 16px;
  color: #333;
}
</style>
