---
creado: 2026-05-14 09:14
modificado: 2026-05-14 09:14
share: "true"
---

# WhatsApp para Salesforce - Integración

## Descripción de los productos

A continuación se describen las soluciones identificadas en las referencias para integrar WhatsApp con Salesforce:
*Este es un documento de trabajo, los precios son aún referenciales y se tiene que confirmar.*
### 1. Tuvis (antes Whatslly)
Tuvis es una solución especializada para integrar aplicaciones de mensajería empresarial con CRM, seguridad y cumplimiento normativo. En el caso de Salesforce, permite trabajar conversaciones de WhatsApp y otros canales desde una experiencia conectada al CRM, con sincronización automática, trazabilidad y controles de seguridad.

*   **Descripción:** Según la demostración, Tuvis se conecta a WhatsApp mediante código QR, de forma similar a WhatsApp Web, y vincula la cuenta con Salesforce para mostrar información del cliente directamente en el entorno conversacional. En su web, Tuvis amplía esta propuesta como una plataforma para integrar **WhatsApp, Telegram, iMessage, Line, WeChat, llamadas de voz y SMS** con sistemas corporativos de productividad, seguridad y compliance.
*   **Potencialidades:**
    *   **Integración directa con Salesforce:** Sincroniza automáticamente mensajes, archivos multimedia y metadatos con registros de **Leads, Contactos, Cuentas y Oportunidades**.
    *   **Registro automático en Salesforce Activity Timeline:** Cada interacción queda vinculada al registro correspondiente, reduciendo la carga manual del equipo comercial.
    *   **Visión contextual del cliente:** Desde la conversación se puede visualizar información del contacto, cuenta y oportunidad asociada. La demo muestra que los campos visibles pueden configurarse según las necesidades del usuario.
    *   **Creación de registros desde WhatsApp:** Permite crear nuevos Leads o Contactos en Salesforce desde números no registrados, sin abandonar la conversación.
    *   **Creación de tareas y actividades:** Desde el chat se pueden generar actividades, tareas y seguimientos que luego quedan disponibles tanto en Tuvis como en Salesforce.
    *   **Continuidad operativa:** Al sincronizar conversaciones en Salesforce, supervisores u otros agentes pueden retomar una conversación con contexto completo si el responsable original se ausenta.
    *   **Automatización con Salesforce Flow:** La web indica que la integración puede activar flujos para actualizar oportunidades o crear tareas a partir de eventos de mensajería.
    *   **Productividad desde la conversación:** Permite agendar reuniones, enviar correos electrónicos, adjuntar archivos e incluir transcripciones completas de chats en emails, incluyendo integración con Outlook cuando aplica.
    *   **Búsqueda y filtros:** Permite buscar contactos de Salesforce desde la interfaz de mensajería, agregar leads desde números nuevos y filtrar historiales por criterios personalizados, fecha o usuario.
    *   **Plantillas personalizadas:** Soporta plantillas de mensajes con variables como nombre, compañía o cargo, útiles para estandarizar respuestas y mantener comunicaciones profesionales.
    *   **Métricas de gestión:** Desde la vista de administrador se pueden revisar mensajes enviados y recibidos, archivos compartidos, engagement, clientes más activos, tareas y actividades creadas, con filtros por usuario.
    *   **IA VIS:** La web presenta VIS como una capa de inteligencia que transforma mensajes en datos y registros, categoriza conversaciones, completa datos del CRM, registra actividades, transcribe mensajes de voz y genera resúmenes de interacciones.
*   **Seguridad y cumplimiento:**
    *   **DLP y prevención de fugas:** Permite definir reglas de Data Loss Prevention, supervisar palabras clave y generar alertas ante posibles filtraciones.
    *   **Monitoreo en tiempo real:** La web describe análisis de conversaciones en tiempo real para detectar riesgos, phishing, accesos no autorizados o comportamientos inusuales.
    *   **Archivado y auditoría:** Captura, transcribe y archiva interacciones corporativas en sistemas de almacenamiento existentes, facilitando auditorías y requisitos normativos.
    *   **Controles corporativos:** Integra capacidades como SSO, firewall, proxy, endpoint, control de copiar/pegar, capturas de pantalla, carga/descarga de archivos y marcas de agua.
    *   **Certificaciones:** La web menciona certificaciones **SOC 2 Tipo 2** e **ISO 27001**.
