# Notas de Aprendizaje n8n - Ruta Local

## Progreso y Configuraciones

### Instalación y configuración
- Instalado Node.js y npm
- Instalado Docker Desktop (opcional)
- Instalado n8n globalmente con `npm install -g n8n`
- Verificada la arquitectura del sistema (64-bit, amd64)
- Iniciado n8n localmente con el comando `n8n`

### Primeros pasos en n8n

### Configuración y pruebas de envío de correo
- Configurada credencial SMTP con autenticación, puerto 465 y SSL/TLS
- Ajustado el campo "client host name" para evitar error HELO (usando "localhost")
- Solucionados errores de autenticación y relay configurando usuario y contraseña correctos
- Realizada prueba de envío de correo con contenido en texto y HTML
- Prueba exitosa de envío de correo usando Postman y el webhook de n8n
- El correo llegó correctamente a la bandeja de entrada (puede llegar a spam si faltan registros SPF/DKIM/DMARC)

### Observaciones sobre límites de envío
- El límite de correos no lo impone n8n, sino tu servidor SMTP o proveedor de correo
- Proveedores gratuitos suelen tener límites diarios o por hora (por ejemplo, Gmail: 100-500 correos/día)
- Servidores propios pueden configurarse sin límite, pero corres riesgo de ser marcado como spam si abusas
- Es recomendable consultar la política de tu proveedor para evitar bloqueos

### Observaciones
- n8n muestra mensaje para activar funciones avanzadas (no obligatorio)
- Todos los nodos y disparadores básicos son gratuitos
- Solo servicios externos pueden requerir cuentas o pagos

---
Puedes seguir agregando aquí cada paso, configuración, error o aprendizaje relevante durante tu avance con n8n.
