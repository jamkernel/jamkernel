
---

### **docs/SECURITY-GUIDE.md**

```markdown
# 🔒 Guía de Seguridad

## Principios de Seguridad

### 1. Cifrado
- **AES-256-GCM:** Cifrado estándar militar con autenticación
- **PBKDF2:** 60,000 iteraciones para derivación de claves
- **Sal Dinámica:** Combinada con el ID de la sala

### 2. Memoria
- **Purga Forense:** Las claves se eliminan físicamente de la RAM
- **Garbage Collection:** Forzado al cerrar sesión
- **Nullificación:** Todas las referencias se rompen

### 3. Red
- **Rate Limiting:** 12 mensajes por segundo por peer
- **Blacklist:** Bloqueo automático de peers maliciosos
- **Sanitización:** Todas las entradas son validadas

---

## Recomendaciones

### Para Desarrolladores

1. **Usar HTTPS** en producción
2. **Validar entradas** antes de procesarlas
3. **Manejar errores** correctamente
4. **Cerrar sesiones** al finalizar

### Para Usuarios

1. **Usar contraseñas fuertes** (mínimo 8 caracteres)
2. **No compartir claves** de sala
3. **Actualizar** a la última versión
4. **Reportar vulnerabilidades** de forma responsable

---

## Reporte de Vulnerabilidades

**Email:** jamkernelp2p@gmail.com

Incluye:
- Descripción detallada
- Pasos para reproducir
- Versión afectada
- Posible impacto

---

## Auditorías

Las auditorías de seguridad se realizan periódicamente.

**Última auditoría:** En curso...