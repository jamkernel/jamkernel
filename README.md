README.md

```markdown
# JAM Omni-Kernel P2P v1.2

### *Núcleo criptográfico para comunicaciones descentralizadas*

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES2020-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

---

## 🌌 ¿Qué es?

JAM Omni-Kernel es un núcleo ligero que permite comunicación entre pares de forma descentralizada y segura. 
Funciona en navegadores, Node.js, Deno y Bun sin necesidad de infraestructura externa.

**Un solo archivo. Cero dependencias.**

---

## 🛡️ Características

- **Cifrado Militar:** AES-256-GCM con autenticación y PBKDF2 (60,000 iteraciones)
- **Anti-DoS Integrado:** Rate limiting por peer + listas negras automáticas
- **Purga Forense:** Eliminación física de claves en memoria RAM
- **Almacenamiento Local:** IndexedDB con mutex y backoff exponencial
- **Multi-Entorno:** Navegadores, Node.js, Deno, Bun
- **Zero Dependencies:** Sin librerías externas

---

## 💻 Uso Rápido

```javascript
// 1. Instanciar el Kernel
const jam = new JAMOmniKernel();

// 2. Iniciar sesión segura
await jam.startSession('mi-sala-soberana', 'mi-clave-segura');

// 3. Transmitir datos cifrados
await jam.mesh.broadcast({ 
    type: 'MENSAJE', 
    data: 'Hola mundo descentralizado!' 
});

// 4. Recibir mensajes
jam.events.on('peer:message', (data) => {
    console.log(`📨 ${data.peerId}:`, data.message);
});

// 5. Cerrar sesión (purga forense)
await jam.closeSession();
```

---

📚 Documentación

· API Reference — Documentación técnica completa
· Guía de Uso — Tutorial paso a paso
· Guía de Seguridad — Prácticas recomendadas

---

🤝 Contribuciones

Las contribuciones son bienvenidas. Lee nuestra Guía de Contribución.

Contacto: jamkernelp2p@gmail.com

---

📜 Licencia

GNU General Public License v3.0

---

✨ Agradecimientos

Félix Martínez — 2026

Dedicado a mi hijo, por ser la motivación para construir tecnología que construya un mejor futuro.