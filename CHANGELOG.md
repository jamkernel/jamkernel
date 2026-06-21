# 📋 Historial de Cambios

## [1.2.0] - 2026-01-20

### 🔒 Seguridad
- Purga forense real de claves en memoria RAM
- Rate limiting por peer (12 msg/segundo)
- Blacklist automática para ataques DoS
- Timeout en operaciones de descifrado (4 segundos)

### 🚀 Mejoras
- Base64URL para compatibilidad con caracteres especiales
- Backoff exponencial en operaciones de disco
- Sanitización de PeerIDs y RoomIDs
- EventBus inmune a condiciones de carrera

### 🐛 Correcciones
- Bug crítico en `transaction.objectStore()`
- Logs sanitizados sin exposición de datos sensibles
- Límite de cola en BatchStorage (1000 elementos)

---

## [1.1.0] - 2025-12-15

### 🎉 Primera versión estable
- Soporte multi-entorno (Node/Deno/Bun/Browser)
- Cifrado AES-256-GCM
- Batch Storage con IndexedDB
- WebRTC Full-Mesh