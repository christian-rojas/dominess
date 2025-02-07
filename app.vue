<template>
  <div class="landing-container">
    <nav class="navbar">
      <div class="logo">
        <h1>Dominess</h1>
      </div>
    </nav>

    <main class="hero-section">
      <div class="hero-content">
        <h1>No pierdas<br /><span class="highlight">Negocios</span><br />de nuevo</h1>
        <p class="subtitle">Asesorate con nosotros</p>
        <NuxtLink to="https://kindap.youcanbook.me" class="booking-button"> AGENDAR </NuxtLink>
      </div>
      <div class="hero-image">
        <img src="/images/calendar-app.jpg" alt="Calendar App Preview" />
      </div>

      <div class="features-section">
        <div class="feature">
          <h2>Agenda gratis</h2>
          <p>Selecciona el día y hora de tu preferencia.</p>
          <!-- <a href="https://kindap.youcanbook.me">Agenda ya</a> -->
        </div>
      </div>

      <BusinessServices />
    </main>
    <AppFooter />
  </div>
</template>

<script setup lang="ts">
import BusinessServices from "@/components/BusinessServices.vue";
import AppFooter from "@/components/AppFooter.vue";

defineComponent({
  components: {
    BusinessServices,
    AppFooter,
  },
});
</script>

<style scoped>
.landing-container {
  min-height: 100vh;
  background: linear-gradient(135deg, #ffffff 0%, #f5f5f5 100%);
}

.navbar {
  padding: 1.5rem 2rem;
  background-color: white;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.logo h1 {
  color: #0066cc;
  margin: 0;
  font-size: 1.5rem;
}

.hero-section {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 4rem 2rem;
  max-width: 1200px;
  margin: 0 auto;
  gap: 2rem;
}

.hero-content {
  flex: 1;
}

.hero-content h1 {
  font-size: 3.5rem;
  line-height: 1.2;
  margin-bottom: 1rem;
  color: #333;
}

.highlight {
  color: #0066cc;
  font-weight: bold;
}

.subtitle {
  font-size: 1.2rem;
  color: #666;
  margin-bottom: 2rem;
}

.booking-button {
  display: inline-block;
  padding: 1rem 2rem;
  background-color: #0066cc;
  color: white;
  text-decoration: none;
  border-radius: 8px;
  font-weight: 600;
  transition: background-color 0.3s ease;
}

.booking-button:hover {
  background-color: #0052a3;
}

.hero-image {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.hero-image img {
  max-width: 100%;
  height: auto;
  border-radius: 12px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
}

@media (max-width: 768px) {
  .hero-section {
    flex-direction: column;
    text-align: center;
    padding: 2rem 1rem;
  }

  .hero-content h1 {
    font-size: 2.5rem;
  }

  .hero-image {
    margin-top: 2rem;
  }
}
</style>
