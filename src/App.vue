<script setup lang="ts">
</script>

<template>
  <div class="container">
    <a href="https://adereso.ai" target="_blank" class="logo-link">
      <img src="/Adereso_Blanco.png" alt="Adereso" class="logo">
    </a>
    
    <div class="card-container">
      <h2>Explora nuestras soluciones de IA personalizadas para cada industria</h2>
      <p class="subtitle">Descubre cómo nuestros bots de IA pueden transformar tu industria</p>
      
      <div class="buttons-grid">
        <a href="https://wa.me/+56949403837" target="_blank" class="button">Automotora</a>
        <a href="https://api.whatsapp.com/send/?phone=56935055832&text&app_absent=0" target="_blank" class="button">Utilities</a>
        <a href="https://api.whatsapp.com/send?phone=56944154087&text=%C2%A1Hola!%20Necesito%20ayuda%20" target="_blank" class="button">Retail</a>
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
}

.container > * {
  position: relative;
  z-index: 2;
}

.logo-link {
  display: block;
  margin-bottom: 3rem;
  transition: opacity 0.3s ease;
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
}

h2 {
  font-size: 1.75rem;
  font-weight: 700;
  color: white;
  margin: 0 0 1rem 0;
  text-align: center;
  line-height: 1.5;
}

.subtitle {
  font-size: 0.875rem;
  color: rgba(255, 255, 255, 0.7);
  margin: 0 0 2.5rem 0;
  text-align: center;
  line-height: 1.4;
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
    padding-top: 3rem;
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
  
  h2 {
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
    gap: 1.3rem;
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
    padding: 3rem 0 2rem 0;
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
  
  h2 {
    font-size: 1.4rem;
    margin: 0 0 1rem 0;
    line-height: 1.4;
  }
  
  .subtitle {
    font-size: 0.875rem;
    margin: 0 0 2.5rem 0;
    line-height: 1.4;
  }
  
  .buttons-grid {
    gap: 1.4rem;
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
    padding: 2.5rem 0 1.5rem 0;
  }
  
  .logo {
    height: 40px;
  }
  
  .card-container {
    max-width: 320px;
    padding: 2rem 1.2rem;
    margin: 0 0.8rem;
  }
  
  h2 {
    font-size: 1.125rem;
  }
  
  .subtitle {
    font-size: 0.8rem;
    margin: 0 0 2rem 0;
  }
  
  .buttons-grid {
    gap: 1.2rem;
  }
  
  .button {
    padding: 1rem 1.2rem;
    font-size: 0.95rem;
  }
}
</style>