*   **Canales e integraciones:**
    *   **Canales soportados:** WhatsApp, Telegram, iMessage, Line, WeChat, llamadas de voz y SMS, según la web de Tuvis.
    *   **CRM y productividad:** La web menciona integraciones con Salesforce, Microsoft Dynamics, Creatio, HubSpot, Pipedrive, Outlook, Microsoft Teams, DocuSign, Zoom y otras herramientas.
    *   **Seguridad:** Se integra con sistemas corporativos como Microsoft Entra ID, Okta, CrowdStrike, Palo Alto, Kaspersky, Check Point, Fortinet y otros proveedores de seguridad.
*   **Diferenciador frente a bandejas compartidas:** Tuvis no se presenta solo como inbox multiagente, sino como una capa de productividad, trazabilidad, gobierno, seguridad y cumplimiento sobre canales de mensajería ya utilizados por los equipos comerciales.
*   **Limitaciones o puntos a validar:**
    *   La demo muestra conexión por QR, por lo que conviene validar si para el caso requerido se usará QR, WhatsApp Business API u otro esquema empresarial.
    *   No se identificaron precios públicos vigentes en la web consultada; el sitio orienta a solicitar una demostración.
    *   Debe confirmarse si las funciones avanzadas de IA, DLP, archivado, Salesforce Flow y llamadas están incluidas en el mismo plan o se licencian como módulos separados.
*   **Precios:** No publicados en la web oficial consultada. La referencia previa estimada era de **$30 a $45 USD por usuario/mes**, pero debe validarse comercialmente con Tuvis porque la web actual opera bajo solicitud de demo/cotización.

![[Pasted image 20260514140124.png|Pasted image 20260514140124.png]]

