<div id="header" align="center">
  <h1>👋 Hola, soy Damián Gamboa</h1>
  <h3>QA Software Engineer</h3>
  <p>
    <a href="https://www.linkedin.com/in/damiangamboa/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
    <a href="mailto:damiangamboa5751@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  </p>
</div>

## 👨‍💻 Sobre mí

Tengo un amor genuino por el mundo del software y la automatización. Actualmente estoy en la etapa final de mi Ingeniería. Mi enfoque profesional va mucho más allá de asegurar la calidad de un release; me dedico a entender la lógica de negocio profunda de los productos (especialmente en ecosistemas logísticos y e-commerce) para construir soluciones y herramientas internas que contribuyan a validar la calidad de los mismos.

## 🛠️ Habilidades de QA

- **Quality Engineering & Análisis Crítico de Negocio:** Diseño y ejecución de estrategias de pruebas para tener cobertura total del producto, asegurando la integridad de datos desde la capa de servicios hasta el cliente final, mitigando riesgos financieros en producción.
- **Test Automation Architecture:** Construcción y despliegue de frameworks corporativos. Dominio de Playwright/JavaScript/Node.js para construcción de frameworks escalables en el ecosistema de Playwright. Gestión autónoma de repositorios y seguridad.
- **CI/CD:** Definición de estándares de calidad e integración de suites de automatización en pipelines de CI/CD (GitHub Actions/Git hooks) para establecer compuertas de seguridad antes de cualquier merge a producción.

## 💻 Stack Tecnológico

| Categoría | Tecnologías & Herramientas |
| :--- | :--- |
| **Test Automation** | *Playwright, JavaScript, Node.js, Custom Fixtures, POM* |
| **Backend & APIs** | *Postman, Swagger, REST APIs, Network Interception* |
| **Mobile & Debugging** | *Xcode, Android Studio, Proxyman, Sentry* |
| **CI/CD, DevOps & Security** | *GitHub Actions, Husky (Pre-commit/Pre-push Hooks), Multi-Environment Orchestration* |
| **Metodologías & Calidad** | *Zero-Flakiness, Shift-Left Testing, Idempotency Validations* |


## 📐 Core Automation Architecture & Shift-Left Integration

Construyo frameworks de alto rendimiento aplicando principios SOLID, minimizando la latencia de ejecución y garantizando casi un 0% flakiness a través del control absoluto del estado y la red.

- **State Persistence & Dynamic Auth Injection**: Abandono la autenticación basada en UI en favor de la manipulación directa del Browser Context. Implemento arquitecturas de Dual-Auth (Bypass vía peticiones POST a la API y persistencia SSO) para inyectar cookies y tokens directamente en el estado del navegador. Esto reduce el setup time de las suites y habilita ejecuciones de ultra-alta velocidad en pipelines.

- **Event-Driven Network Synchronization**: Reemplazo por completo los hard waits y la evaluación ciega del DOM. Diseño interceptores de red que condicionan los assertions del Frontend a la resolución exitosa (HTTP 200 OK) del Backend. Implemento listeners asíncronos para capturar promesas fallidas y errores silenciosos (HTTP 5xx) en segundo plano, logrando aislar si la causa raíz de un bug pertenece a la capa de servicios o del Frontend.

- **Fail-Fast Orchestration & Pre-flight Checks**: Orquestación centralizada mediante Global Setups que evalúan dinámicamente la salud de los endpoints críticos y la validez de los objetos de sesión antes de instanciar los workers. Si el entorno presenta degradación, el framework aborta el proceso para no desperdiciar recursos de cómputo en la nube.

- **Custom Fixtures & Dependency Injection**: Extensión nativa del motor de Playwright para inyectar Page Objects pre-configurados en el contexto de cada prueba. Esto garantiza el aislamiento estricto de los datos, elimina la instanciación manual y mantiene el código altamente modular.

- **Shift-Left Security & Git Hooks**: Integración de automatizaciones en el ciclo de vida del control de versiones mediante Husky. Implementación de Pre-commit hooks para el análisis estático y prevención de fuga de credenciales (API keys/Tokens), junto con Pre-push hooks para la auditoría y bloqueo de vulnerabilidades críticas en el árbol de dependencias de Node.js.
