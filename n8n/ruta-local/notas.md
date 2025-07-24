
# Notas de Aprendizaje n8n - Ruta Local

## Pasos seguidos en n8n
1. Instalado Node.js y npm
2. Instalado Docker Desktop (opcional)
3. Instalado n8n globalmente con `npm install -g n8n`
4. Verificada la arquitectura del sistema (64-bit, amd64) para instalar docker-desktop
5. Iniciado n8n localmente con el comando `n8n`
6. Acceso a la interfaz web en http://localhost:5678
7. Creación de un nuevo flujo de trabajo
8. Creación del nodo Webhook como disparador principal del flujo
9. Configuración del nodo Webhook (selección de método POST y copia de la URL generada)
10. Creación del nodo Email para el envío de correos
11. Configuración del nodo Email (selección de credencial SMTP, destinatario, asunto y mensaje)
12. Conexión entre el nodo Webhook y el nodo Email
13. Guardado y activación del flujo
14. Configurada credencial SMTP con autenticación, puerto 465 y SSL/TLS
15. Solucionados errores de autenticación y relay configurando usuario y contraseña correctos
16. Realizada prueba de envío de correo con contenido en texto y HTML
17. Prueba exitosa de envío de correo usando Postman y el webhook de n8n
18. El correo llegó correctamente a la bandeja de entrada (puede llegar a spam si faltan registros SPF/DKIM/DMARC)

## Observaciones sobre límites de envío
- El límite de correos no lo impone n8n, sino tu servidor SMTP o proveedor de correo
- Proveedores gratuitos suelen tener límites diarios o por hora (por ejemplo, Gmail: 100-500 correos/día)
- Servidores propios pueden configurarse sin límite, pero corres riesgo de ser marcado como spam si abusas
- Es recomendable consultar la política de tu proveedor para evitar bloqueos

## Observaciones generales
- n8n muestra mensaje para activar funciones avanzadas (no obligatorio)
- Todos los nodos y disparadores básicos son gratuitos
- Solo servicios externos pueden requerir cuentas o pagos

---
Puedes seguir agregando aquí cada paso, configuración, error o aprendizaje relevante durante tu avance con n8n.
