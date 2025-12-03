# 📌 Chat Flows Chart – n8n Webhook con Twilio #

Este proyecto muestra un flujo completo en n8n para:

- Recibir mensajes a través de un Webhook (POST) y conectarlo con Twilio.
- Procesar los mensajes con un agente de IA (Google Gemini).
- Responder al usuario mediante SMS, MMS o WhatsApp.

# 🚀 Resumen del Flujo Principal #

1. Recepción de Datos via Webhook                                                                                    
**El flujo inicia con un Webhook (POST) que recibe datos desde Twilio.**

## Twilio: Pasos Adicionales ##

- Crear una cuenta en Twilio.
- Registrar un número telefónico para pruebas.

2. Procesamiento con IA                                                                                                    
**Se utiliza un agente de IA con un prompt personalizado para responder preguntas concretas sobre horarios, disponibilidad y costo.**

3. Respuesta al Usuario                                                                                                                    
**El mensaje generado por la IA se envía de vuelta al usuario usando Twilio, ya sea por SMS, MMS o WhatsApp.**

# 🔧 Tecnologías Utilizadas #

- n8n
- Twilio
- Google Gemini (Chat Model)
- IA Agent + Memory
- Webhook Trigger

# 📅 Objetivo del Proyecto #

- Demostrar cómo integrar un flujo de n8n con Twilio y un agente de IA para:
- Recibir y procesar mensajes de forma automática.
- Responder con información específica y relevante.
- Enviar respuestas a través de múltiples canales.
