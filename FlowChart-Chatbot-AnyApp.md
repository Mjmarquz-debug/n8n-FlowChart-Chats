# 📌 Chat Flows Chart – n8n Webhook Chat Flow #

Este proyecto muestra un flujo completo creado en n8n para:

- Recibir mensajes a través de un Webhook.
- Procesarlos con un agente de IA (Google Gemini).
- Clasificar país y ciudad.
- Validar la información.
- Responder con un JSON estructurado.
- Opcionalmente, agendar automáticamente una cita en Google Calendar.

Este repositorio sirve como ejemplo práctico para quienes buscan aprender a crear flujos inteligentes, estructurados y escalables en n8n.

# 🚀 Resumen del Flujo Principal #

1. Recepción de Datos via Webhook  
**El flujo inicia con un Webhook (POST) que recibe datos de un formulario simulado.**

2. Validación del Mensaje (IF)                                                                                                                                                                             
**Se verifica que el mensaje no esté vacío.**                                                                   
*Si está vacío, se devuelve un error en JSON.*                                                                                  
*Si no está vacío, continúa el flujo.*                                                

3. Conexión con el Flujo de IA                                                                                               
**Se llama a un flujo secundario que utiliza el agente de IA para procesar el mensaje y extraer país y ciudad.**

4. Mapeo Final de País y Ciudad                                                                     
**Se realiza otro mapeo para asegurar que la respuesta final esté bien estructurada.**

5. Respuesta Final (Respond to Webhook)                                                                              
**Se devuelve un JSON confirmando la recepción y procesamiento correcto.**

6. Integración con Google Calendar (*Opcional*)                                                                                                            
**El flujo puede crear un evento en Google Calendar automáticamente.**

# 🔧 Tecnologías Utilizadas #

- n8n
- Webhook Trigger
- Google Gemini (Chat Model)
- IA Agent + Memory + Structured Output Parser
- Google Calendar 
- JSON Manual Mapping
- Conditional logic (IF)

# 📅 Objetivo del Proyecto #

- Demostrar cómo construir un flujo profesional en n8n que sea capaz de:
- Recibir y validar datos externos.
- Procesar información con IA.
- Devolver respuestas estructuradas.
- Integrarse con servicios externos como Google Calendar.
- Mantener una arquitectura modular.
