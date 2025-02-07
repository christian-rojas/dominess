<template>
  <section class="business-services">
    <div class="about-section">
      <div class="about-image">
        <img src="/images/consultancy.jpg" alt="Business Consulting" />
      </div>
      <div class="about-content">
        <span class="section-tag">Sobre Nosotros</span>
        <h2>Consultores de confianza</h2>
        <p>
          Somos una firma consultora especializada en ayudar a empresas a alcanzar su máximo potencial. Nuestro equipo
          de expertos combina conocimiento industrial y tecnología de vanguardia para ofrecer soluciones personalizadas
          que impulsan el crecimiento de su negocio.
        </p>
        <!-- <NuxtLink to="/about" class="about-button">Conoce Más</NuxtLink> -->
      </div>
    </div>

    <div class="services-container">
      <div class="services-header">
        <span class="section-tag">Nuestros Servicios</span>
        <h2>Servicios de Consultoría que Ofrecemos</h2>
        <p>
          Nuestros consultores expertos combinan conocimiento industrial y tecnología innovadora para guiarlo hacia un
          futuro más brillante.
        </p>
      </div>

      <div class="services-grid">
        <div class="service-card">
          <div class="service-icon">
            <i class="fas fa-chart-line"></i>
          </div>
          <h3>Consultoría Estratégica</h3>
          <p>Desarrollamos planes estratégicos para impulsar el crecimiento empresarial y mejorar operaciones.</p>
          <a href="#" class="service-link">Leer Más →</a>
        </div>

        <!-- <div class="service-card highlight">
          <div class="service-icon">
            <i class="fas fa-bullhorn"></i>
          </div>
          <h3>Consultoría de Marketing</h3>
          <p>Estrategias de marketing efectivas para mejorar su presencia en el mercado y atraer clientes.</p>
          <a href="#" class="service-link">Leer Más →</a>
        </div> -->

        <div class="service-card">
          <div class="service-icon">
            <i class="fas fa-calculator"></i>
          </div>
          <h3>Consultoría Financiera</h3>
          <p>Análisis financiero, presupuestos y pronósticos para optimizar su rendimiento.</p>
          <a href="#" class="service-link">Leer Más →</a>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.business-services {
  padding: 4rem 2rem;
  background-color: #fff;
}

.about-section {
  display: flex;
  max-width: 1200px;
  margin: 0 auto;
  gap: 4rem;
  align-items: center;
  margin-bottom: 6rem;
}

.about-image {
  flex: 1;
}

.about-image img {
  width: 100%;
  border-radius: 20px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
}

.about-content {
  flex: 1;
}

.section-tag {
  background-color: #e6f0ff;
  color: #0066cc;
  padding: 0.5rem 1rem;
  border-radius: 20px;
  font-size: 0.9rem;
  font-weight: 500;
}

.about-content h2 {
  font-size: 2.5rem;
  color: #1a1a1a;
  margin: 1rem 0;
  line-height: 1.2;
}

.about-content p {
  color: #666;
  margin-bottom: 2rem;
  line-height: 1.6;
}

.about-button {
  display: inline-block;
  padding: 1rem 2rem;
  background-color: #0066cc;
  color: white;
  text-decoration: none;
  border-radius: 8px;
  font-weight: 600;
  transition: all 0.3s ease;
}

.about-button:hover {
  background-color: #0052a3;
  transform: translateY(-2px);
}

.services-container {
  max-width: 1200px;
  margin: 0 auto;
}

.services-header {
  text-align: center;
  margin-bottom: 4rem;
}

.services-header h2 {
  font-size: 2.5rem;
  color: #1a1a1a;
  margin: 1rem 0;
}

.services-header p {
  color: #666;
  max-width: 600px;
  margin: 0 auto;
}

.services-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
}

.service-card {
  background-color: #f8f9fa;
  padding: 2rem;
  border-radius: 15px;
  transition: all 0.3s ease;
}

.service-card.highlight {
  background-color: #0066cc;
  color: white;
}

.service-card.highlight h3,
.service-card.highlight p,
.service-card.highlight .service-link {
  color: white;
}

.service-icon {
  font-size: 2rem;
  color: #0066cc;
  margin-bottom: 1rem;
}

.service-card.highlight .service-icon {
  color: white;
}

.service-card h3 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #1a1a1a;
}

.service-card p {
  color: #666;
  margin-bottom: 1.5rem;
  line-height: 1.6;
}

.service-link {
  color: #0066cc;
  text-decoration: none;
  font-weight: 500;
}

@media (max-width: 968px) {
  .about-section {
    flex-direction: column;
    gap: 2rem;
  }

  .services-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 768px) {
  .services-grid {
    grid-template-columns: 1fr;
  }
}
</style>
