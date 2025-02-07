<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="footer-logo">
        <h2>Dominess</h2>
        <p>Transformando negocios con soluciones efectivas</p>
      </div>
      <div class="footer-links">
        <div class="link-group">
          <h3>Servicios</h3>
          <ul>
            <li><a href="#">Consultoría Estratégica</a></li>
            <li><a href="#">Asesoría Empresarial</a></li>
            <li><a href="#">Optimización de Procesos</a></li>
          </ul>
        </div>
        <div class="link-group">
          <h3>Contacto</h3>
          <ul>
            <li>contacto@dominess.com</li>
            <li>Santiago, Chile</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <p>&copy; 2025 Dominess. Todos los derechos reservados.</p>
    </div>
  </footer>
</template>

<style scoped>
.footer {
  background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
  box-shadow: 0 -2px 4px rgba(0, 0, 0, 0.1);
  padding: 3rem 2rem 1rem;
  font-family: "Poppins", sans-serif;
}

.footer-content {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  gap: 4rem;
}

.footer-logo h2 {
  color: #ffffff;
  margin: 0;
  font-size: 2rem;
  margin-bottom: 1rem;
  font-family: "Montserrat", sans-serif;
  font-weight: 700;
  letter-spacing: -0.5px;
}

.footer-logo p {
  color: #e0e0e0;
  max-width: 300px;
  font-size: 1.1rem;
  line-height: 1.6;
}

.footer-links {
  display: flex;
  gap: 4rem;
}

.link-group h3 {
  color: #ffffff;
  font-size: 1.2rem;
  margin-bottom: 1.2rem;
  font-family: "Montserrat", sans-serif;
  font-weight: 600;
  position: relative;
}

.link-group h3::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -8px;
  width: 40px;
  height: 3px;
  background: #4caf50;
  border-radius: 2px;
}

.link-group ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.link-group ul li {
  margin-bottom: 0.8rem;
}

.link-group ul li a {
  color: #e0e0e0;
  text-decoration: none;
  transition: all 0.3s ease;
  font-size: 1rem;
  position: relative;
}

.link-group ul li a:hover {
  color: #4caf50;
  padding-left: 5px;
}

.link-group ul li {
  color: #e0e0e0;
}

.footer-bottom {
  max-width: 1200px;
  margin: 2rem auto 0;
  padding-top: 2rem;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
  text-align: center;
  color: #e0e0e0;
  font-size: 0.9rem;
}

@media (max-width: 768px) {
  .footer-content {
    flex-direction: column;
    gap: 2rem;
  }

  .footer-links {
    flex-direction: column;
    gap: 2rem;
  }
}
</style>