- Adicionalmente puede requerirse el pago del servicio de mensajería/API de WhatsApp Business, según el esquema contratado.
- [Presentación de Tuvis](https://youtu.be/zEkpXAi3JWA?si=IE_4MQKkRA71y7s6)

 - [Demo tuvis](https://youtu.be/bGkYU-B8m4Q?si=ySYRAN75rVixXvFP)
- [[Demostración Tuvis - Traanscripción|Demostración Tuvis - Traanscripción]]

### 2. Callbell
[Como funciona Callbell](https://www.youtube.com/watch?v=0tAVNEVWHPI)
- [[Video desmostración de Callbell - Transcripción|Video desmostración de Callbell - Transcripción]].

Callbell es una plataforma SaaS orientada a que equipos de ventas, soporte o atención al cliente gestionen conversaciones desde una bandeja compartida multiagente. En su sitio web se presenta como una plataforma CRM conversacional para **WhatsApp, Instagram Direct, Facebook Messenger y Telegram**, con foco en colaboración, automatización y métricas para equipos.

*   **Descripción:** Funciona desde navegador, aplicaciones móviles y versiones de escritorio, centralizando conversaciones de canales de mensajería en una sola interfaz. Callbell se declara **WhatsApp Business Partner** y posiciona su producto como una suite compuesta por chat multiagente, chatbot avanzado, módulo de difusión, API y webhooks.
*   **Potencialidades:**
    *   **Bandeja omnicanal compartida:** Permite recibir y responder mensajes de WhatsApp, Instagram Direct, Messenger y Telegram desde una sola interfaz.
    *   **Un solo número para varios agentes:** Varios usuarios pueden atender conversaciones asociadas al mismo número de WhatsApp, útil para equipos que superan la capacidad de atención de una sola persona.
    *   **Múltiples números y canales:** La web indica que se pueden conectar uno o más números de WhatsApp Business API y centralizarlos en una misma interfaz, incluso separando la atención por equipos y permisos.
    *   **Asignación y transferencia de conversaciones:** Los chats pueden asignarse manual o automáticamente a agentes, equipos o sucursales. También permite transferir conversaciones completas entre usuarios.
    *   **Notas internas entre agentes:** Los usuarios pueden dejar comentarios internos, mencionar compañeros y coordinar la atención sin que el cliente vea esas notas.
    *   **Etiquetas, embudos y campos personalizados:** Permite crear etiquetas, organizar conversaciones por etapas comerciales, administrar contactos y segmentar bases para operación comercial o soporte.
    *   **Respuestas rápidas y automáticas:** Incluye mensajes de bienvenida, ausencia, cierre, horarios de atención y respuestas rápidas para direcciones, catálogos, enlaces o información frecuente.
    *   **Enrutamiento y automatización:** Ofrece reglas de distribución automática y chatbots optimizados para WhatsApp y otros canales. La web menciona un **Advanced Bot Builder** para construir flujos no-code más complejos que los mostrados en la demo.
    *   **Métricas operativas:** Entrega KPIs sobre volumen de mensajes, tiempos de respuesta, chats pendientes, rendimiento del equipo, conversaciones asignadas y uso de etiquetas.
    *   **Aplicación móvil y escritorio:** Tiene aplicaciones para Android, iOS, Windows y MacOS, además del acceso por navegador.
    *   **Campañas y difusión en WhatsApp:** Incluye un módulo de broadcast/campañas para importar contactos por CSV, preparar mensajes con texto, imagen o documento y analizar indicadores de campaña.
    *   **API, webhooks e integraciones:** Callbell ofrece API pública, webhooks e integración oficial con Zapier. Esto permite conectar la plataforma con CRM/ERP corporativos y automatizar flujos sin depender solo de exportaciones CSV.
    *   **Integración posible con Salesforce vía Zapier:** Zapier publica una conexión Callbell + Salesforce con disparadores como contacto creado/actualizado, conversación abierta, mensaje creado, conversación cerrada o estado de mensaje actualizado; y acciones hacia Salesforce como crear lead, crear registro, actualizar contacto, buscar registros o agregar contactos/leads a campañas.
*   **Modalidades de conexión con WhatsApp:**
    *   **Código QR:** Es una conexión inmediata, similar a WhatsApp Web. Sirve para pruebas o usos simples, pero depende de que el teléfono permanezca conectado y no permite cargar el histórico completo de conversaciones.
    *   **WhatsApp Business API:** Es la opción más estable para uso empresarial. No depende de un teléfono conectado, permite recibir mensajes aunque el equipo no esté en línea y soporta audios, videos, ubicaciones, confirmaciones de lectura, documentos de mayor tamaño y nombre comercial verificado.
*   **Limitaciones relevantes:**
    *   No carga el historial completo de chats al conectar WhatsApp por primera vez.
    *   En la demostración, las métricas mostradas eran semanales; la web actual menciona estadísticas avanzadas y KPIs en tiempo real en planes superiores.
    *   No permite llamadas, videollamadas, listas de difusión ni chats grupales cuando se usa WhatsApp Business API, por restricciones propias de WhatsApp.
    *   Para iniciar conversaciones mediante WhatsApp Business API se requiere usar plantillas aprobadas de inicio de conversación.
    *   No se identificó en la web pública de Callbell un conector nativo específico para Salesforce; la alternativa viable es integración mediante API/webhooks, Zapier o exportación CSV.
*   **Precios mencionados en la demostración:**
    *   **Herramienta Callbell:** 14 euros por usuario/mes.
    *   **Canal WhatsApp por QR:** 35 euros por mes por número.
    *   **WhatsApp Business API:** 50 euros por mes por número.
    *   Se menciona mensajería ilimitada bajo costo fijo anual o trimestral, sin cobro por consumo de mensajes, sujeto al acuerdo comercial indicado por Callbell.
*   **Precios publicados en la web de Callbell:**
    *   **Multiagent Chat:** 15 USD por usuario/mes.
    *   **Multiagent Chat Plus:** 20 USD por usuario/mes; agrega soporte dedicado, estadísticas avanzadas, API e integraciones, y solicitud de WhatsApp verificado.
    *   **Enterprise:** precio personalizado; incluye 50+ agentes, integración con ChatGPT y autenticación SAML/SSO.
    *   **WhatsApp:** desde 54 USD/mes en créditos consumibles, según la página de precios.
    *   **Instagram Direct:** 22 USD/mes.
    *   **Módulo Broadcast/Campaign:** 0,02 USD por contacto alcanzado.
    *   **Advanced Bot Builder:** 65,55 USD/mes.
    *   **Cuentas adicionales de FB, Instagram, WhatsApp o Telegram:** 22 USD/mes.
*   **Prueba:** Ofrece un período de prueba de 7 días, sin requerir tarjeta de crédito según la web de precios.
*   **Señal de adopción:** La web indica que más de 75.000 empresas utilizan Callbell a nivel global.

### 3. QuickReply.ai
QuickReply.ai es una plataforma de automatización conversacional orientada principalmente a marketing, ventas, soporte y retención de clientes por WhatsApp. Su foco histórico está en e-commerce y DTC (Direct to customer), pero la web actual también posiciona casos de uso para educación, salud, bienes raíces, viajes, automotriz, servicios y equipos B2B que usan Salesforce.

*   **Descripción:** Utiliza WhatsApp Business API y otros canales conversacionales para automatizar campañas, atención, calificación de leads, recuperación de carritos y seguimiento comercial. La plataforma combina bandeja omnicanal, chatbots, broadcast, journeys, pagos, analítica e integraciones con CRM y herramientas de negocio.
*   **Potencialidades:**
    *   **Integración con Salesforce CRM:** La web publica una integración específica de **Salesforce CRM** para capturar leads desde WhatsApp y sincronizar conversaciones de clientes directamente en Salesforce, manteniendo actualizado el pipeline comercial.
    *   **WhatsApp dentro de Salesforce:** QuickReply indica que permite chatear 1 a 1 con leads y clientes desde Salesforce, registrar mensajes, centralizar interacciones y usar Salesforce como base de seguimiento comercial.
    *   **Captura y calificación de leads:** Permite capturar leads mediante widgets de WhatsApp, formularios conversacionales o anuncios Click-to-WhatsApp, calificarlos con bots y enviar solo leads con intención al equipo comercial.
    *   **Automatización con Salesforce Flows:** La web menciona disparadores basados en comportamiento para activar seguimientos, recordatorios y re-engagement según eventos como reuniones agendadas, ausencias, leads inactivos o etapas del pipeline.
    *   **Bandeja omnicanal:** Centraliza conversaciones de WhatsApp, web chat e Instagram en una sola bandeja, con historial completo, etiquetas, notas internas, estados de chat y filtros por agente, canal, estado o calidad del lead.
    *   **Chatbots y handover humano:** Permite usar bots para bienvenida, preguntas frecuentes, calificación inicial y recolección de datos; luego entrega el contexto completo a un agente humano cuando la conversación lo requiere.
    *   **Enrutamiento y asignación:** Soporta reglas para enviar conversaciones a ventas, soporte u otros equipos según canal, tema, respuestas del usuario, etiquetas u horarios de atención.
    *   **Campañas y broadcast:** Permite campañas masivas personalizadas, segmentación, filtros de audiencia, seguimiento de lectura, clics y conversiones, además de reintentos automáticos ante fallas de entrega.
    *   **Journeys y drip campaigns:** Permite construir flujos multi-etapa y multi-día con ramificaciones condicionales, útiles para abandono de carrito, postventa, win-back, upsell, cross-sell y nurturing.
    *   **E-commerce y retención:** Especializado en recuperación de carritos, abandono de navegación, alertas de pedidos, conversión de pedidos contra entrega a prepago, repetición de compra y campañas de lanzamiento.
    *   **Analítica:** Incluye métricas de conversión, engagement, desempeño de agentes, resultados por conversación, seguimiento de ROAS (Retunr on Ad Spend) y análisis de embudos.
    *   **Pagos por WhatsApp:** La web menciona pagos y conversiones de COD (Cash on delivery) a prepago mediante integraciones con pasarelas como Razorpay, PayU y Cashfree.
*   **Canales e integraciones:**
    *   **Canales:** WhatsApp, Instagram, Facebook Messenger, SMS, RCS y web chat, según la navegación principal de la web.
    *   **CRM:** Salesforce CRM, HubSpot, Zoho CRM, LeadSquared, Kylas, GoHighLevel, ERP/CRM genérico y otros.
    *   **Automatización/API:** Zapier, Pabbly, Pipedream y HTTP API.
    *   **E-commerce, soporte y analítica:** Shopify, Google Analytics, Meta Pixel, Freshdesk, Zoho Desk, Gorgias, Judge.me, Loox, Shiprocket, GoKwik, Shopflo, Razorpay y otros.
*   **Casos de uso destacados:**
    *   **Ventas B2B:** Seguimiento de leads, respuestas rápidas, notificaciones al equipo comercial y ciclos de venta más cortos.
    *   **Soporte:** Atención rápida, automatización de preguntas frecuentes, handover a agentes y trazabilidad de conversaciones.
    *   **Marketing Cloud / journeys:** Personalización de campañas usando datos de Salesforce, automatización de mensajes, segmentación y medición de interacciones.
    *   **Logística y servicios:** Notificaciones de entrega, confirmaciones, actualizaciones de estado y atención en tiempo real.
*   **Limitaciones o puntos a validar:**
    *   Aunque la web publica integración con Salesforce, conviene validar si el requerimiento específico usa Salesforce CRM, Salesforce Marketing Cloud o ambos, porque las capacidades descritas aparecen en páginas separadas.
    *   La sincronización bidireccional con CRM aparece asociada al plan Plus en la página de precios general; en planes menores puede requerir un cargo adicional o sincronización limitada.
    *   Los costos de WhatsApp no están incluidos en la suscripción: la web indica que los cargos de mensajería son adicionales y dependen del país, tipo de mensaje y volumen.
*   **Precios publicados en la web:**
    *   **Starter, Standard, Plus y Enterprise:** la página de precios muestra planes por nivel, pero no expone valores base visibles; orienta a reservar una demo/cotización.
    *   **Agentes incluidos:** Starter incluye 1 agente, Standard 2 agentes y Plus 5 agentes; agentes adicionales figuran como `₹500/mes` por agente en la tabla de precios.
    *   **Integración Salesforce:** la página específica de Salesforce indica que está disponible por **$50 USD/mes** en planes Starter y Standard, e incluida sin costo adicional en Plus.
    *   **Mensajería:** cargos adicionales. La página de Salesforce menciona mensajes desde **$0.009 USD por mensaje** para números de Estados Unidos; la página general indica que los cargos varían por país y categoría de mensaje.
    *   **WhatsApp API:** QuickReply aclara que WhatsApp no cobra una mensualidad fija por la API, pero sí existen cargos por mensajes plantilla y costos de proveedor/plataforma.
*   **Señal de adopción:** La web menciona más de 1000 negocios/merchants que usan QuickReply.ai; la página de inbox omnicanal menciona más de 1500 marcas en 29 países.

- [Video demostración](https://youtu.be/5Np9wGwrDxo?si=0VqVPMiAlRZPrfre)

### 4. WATI (wati.io)
WATI es una plataforma de mensajería empresarial basada en **WhatsApp Business API**, orientada a marketing, ventas y soporte. Su propuesta combina bandeja compartida, automatización no-code, campañas, IA conversacional, integraciones CRM y herramientas para operar WhatsApp a escala.

*   **Descripción:** WATI permite gestionar conversaciones de WhatsApp y otros canales desde una bandeja unificada para equipos. La web la presenta como una plataforma de crecimiento conversacional con IA, usada para adquirir leads, automatizar soporte, nutrir ventas y centralizar conversaciones. WATI se declara **Meta Business Partner** y también muestra asociación oficial con Google para anuncios que llevan a WhatsApp.
*   **Potencialidades:**
    *   **Integración con Salesforce CRM:** WATI publica una integración específica para conectar WATI con Salesforce en minutos y dar a los agentes contexto completo de los leads mientras conversan por WhatsApp.
    *   **Consulta de datos de Salesforce desde WATI:** Permite traer automáticamente datos de leads desde Salesforce hacia la ventana de chat de WATI, evitando alternar entre ambos sistemas.
    *   **Actualización de Salesforce desde WATI:** La web menciona sincronización bidireccional, permitiendo que los agentes actualicen datos de Salesforce en tiempo real desde la conversación en WATI.
    *   **Vista personalizada para agentes:** Permite seleccionar qué propiedades o campos de Salesforce mostrar en el widget de Team Inbox, por ejemplo estado del lead, datos de cuenta o campos personalizados.
    *   **Priorización de conversaciones:** Los datos enriquecidos del CRM pueden usarse para priorizar leads importantes y conversaciones con mayor valor comercial.
    *   **Bandeja de entrada del equipo:** Centraliza chats de ventas y soporte, permite asignar conversaciones a usuarios, organizar equipos, etiquetar contactos, hacer seguimiento y colaborar entre agentes.
    *   **Gestión de contactos:** Soporta listas de contactos, alta de nuevos números, importación/exportación CSV y etiquetas para segmentar categorías como VIP u otros criterios comerciales.
    *   **Chatbots no-code:** Permite crear flujos de chatbot sin código, automatizar hasta 200 pasos, interconectar múltiples chatbots y apoyarse en APIs e integraciones documentadas.
    *   **WATI AI / Astra:** Incluye capacidades de IA para calificar leads, descubrir intención, responder consultas, automatizar recordatorios y derivar conversaciones complejas a agentes humanos.
    *   **Campañas y difusión:** Permite enviar campañas multimedia, usar plantillas, medir apertura/lectura, ejecutar retargeting y trabajar con anuncios Click-to-WhatsApp.
    *   **WhatsApp Business API oficial:** A diferencia de WhatsApp Business App, permite múltiples agentes, altos volúmenes, automatizaciones, webhooks, catálogos, flujos, analítica y conexión con sistemas externos.
    *   **WhatsApp Business Calling:** La web menciona llamadas de WhatsApp Business como parte del producto, útil si se requiere pasar de chat a voz dentro del ecosistema WhatsApp.
*   **Canales e integraciones:**
    *   **Canales:** WhatsApp, llamadas de WhatsApp Business, Instagram, Facebook Messenger, widget web, enlaces `wa.me`, códigos QR, SMS y otros canales sociales según la web.
    *   **CRM e integraciones:** Salesforce, HubSpot, Zoho CRM, Shopify, WooCommerce, Zapier, Pabbly Connect, Make/Integromat, Google Sheets, Klaviyo, Zoho Flow, WhatsApp Shop y otras herramientas.
    *   **API y webhooks:** El plan Business incluye 20 millones de llamadas API por mes y webhooks extensivos, según la página de precios.
*   **Casos de uso destacados:**
    *   **Marketing:** Captura de leads desde anuncios Click-to-WhatsApp, campañas personalizadas, retargeting y medición de rendimiento.
    *   **Ventas:** Calificación automática de leads, asignación a representantes, visibilidad de conversaciones y seguimiento del pipeline.
    *   **Soporte:** Resolución de preguntas frecuentes con IA, enrutamiento a agentes, control de tiempos de respuesta y reportes por operador.
    *   **E-commerce:** Catálogo de WhatsApp, recuperación de carritos, plantillas de pedidos, Shopify y opciones de checkout/pago según el plan.
*   **Limitaciones o puntos a validar:**
    *   Salesforce aparece incluido dentro de **integraciones ilimitadas** en el plan Business; en planes menores conviene validar si está disponible o requiere upgrade.
    *   Los cargos por plantillas/mensajes de WhatsApp son adicionales y varían según categoría: marketing, utilidad o autenticación.
    *   La integración avanzada depende del alcance contratado: API, webhooks, múltiples números, roles, enmascaramiento de teléfonos, listado blanco de IPs y soporte dedicado aparecen asociados a planes superiores.
    *   Debe validarse si el caso requiere Salesforce Sales Cloud, Service Cloud, Marketing Cloud o solo sincronización de leads/contactos.
*   **Precios publicados en la web:** (REVISAR)
      **Plan Pay-as-you-go:** pago único de **$12**, recuperado como créditos de mensajes; orientado a campañas masivas sin suscripción recurrente.
    *   **Growth:** 3 usuarios incluidos, sin usuarios adicionales; incluye configuración de WhatsApp sin costo, bandeja omnicanal, campañas estándar, captura de leads, Team Inbox, herramientas e-commerce, 15k plantillas/mes, 1k activadores de automatización/mes, 2 integraciones seleccionadas y 10k llamadas API/mes sin webhooks.
    *   **Pro:** 5 usuarios incluidos; usuarios adicionales a **$24 USD/usuario/mes**; agrega chatbot avanzado, formularios, automatización en Instagram, retargeting, plantillas carrusel, pagos en catálogo, automatización con IA, Astra AI Agents, equipos, enrutamiento automático, reportes de operadores, 2k activadores/mes, 5 integraciones seleccionadas, 200k llamadas API/mes y webhooks limitados.
    *   **Business:** 5 usuarios incluidos **$199**; usuarios adicionales a **$59 USD/usuario/mes**; agrega múltiples números, asignación rotativa, descuentos por volumen, soporte prioritario, roles, enmascaramiento de números, listado blanco de IPs, integraciones ilimitadas incluyendo **Salesforce**, 20M llamadas API/mes, webhooks extensivos y 5k activadores/mes.
    *   **Mensajería:** cargos adicionales por plantillas y mensajes, cobrados según tarifa de WATI/Meta.
*   **Prueba:** La página de integración con Salesforce ofrece prueba gratuita de 7 días; otras páginas de WATI mencionan prueba gratuita sin tarjeta de crédito.
*   **Señal de adopción:** WATI declara más de **16.000 clientes** en más de **180 países**, más de **10B mensajes procesados**, 99,9% de uptime histórico y rating aproximado de 4,6/5 en G2.

- [Información de Leads en Wati](https://www.youtube.com/watch?v=RDFzqSQ4wgE)
### 5. Automatización utilizando Twilio
- [Salesforce WhatsApp integration](https://www.youtube.com/watch?v=OL1weB1iLGY)
- [[Salesforce e integración WhatsApp - transcripción|Salesforce e integración WhatsApp - transcripción]]

La automatización utilizando Twilio corresponde a una integración personalizada entre Salesforce y WhatsApp Business mediante APIs. A diferencia de soluciones SaaS como Tuvis, Callbell o QuickReply.ai, esta alternativa requiere configuración técnica en Salesforce, desarrollo Apex y uso de Twilio como proveedor de mensajería WhatsApp.

*   **Descripción:** La demostración construye un caso de uso donde Salesforce actúa como sistema central de datos y lógica de negocio, mientras Twilio opera como pasarela para enviar y recibir mensajes de WhatsApp. El ejemplo usa una academia ficticia en Salesforce, con objetos como estudiantes, asistencia, notas y anuncios, para responder automáticamente consultas enviadas por WhatsApp.
*   **Arquitectura general:**
    *   **Salesforce:** almacena los datos del negocio y ejecuta la lógica mediante Apex.
    *   **Twilio WhatsApp Sandbox:** permite probar el envío y recepción de mensajes de WhatsApp durante la etapa de desarrollo.
    *   **Named Credential y External Credential:** Salesforce los usa para autenticar llamadas hacia la API de Twilio con `Account SID` y `Auth Token`.
    *   **Apex Callout:** clase Apex que envía mensajes a WhatsApp usando el endpoint de Twilio.
    *   **Apex REST Webhook:** endpoint en Salesforce que recibe mensajes entrantes desde Twilio.
    *   **Salesforce Site:** expone públicamente el endpoint REST para que Twilio pueda invocarlo cuando llega un mensaje de WhatsApp.
*   **Flujo funcional demostrado:**
    *   El usuario envía un mensaje inicial por WhatsApp, por ejemplo `hi`, `hello`, `menu` o `start`.
    *   Twilio recibe el mensaje y lo reenvía al webhook Apex configurado en Salesforce.
    *   Salesforce valida si el número telefónico existe en la base de datos, por ejemplo como estudiante o apoderado registrado.
    *   Si el número existe, Salesforce responde con un menú de opciones: anuncios, asistencia o notas.
    *   Según la opción seleccionada, Salesforce consulta los objetos correspondientes y devuelve la información por WhatsApp.
    *   Si el número no existe, Salesforce responde con un mensaje indicando que no se encontró el registro y que el número debe estar registrado.
*   **Potencialidades:**
    *   **Automatización altamente flexible:** Permite adaptar WhatsApp a cualquier objeto, campo o proceso de Salesforce, no solo a Leads o Contactos.
    *   **Consultas desde WhatsApp hacia Salesforce:** Los usuarios pueden consultar información almacenada en Salesforce, como estados, anuncios, notas, asistencia, pedidos, casos o cualquier dato modelado en el CRM.
    *   **Mensajería saliente desde Salesforce:** Permite enviar mensajes automáticos desde Apex ante eventos, cambios de estado, creación de registros o ejecución de procesos.
    *   **Interacciones bidireccionales:** No se limita al envío de notificaciones; también puede recibir respuestas del cliente y ejecutar lógica en Salesforce.
    *   **Menús conversacionales simples:** Se pueden construir flujos tipo menú con opciones numéricas o palabras clave, útiles para autoservicio básico.
    *   **Uso de lógica de negocio propia:** Salesforce puede decidir qué responder según reglas, validaciones, permisos, estado del registro o información histórica.
    *   **Escalabilidad técnica:** Twilio ofrece APIs programables para WhatsApp, Conversations API, mensajería bidireccional, plantillas, webhooks y, según disponibilidad, llamadas de WhatsApp Business.
    *   **Integración multicanal futura:** Al usar Twilio, la arquitectura podría ampliarse a SMS, RCS, voz u otros canales soportados por Twilio.
*   **Pasos técnicos principales según la demostración:**
    *   Crear o ingresar a una cuenta de Twilio.
    *   Activar el flujo de prueba en **Twilio WhatsApp Sandbox** y vincular el número personal mediante el mensaje `join` indicado por Twilio.
    *   Obtener `Account SID` y `Auth Token` desde Twilio Console.
    *   Crear en Salesforce una **External Credential** con autenticación Basic Auth.
    *   Crear una **Named Credential** apuntando al endpoint de Twilio API y habilitar callouts.
    *   Desarrollar una clase Apex para enviar mensajes WhatsApp usando `POST` y contenido `application/x-www-form-urlencoded`.
    *   Probar el envío desde Anonymous Apex y validar respuesta HTTP `201` como envío exitoso.
    *   Crear una clase Apex REST como webhook para procesar mensajes entrantes.
    *   Crear un Salesforce Site para exponer el webhook públicamente.
    *   Dar permisos al guest user del Site sobre las clases Apex y el External Credential Principal.
    *   Configurar la URL del webhook en Twilio Sandbox Settings usando método `POST`.
*   **Limitaciones o riesgos:**
    *   **Requiere desarrollo:** No es una solución no-code; necesita conocimientos de Apex, APIs, seguridad de Salesforce, Sites y configuración de Twilio.
    *   **Gobierno de seguridad:** Exponer un endpoint por Salesforce Site exige validar autenticidad, sanitizar entradas, controlar permisos y evitar abuso del endpoint público.
    *   **Sandbox no es producción:** El sandbox de Twilio sirve para pruebas; para producción se requiere configurar un número de WhatsApp Business aprobado y plantillas verificadas cuando corresponda.
    *   **Mantenimiento interno:** La empresa debe mantener código, manejo de errores, logs, reintentos, monitoreo, límites de API, pruebas y cambios de versión.
    *   **Experiencia de agente limitada:** Por sí sola, esta arquitectura no entrega una bandeja multiagente, asignación de conversaciones, métricas de atención ni interfaz para equipos comerciales, salvo que se desarrollen adicionalmente.
    *   **Cumplimiento de WhatsApp:** Los mensajes iniciados por la empresa deben respetar reglas de opt-in, plantillas aprobadas y ventanas de servicio definidas por Meta.
*   **Precios:**
    *   **Twilio:** modelo pay-as-you-go. La web de Twilio indica una tarifa de **$0.005 USD por mensaje WhatsApp** de Twilio, tanto entrante como saliente, más las tarifas de Meta por mensajes plantilla cuando aplican.
    *   **Meta:** cobra por mensajes plantilla según categoría y país: utility, authentication o marketing. Los mensajes free-form solo aplican dentro de la ventana de atención al cliente.
    *   **Costos Salesforce:** no hay licencia SaaS adicional de un conector, pero sí hay costo de desarrollo, mantenimiento, pruebas, monitoreo y posible consumo de recursos/licencias de Salesforce.
*   **Cuándo conviene:** Es una alternativa útil cuando se requiere una automatización específica, control total de la lógica y fuerte integración con objetos propios de Salesforce. Es menos conveniente si se necesita una solución rápida para usuarios comerciales con bandeja compartida, métricas listas, gestión de agentes y configuración no-code.

### 6. Solución "Click to Chat" (Manual - No-Code)
Es un método nativo y gratuito que utiliza la funcionalidad "Clic para chatear" de WhatsApp para iniciar conversaciones desde Salesforce.

*   **Descripción:** Consiste en crear botones o enlaces personalizados en Salesforce (usando el formato de URL `https://wa.me/{Teléfono}`) que, al ser pulsados, abren la aplicación de WhatsApp con el número del cliente pre-cargado.
*   **Ventajas:**
    *   **Cero costo:** No requiere suscripciones a terceros ni pagos por API.
    *   **Simplicidad:** Configuración rápida mediante la creación de botones o campos de fórmula sin necesidad de código complejo.
    *   **Sin complicaciones de API:** No requiere verificación de Meta Business Manager ni configuraciones técnicas avanzadas.
    *   **Privacidad:** El usuario mantiene el control total de cuándo y cómo inicia la conversación.
*   **Precios:** **Gratis** (solo requiere configuración en el Object Manager de Salesforce).

## Referencias

1. https://www.wati.io/
2. https://www.callbell.eu/en/
3. https://www.callbell.eu/en/pricing/
4. https://www.callbell.eu/en/whatsapp-crm-platform/
5. https://docs.callbell.eu/
6. https://zapier.com/apps/callbell/integrations/salesforce
7. https://tuvis.com/es/
8. https://tuvis.com/es/channels/salesforce/
9. https://tuvis.com/es/productivity/
10. https://tuvis.com/es/security/
11. https://tuvis.com/es/compliance/
12. https://www.quickreply.ai/
13. https://www.quickreply.ai/pricing
14. https://www.quickreply.ai/integrations
15. https://www.quickreply.ai/integrations/salesforce-crm
16. https://www.quickreply.ai/whatsapp-salesforce-integration-pricing
17. https://www.quickreply.ai/whatsapp-salesforce-marketing-cloud
18. https://www.quickreply.ai/omnichannel-messaging-inbox
19. https://youtu.be/OL1weB1iLGY
20. https://www.twilio.com/en-us/messaging/channels/whatsapp
21. https://www.twilio.com/en-us/whatsapp/pricing
22. https://www.twilio.com/docs/whatsapp
23. https://www.wati.io/
24. https://www.wati.io/pricing/
25. https://www.wati.io/saleforce-integration/
26. https://www.wati.io/whatsapp-business-api/
27. https://www.wati.io/shared-team-Inbox/
28. https://www.wati.io/no-code-chatbot/
29. https://youtu.be/bGkYU-B8m4Q?si=d6SvSRnDDCnfWHbM
30. https://youtu.be/0tAVNEVWHPI?si=Q8GNT09awHpSdznO
31. https://youtu.be/5Np9wGwrDxo?si=ldgs-NzCj3TM9v7G