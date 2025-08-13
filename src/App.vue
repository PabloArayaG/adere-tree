<script setup lang="ts">
</script>

<template>
  <div class="container">
    <a href="https://adereso.ai" target="_blank" class="logo-link">
      <img src="/Adereso_Blanco.png" alt="Adereso" class="logo">
    </a>
    
    <div class="card-container">
      <h1>Prueba los Agentes IA que están transformando el CX en tu industria</h1>
      <p class="subtitle">Chatea con los bots de empresas similares a la tuya y experimenta el potencial de tu CX</p>
      
              <div class="buttons-grid">
          <a href="https://adereso.ai/contacto-wbl" target="_blank" class="button">Agendar reunión</a>
          <a href="https://wa.me/+56941581023" target="_blank" class="button">Automotora</a>
          <a href="https://api.whatsapp.com/send/?phone=56935055832&text&app_absent=0" target="_blank" class="button">Utilities</a>
          <a href="https://api.whatsapp.com/send?phone=56944154087&text=%C2%A1Hola!%20Necesito%20ayuda%20" target="_blank" class="button">Retail</a>
          <a href="https://genianew.adereso.ai" target="_blank" class="button">Ver GenIA</a>
        </div>
    </div>
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
}

html, body {
  height: 100%;
  width: 100%;
  overflow-x: hidden;
  background-color: #131415;
  position: relative;
}

body::before {
  content: '';
  position: fixed;
  top: -30%;
  left: -50%;
  width: 200%;
  height: 200%;
  background-image: url('/Degradados-16.png');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  opacity: 0.3;
  filter: blur(20px);
  z-index: 1;
}

#app {
  width: 100vw;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

.container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 2rem;
  position: relative;
  z-index: 5;
  opacity: 0;
  animation: fadeIn 0.6s ease-out forwards;
}

.container > * {
  position: relative;
  z-index: 2;
}

.logo-link {
  display: block;
  margin-bottom: 3rem;
  transition: opacity 0.3s ease;
  opacity: 0;
  animation: fadeInScale 0.6s ease-out 0.2s forwards;
}

.logo-link:hover {
  opacity: 0.8;
}

.logo {
  height: 60px;
  width: auto;
}

.card-container {
  background: rgba(19, 20, 21, 0.8);
  backdrop-filter: blur(20px);
  border-radius: 24px;
  padding: 3rem 2.5rem;
  max-width: 600px;
  border: 1px solid rgba(255, 255, 255, 0.1);
  box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
  opacity: 0;
  transform: translateY(30px);
  animation: slideInUp 0.8s ease-out 0.4s forwards;
}

h1 {
  font-size: 1.75rem;
  font-weight: 700;
  color: white;
  margin: 0 0 1rem 0;
  text-align: center;
  line-height: 1.5;
  opacity: 0;
  transform: translateY(20px);
  animation: slideInUp 0.8s ease-out 0.6s forwards;
}

.subtitle {
  font-size: 0.875rem;
  color: rgba(255, 255, 255, 0.7);
  margin: 0 0 2.5rem 0;
  text-align: center;
  line-height: 1.4;
  opacity: 0;
  transform: translateY(20px);
  animation: slideInUp 0.8s ease-out 0.7s forwards;
}

.buttons-grid {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.button {
  display: block;
  width: 100%;
  padding: 1.2rem 2rem;
  background-color: #1864FF;
  color: white;
  text-decoration: none;
  border-radius: 16px;
  font-size: 1.1rem;
  font-weight: 600;
  text-align: center;
  box-shadow: 0 4px 15px rgba(24, 100, 255, 0.3);
  transition: all 0.3s ease;
  opacity: 0;
  transform: translateY(20px);
}

.button:nth-child(1) {
  animation: buttonSlideIn 0.6s ease-out 0.8s forwards;
  background-color: white;
  color: #131415;
  box-shadow: 0 4px 15px rgba(255, 255, 255, 0.2);
}

.button:nth-child(1):hover {
  background-color: #f0f0f0;
  color: #131415;
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(255, 255, 255, 0.3);
}

.button:nth-child(2) {
  animation: buttonSlideIn 0.6s ease-out 1s forwards;
}

.button:nth-child(3) {
  animation: buttonSlideIn 0.6s ease-out 1.2s forwards;
}

.button:nth-child(4) {
  animation: buttonSlideIn 0.6s ease-out 1.4s forwards;
}

.button:nth-child(5) {
  animation: buttonSlideIn 0.6s ease-out 1.6s forwards;
}



.button:hover {
  background-color: #1450D9;
  color: white;
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(24, 100, 255, 0.4);
}

/* Responsive */
@media (max-width: 768px) and (min-width: 481px) {
  #app {
    align-items: flex-start;
    padding: 3rem 0 6rem 0;
}
  
  .logo {
    height: 45px;
  }
  
  .logo-link {
    margin-bottom: 1.5rem;
  }
  
  .card-container {
    max-width: 500px;
    padding: 2rem 1.8rem;
    margin: 0 1.5rem;
  }
  
  h1 {
    font-size: 1.375rem;
    margin: 0 0 0.9rem 0;
  }
  
  .subtitle {
    font-size: 0.875rem;
  }
  
  .subtitle {
    margin: 0 0 2rem 0;
  }
  
  .buttons-grid {
    gap: 1.2rem;
  }
  
  .button {
    padding: 1rem 1.8rem;
    font-size: 1.05rem;
  }
  
  .container {
    gap: 1.3rem;
    padding: 0;
  }
}

@media (max-width: 480px) {
  #app {
    align-items: flex-start;
    padding: 3rem 0 6rem 0;
  }
  
  .logo {
    height: 45px;
  }
  
  .logo-link {
    margin-bottom: 2rem;
  }
  
  .card-container {
    max-width: 350px;
    padding: 2.5rem 1.5rem;
    margin: 0 1rem;
  }
  
  h1 {
    font-size: 1.4rem;
    margin: 0 0 1rem 0;
    line-height: 1.4;
  }
  
  .subtitle {
    font-size: 0.875rem;
    margin: 0 0 2.2rem 0;
    line-height: 1.4;
  }
  
  .buttons-grid {
    gap: 1.3rem;
  }
  
  .button {
    padding: 1.1rem 1.5rem;
    font-size: 1rem;
  }
  
  .container {
    gap: 1.5rem;
    padding: 0;
  }
}

@media (max-width: 360px) {
  #app {
    padding: 2.5rem 0 5.5rem 0;
  }
  
  .logo {
    height: 40px;
  }
  
  .card-container {
    max-width: 320px;
    padding: 2rem 1.2rem 2.5rem 1.2rem;
    margin: 0 0.8rem;
  }
  
  h1 {
    font-size: 1.125rem;
  }
  
  .subtitle {
    font-size: 0.8rem;
    margin: 0 0 2rem 0;
  }
  
  .buttons-grid {
    gap: 1.1rem;
  }
  
  .button {
    padding: 1rem 1.2rem;
    font-size: 0.95rem;
  }
}

/* Animaciones */
@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes fadeInScale {
  from {
    opacity: 0;
    transform: scale(0.9);
  }
  to {
    opacity: 1;
    transform: scale(1);
  }
}

@keyframes slideInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes buttonSlideIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
