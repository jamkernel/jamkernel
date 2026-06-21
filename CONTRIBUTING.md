
---

### **CONTRIBUTING.md**

```markdown
# 🤝 Guía de Contribución

¡Gracias por tu interés en JAM Omni-Kernel!

---

## Tipos de Contribución

- **💻 Código:** Nuevas funcionalidades, optimizaciones, correcciones
- **📚 Documentación:** Traducciones, guías, ejemplos
- **🔐 Seguridad:** Auditorías, reporte de vulnerabilidades
- **🌐 Difusión:** Compartir, usar, recomendar

---

## Reporte de Vulnerabilidades

**No** reportes vulnerabilidades en issues públicos.

Envía un correo a: **jamkernelp2p@gmail.com**

Incluye:
- Descripción detallada
- Pasos para reproducir
- Versiones afectadas

---

## Pull Requests

1. **Fork** el repositorio
2. **Crea una rama** con nombre descriptivo
3. **Desarrolla** los cambios
4. **Prueba** que todo funcione
5. **Envía** el Pull Request con descripción

---

## Estilo de Código

```javascript
// ✅ Buenas prácticas
class SecureComponent {
    constructor() {
        this._privateField = null;
    }
    
    async publicMethod() {
        const result = await this._privateMethod();
        return result;
    }
}