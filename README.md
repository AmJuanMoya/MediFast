<img width="1315" height="112" alt="image" src="https://github.com/user-attachments/assets/93252647-29b9-4640-a24d-e7f3b61e986b" />

*MVP - Chat-Bot conversacional para agilizar orientación medica a población rural.*
## CONTENIDO

1. CONTEXTO DEL PROYECTO- MEDIFAST
2. ALCANCE DEL MVP
3. ARQUITECTURA Y COMPONENTES
4. STACK TECNOLOGICO
5. ROLES Y RESPOSABILIDADES
6. PRUEBAS DE ACEPTACION Y VALIDACION
7. LICENCIA Y CREDITOS




---
## 1.Contexto del Proyecto

En zonas rurales y periurbanas, muchas personas enfrentan **incertidumbre médica**: no saben si un síntoma necesita atención inmediata o puede manejarse en casa.  
El  MVP busca **reducir esta incertidumbre**, brindando **orientación básica y confiable** mediante una conversación sencilla con una base de conocimientos, **sin reemplazar al personal médico.**

**Problema identificado:** Falta de acceso oportuno a orientación médica clara y comprensible en momentos de urgencia.  
**Objetivo del MVP:** Ofrecer una primera orientación que clasifique los síntomas por niveles de urgencia y le indique al usuario una primera forma de actuar ante la situacion adndo solucion al problema de "Incertidumbre en la Salud" 

---

##  2. Alcance del MVP

*La solucion propuesta para el problema cosnta de un chat web integrado*
Puede hacer uso y prueba de él haciendo clik [AQUI](https://amjuanmoya.github.io/MediFast/)

- Canal inicial: **Chat web (VoiceFlow)**  
- Entrada: Descripción en lenguaje cotidiano  
- Salida: orientación en base en **3 niveles de urgencia**:
  -  Autocuidado  
  -  Atención temprana (24–48h)  
  -  Emergencia inmediata  

**Fuera de alcance en esta fase:**
- Diagnóstico médico o prescripción de tratamientos   
- Persistencia de datos (BD no requerida para el flujo base)
- Integracion con MCP.



---

## 3. Arquitectura y Componentes

### Flujo de VoiceFlow

<img width="956" height="491" alt="image" src="https://github.com/user-attachments/assets/8a6bc3a4-5a69-4f15-8de5-8ea9bef1615f" />

### Arquitectura del proyecto*

<img width="873" height="427" alt="image" src="https://github.com/user-attachments/assets/691e2680-1faa-4455-983d-7f421a9f0105" />


| Componente                                       | Descripción                                                         | Estado        |
| ------------------------------------------------ | ------------------------------------------------------------------- | ------------- |
| **Frontend (VoiceFlow)**+html with tailwind      | Interfaz conversacional base                                        | ✅ Activo      |
| **Agente IA (api integrada en VoiceFlow)**       | Procesa lenguaje natural,  clasifica urgencia y da la orientacion   | ✅ Integrado   |
| **Orquestador interno VoiceFlow**                | Gestiona flujo conversacional y prompts                             | ✅ Integrado   |
| **MCP (Model Context Protocol)**                 | Punto de conexión contextual                                        | 🔄 En pruebas |
| **A2A Agent (- Interacion directa en Voiceflow)** | Comunicación entre agentes (flujo interno orquestado por VoiceFlow) | ✅ Integrado   |
| **Base De Conocimiento** | Para alimentar los agentes de conocimiento relacionado con primeros auxilios y orentacion medica documentada | ✅ Integrado   |

> 💡 *No se requiere base de datos ni infraestructura compleja en esta versión dado que no se requiere persistencia de datos en esta fase. *

---

## 4. Stack Tecnológico

| Área                        | Herramienta / Tecnología                                                      |
| --------------------------- | ----------------------------------------------------------------------------- |
| Plataforma de Interagracion | VoiceFlow                                                                     |
| Lógica IA                   | Modelos LLM integrados en Voiceflow, , capacidad para intergarse con API Keys |
| Lenguaje                    | bajo codigo en JavaScript /                                         |
| Despliegue                  | VoiceFlow (entorno web) + GitHub Pages                                        |
| Control de versiones        | GitHub (repositorio público)                                                  |

---

## 5. Roles y Responsabilidades

| Rol | Integrante | Función Principal |
|------|-------------|-------------------|
| **BA – Business Analyst** | Samuel Ramos | Documentar requisitos, alcance y casos de uso |
| **QA – Quality Assurance** | Juan Moya | Diseñar pruebas y validar funcionamiento |
| **DEV – Developer** | Isabella Sánchez | Implementar flujos y conexión con la IA |

---

## 6. Pruebas de aceptacion y Validación

- se hizo la verificación de comprensión de respuestas (lenguaje no técnico).  
- Pruebas de flujo conversacional: interpretación → clasificación → orientación.  
- se valido de que el agente **no diagnostica ni prescribe.** en unos casos  
- se probaron escenarios de usuario con distintos niveles de alfabetización.
- 

---


## 7. Licencia y Créditos

**Equipo 03  SmartCode – SENASoft 2025**  
Desarrollo Integral de Software  
**Licencia:** MIT 

---



> _"No se trata de reemplazar al médico, sino de brindar una mano a quien no sabe qué hacer."_  
> — Equipo 03 - SmartCode💙
