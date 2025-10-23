## **1. Descripción General**

Este documento presenta la hoja de ruta del proyecto “La Incertidumbre en Salud”, una propuesta tecnológica desarrollada con el propósito de brindar **orientación médica básica no diagnóstica** a usuarios que viven en zonas rurales o con acceso limitado a servicios de salud.  
El enfoque principal ha sido crear una **solución práctica y funcional** que permita al usuario obtener recomendaciones claras y accionables ante situaciones médicas imprecisas, sin reemplazar la labor de un profesional.

---

## **2. Fase Inicial — MVP (2 días)**

### **2.1 Descripción**

El MVP se desarrolló como un **chat conversacional funcional** siguiendo el flujo principal:

> Usuario describe su sintomatología → asistente clasifica prioridad → asistente consulta documentación médica → asistente describe indicaciones de orientación al usuario.

### **2.2 Implementación técnica**

Debido al tiempo limitado y a la necesidad de presentar una solución funcional en poco tiempo, el MVP se implementó de la siguiente forma:

- **Frontend:** desarrollado en **HTML puro**, alojado en **GitHub Pages**.
    
- **Estilos:** integración mediante CDN de **Tailwind CSS** para agilizar la maquetación visual.
    
- **Interfaz conversacional:** se integró el **widget de VoiceFlow** a través de su CDN, encargado de ejecutar el flujo conversacional configurado
    
- **Sin frameworks ni backend propio:** el flujo de conversación y lógica principal se manejan desde la configuración en VoiceFlow.
    

>*EL objetivo principal fue dar solucion a la problematica con intergaciones*
### **2.3 Integración pendiente (MCP no implementado)**

Durante el desarrollo se evaluó la posibilidad de integrar el recurso abierto disponible en:

> [https://github.com/Cicatriiz/healthcare-mcp-public](https://github.com/Cicatriiz/healthcare-mcp-public)  
> Este proyecto público ofrece un **servidor MCP ** orientado a conectar sistemas externos con servicios de consulta médica y repositorios de información en salud.  
> No se logró implementar debido a **limitaciones técnicas, de tiempo y desconocimiento en la configuración del entorno de servidor**, lo cual impidió su conexión con la interfaz del MVP.  
> Sin embargo, se reconoce la  integración **hubiera permitido ampliar el alcance del sistema bastante**, habilitando consultas a bases de conocimiento externas y mejorando la calidad de las orientaciones ofrecidas al usuario.

---

## **3. Fase de Producto (6 meses)**

En esta etapa el proyecto busca establecer una estructura más sólida con roles definidos y mayor trazabilidad de las consultas generadas por los usuarios.

### **3.1 Características principales**

- Inclusión de un **rol de moderador clínico** encargado de validar reglas y criterios del triage médico sin emitir diagnósticos.
    
- Rol de **administrador del sistema** para la gestión del catálogo de síntomas, métricas y configuraciones.
    
- Implementación de una **base de datos MySQL** para registrar y analizar las consultas.
    
- **Integración con WhatsApp**, priorizando el acceso desde canales comunes en comunidades rurales.
    
- **Reevaluación técnica del MCP público**, con el objetivo de implementar la conexión con servicios de salud externos.
    

---

## **4. Fase de Escalamiento (1 año)**

El propósito en este punto es mejorar la calidad del servicio, la capacidad de respuesta y la cobertura de usuarios mediante la incorporación de nuevas funcionalidades.

### **4.1 Características proyectadas**

- Detección automática de palabras clave críticas (“no respira”, “convulsiona”, etc.).
    
- Botón de **alerta rápida (SOS)** conectado a centros de salud locales.
    
- Expansión a nuevas plataformas conversacionales (Telegram, Messenger).
    
- Personalización de respuesta según **perfiles de riesgo** (niños, adultos mayores, gestantes).
    
- Inclusión de **reconocimiento de voz** para usuarios con baja alfabetización.
    
- Integración funcional del **MCP de salud** para consulta de información médica en tiempo real.
    

---

## **5. Fase de Consolidación (5 años)**

En este horizonte el proyecto se plantea como un sistema de apoyo validado y útil para entidades médicas, con impacto directo en la reducción de la incertidumbre en decisiones de salud.

### **5.1 Proyección**

- Integración con plataformas de **telemedicina**, permitiendo contacto directo con profesionales en casos urgentes.
    
- Validación legal y certificación por parte de **autoridades sanitarias nacionales**.
    
- Módulo colaborativo para **actualización de protocolos clínicos** por médicos acreditados.
    
- Sistema de **seguimiento continuo de síntomas** para coordinación con citas médicas.
    
- Rol analítico para **entidades de salud** orientado al estudio de patrones y tendencias epidemiológicas.
    

---

## **6. Impacto Social**

El proyecto busca **reducir la brecha informativa en salud** mediante una herramienta digital accesible, comprensible y gratuita, que:

- Brinda orientación rápida ante síntomas comunes.
    
- Disminuye desplazamientos innecesarios y gastos médicos evitables.
    
- Promueve la toma de decisiones acertadas en comunidades rurales.
    
- Facilita la futura integración con redes médicas locales y nacionales.