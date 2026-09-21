
<div align="center">

<img src="UrbanGuard/Resources/UPClogo.png" width="180" alt="Logo UPC">

# Universidad Peruana de Ciencias Aplicadas

### Carrera de Ingeniería de Software

### **1ASI0729**

### **Desarrollo de Aplicaciones Open Source**

NRC

### **7769**

### **Informe del Trabajo Final**

Docente

### **Mori Paiva, Hugo Allan**

Equipo

### **UrbanGuardle**

Proyecto

### **UrbanGuard**

### **Integrantes**

| Código     | Apellidos y Nombres             |
| ---------- | ------------------------------- |
| U202311082 | Miraval Pomalaya, Rodrigo Jesus |
| U202319398 | Llamozas Diaz, Edson Diego      |
| U202423262 | Reyes Muñoz, Joaquin Leonardo   |
| U20241A322 | Blancas Chavez, Carlos Franco   |
| U202412447 | Portal Inga, Waldo Alonso       |

### **Período 202620**

**Septiembre 2026**
---
| Versión | Fecha | Autor/es | Descripción de Modificación |
|---------|-------|----------|-----------------------------|
| 0.1 | 20/09/2026 | Todos los integrantes | Agregación de: Carátula, Registro de Versiones del Informe, Project Report Collaboration Insights, Contenido (Índice), Student Outcome, Capítulo I: Introducción, Capítulo II: Requirements Elicitation & Analysis, Capítulo III: Requirements Specification, Capítulo IV: Product Design, Capítulo V: Product Implementation, Validation & Deployment. Avance de: Conclusiones, Bibliografía, Anexos. |
---
</div>

## Project Report Collaboration Insights

**Project Report URL:** https://github.com/G3-Avisum-OpenSource/informe-proyecto

El presente apartado tiene como finalidad evidenciar el trabajo colaborativo realizado durante la elaboración del informe del proyecto. Para ello, se considera como fuente principal el repositorio oficial del informe, alojado en GitHub bajo la organización del equipo: [https://github.com/OpenSource-Grupo-1](https://github.com/G3-Avisum-OpenSource/informe-proyecto)

A partir de este repositorio, se analiza la participación de los integrantes mediante indicadores como la distribución de tareas, la frecuencia de contribuciones, la revisión de contenidos y la integración progresiva de los entregables desarrollados durante el avance del proyecto.

En el contexto de la entrega correspondiente a AV1, el análisis de colaboración permite visualizar el aporte individual de cada miembro del equipo, sustentado en los registros de GitHub, la organización de responsabilidades y la evolución del informe. Este seguimiento busca demostrar una distribución ordenada del trabajo, la consistencia en la documentación y el cumplimiento de las actividades asignadas.

### AV1

Durante el desarrollo de la entrega AV1, el equipo organizó la elaboración del informe mediante la asignación de responsabilidades por secciones. Esta distribución permitió avanzar de manera paralela en actividades relacionadas con investigación, análisis del segmento objetivo, definición de requisitos, diseño UX, modelado del dominio, arquitectura de software y documentación técnica.

El proceso de desarrollo del informe se realizó de forma incremental, incorporando progresivamente los contenidos conforme se consolidaban los artefactos del proyecto. Esto se refleja en el Registro de Versiones del Informe, donde se evidencia la evolución del documento desde su estructura inicial hasta la inclusión de elementos como Lean UX, entrevistas, user stories, impact maps, event storming, bounded contexts, diagramas C4, diagramas de clases, diseño de base de datos y evidencias de implementación.

Asimismo, todos los integrantes participaron activamente en la construcción del informe, realizando aportes continuos que permitieron consolidar una documentación coherente y alineada entre sus distintas secciones. La colaboración se evidencia tanto en la planificación de tareas como en los cambios registrados en el repositorio, los cuales reflejan la participación distribuida del equipo.

---
# Contenido

- [Carátula](#universidad-peruana-de-ciencias-aplicadas)
- [Registro de Versiones del Informe](#registro-de-versiones-del-informe)
- [Project Report Collaboration Insights](#project-report-collaboration-insights)
- [Contenido](#contenido)
- [Student Outcome](#student-outcome)

- [Capítulo I: Introducción](UrbanGuard/Resources/Chapter1.md)
    - [1.1. Startup Profile](UrbanGuard/Resources/Chapter1.md#11-startup-profile)
        - [1.1.1. Descripción de la Startup](UrbanGuard/Resources/Chapter1.md#111-descripción-de-la-startup)
        - [1.1.2. Perfiles de integrantes del equipo](UrbanGuard/Resources/Chapter1.md#112-perfiles-de-integrantes-del-equipo)
    - [1.2. Solution Profile](UrbanGuard/Resources/Chapter1.md#12-solution-profile)
        - [1.2.1. Antecedentes y problemática](UrbanGuard/Resources/Chapter1.md#121-antecedentes-y-problemática)
        - [1.2.2. Lean UX Process](UrbanGuard/Resources/Chapter1.md#122-lean-ux-process)
            - [1.2.2.1. Lean UX Problem Statements](UrbanGuard/Resources/Chapter1.md#1221-lean-ux-problem-statements)
            - [1.2.2.2. Lean UX Assumptions](UrbanGuard/Resources/Chapter1.md#1222-lean-ux-assumptions)
            - [1.2.2.3. Lean UX Hypothesis Statements](UrbanGuard/Resources/Chapter1.md#1223-lean-ux-hypothesis-statements)
            - [1.2.2.4. Lean UX Canvas](UrbanGuard/Resources/Chapter1.md#1224-lean-ux-canvas)
    - [1.3. Segmentos objetivo](UrbanGuard/Resources/Chapter1.md#13-segmentos-objetivo)

- [Capítulo II: Requirements Elicitation & Analysis](UrbanGuard/Resources/Chapter2.md)
    - [2.1. Competidores](UrbanGuard/Resources/Chapter2.md#21-competidores)
        - [2.1.1. Análisis Competitivo](UrbanGuard/Resources/Chapter2.md#211-análisis-competitivo)
        - [2.1.2. Estrategia y tácticas frente a competidores](UrbanGuard/Resources/Chapter2.md#212-estrategia-y-tácticas-frente-a-competidores)
    - [2.2. Entrevistas](UrbanGuard/Resources/Chapter2.md#22-entrevistas)
        - [2.2.1. Diseño de entrevistas](UrbanGuard/Resources/Chapter2.md#221-diseño-de-entrevistas)
        - [2.2.2. Registro de entrevistas](UrbanGuard/Resources/Chapter2.md#222-registro-de-entrevistas)
        - [2.2.3. Análisis de entrevistas](UrbanGuard/Resources/Chapter2.md#223-análisis-de-entrevistas)
    - [2.3. Needfinding](UrbanGuard/Resources/Chapter2.md#23-needfinding)
        - [2.3.1. User Personas](UrbanGuard/Resources/Chapter2.md#231-user-personas)
        - [2.3.2. User Task Matrix](UrbanGuard/Resources/Chapter2.md#232-user-task-matrix)
        - [2.3.3. User Journey Mapping](UrbanGuard/Resources/Chapter2.md#233-user-journey-mapping)
        - [2.3.4. Empathy Mapping](UrbanGuard/Resources/Chapter2.md#234-empathy-mapping)
    - [2.4. Big Picture EventStorming](UrbanGuard/Resources/Chapter2.md#24-big-picture-eventstorming)
    - [2.5. Ubiquitous Language](UrbanGuard/Resources/Chapter2.md#25-ubiquitous-language)

- [Capítulo III: Requirements Specification](UrbanGuard/Resources/Chapter3.md)
    - [3.1. User Stories](UrbanGuard/Resources/Chapter3.md#31-user-stories)
    - [3.2. Impact Mapping](UrbanGuard/Resources/Chapter3.md#32-impact-mapping)
    - [3.3. Product Backlog](UrbanGuard/Resources/Chapter3.md#33-product-backlog)

- [Capítulo IV: Product Design](UrbanGuard/Resources/Chapter4.md)
    - [4.1. Style Guidelines](UrbanGuard/Resources/Chapter4.md#41-style-guidelines)
        - [4.1.1. General Style Guidelines](UrbanGuard/Resources/Chapter4.md#411-general-style-guidelines)
        - [4.1.2. Web Style Guidelines](UrbanGuard/Resources/Chapter4.md#412-web-style-guidelines)
    - [4.2. Information Architecture](UrbanGuard/Resources/Chapter4.md#42-information-architecture)
        - [4.2.1. Organization Systems](UrbanGuard/Resources/Chapter4.md#421-organization-systems)
        - [4.2.2. Labeling Systems](UrbanGuard/Resources/Chapter4.md#422-labeling-systems)
        - [4.2.3. SEO Tags and Meta Tags](UrbanGuard/Resources/Chapter4.md#423-seo-tags-and-meta-tags)
        - [4.2.4. Searching Systems](UrbanGuard/Resources/Chapter4.md#424-searching-systems)
        - [4.2.5. Navigation Systems](UrbanGuard/Resources/Chapter4.md#425-navigation-systems)
    - [4.3. Landing Page UI Design](UrbanGuard/Resources/Chapter4.md#43-landing-page-ui-design)
        - [4.3.1. Landing Page Wireframe](UrbanGuard/Resources/Chapter4.md#431-landing-page-wireframe)
        - [4.3.2. Landing Page Mock-up](UrbanGuard/Resources/Chapter4.md#432-landing-page-mock-up)
    - [4.4. Web Applications UX/UI Design](UrbanGuard/Resources/Chapter4.md#44-web-applications-uxui-design)
        - [4.4.1. Web Applications Wireframes](UrbanGuard/Resources/Chapter4.md#441-web-applications-wireframes)
        - [4.4.2. Web Applications Wireflow Diagrams](UrbanGuard/Resources/Chapter4.md#442-web-applications-wireflow-diagrams)
        - [4.4.3. Web Applications Mock-ups](UrbanGuard/Resources/Chapter4.md#443-web-applications-mock-ups)
        - [4.4.4. Web Applications User Flow Diagrams](UrbanGuard/Resources/Chapter4.md#444-web-applications-user-flow-diagrams)
    - [4.5. Web Applications Prototyping](UrbanGuard/Resources/Chapter4.md#45-web-applications-prototyping)
    - [4.6. Domain-Driven Software Architecture](UrbanGuard/Resources/Chapter4.md#46-domain-driven-software-architecture)
        - [4.6.1. Design-Level Event Storming](UrbanGuard/Resources/Chapter4.md#461-design-level-event-storming)
        - [4.6.2. Software Architecture Context Diagram](UrbanGuard/Resources/Chapter4.md#462-software-architecture-context-diagram)
        - [4.6.3. Software Architecture Container Diagrams](UrbanGuard/Resources/Chapter4.md#463-software-architecture-container-diagrams)
        - [4.6.4. Software Architecture Components Diagrams](UrbanGuard/Resources/Chapter4.md#464-software-architecture-components-diagrams)
    - [4.7. Software Object-Oriented Design](UrbanGuard/Resources/Chapter4.md#47-software-object-oriented-design)
        - [4.7.1. Class Diagrams](UrbanGuard/Resources/Chapter4.md#471-class-diagrams)
    - [4.8. Database Design](UrbanGuard/Resources/Chapter4.md#48-database-design)
        - [4.8.1. Database Diagrams](UrbanGuard/Resources/Chapter4.md#481-database-diagrams)

- [Capítulo V: Product Implementation, Validation & Deployment](UrbanGuard/Resources/Chapter5.md)
    - [5.1. Software Configuration Management](UrbanGuard/Resources/Chapter5.md#51-software-configuration-management)
        - [5.1.1. Software Development Environment Configuration](UrbanGuard/Resources/Chapter5.md#511-software-development-environment-configuration)
        - [5.1.2. Source Code Management](UrbanGuard/Resources/Chapter5.md#512-source-code-management)
        - [5.1.3. Source Code Style Guide & Coding Conventions](UrbanGuard/Resources/Chapter5.md#513-source-code-style-guide--coding-conventions)
    - [5.2. Landing Page, Services & Applications Implementation](UrbanGuard/Resources/Chapter5.md#52-landing-page-services--applications-implementation)
        - [5.2.1. Sprint 1](UrbanGuard/Resources/Chapter5.md#521-sprint-1)
            - [5.2.1.1. Sprint Planning 1](UrbanGuard/Chapter5.md#5211-sprint-planning-1)
            - [5.2.1.2. Aspect Leaders and Collaborators](UrbanGuard/Resources/Chapter5.md#5212-aspect-leaders-and-collaborators)
            - [5.2.1.3. Sprint Backlog 1](UrbanGuard/Resources/Chapter5.md#5213-sprint-backlog-1)
            - [5.2.1.4. Development Evidence for Sprint Review](UrbanGuard/Resources/Chapter5.md#5214-development-evidence-for-sprint-review)
            - [5.2.1.5. Execution Evidence for Sprint Review](UrbanGuard/Resources/Chapter5.md#5215-execution-evidence-for-sprint-review)
            - [5.2.1.6. Services Documentation Evidence for Sprint Review](UrbanGuard/Resources/Chapter5.md#5216-services-documentation-evidence-for-sprint-review)
            - [5.2.1.7. Software Deployment Evidence for Sprint Review](UrbanGuard/Resources/Chapter5.md#5217-software-deployment-evidence-for-sprint-review)
            - [5.2.1.8. Team Collaboration Insights during Sprint](UrbanGuard/Resources/Chapter5.md#5218-team-collaboration-insights-during-sprint)

---

## Student Outcome

En Ingeniería de Software el logro contribuye a alcanzar el Student Outcome EAC 3:
> *"Demonstrates an ability to communicate effectively with a range of audiences"*

| Criterio Específico | Evidencias por entrega | Conclusiones |
|---------------------|-------------------------|--------------|
| **3.c1. Comunica oralmente con efectividad a diferentes rangos de audiencia** | **AV1**<br>• Llamozas Diaz, Edson Diego: Services Documentation Evidence y Software Deployment Evidence.<br>• Reyes Muñoz, Joaquin Leonardo: Development Evidence y Team Collaboration Insights.<br>• Blancas Chavez, Carlos Franco: Sprint Backlog 1.<br>• Portal Inga, Waldo Alonso: Execution Evidence. | A través de la AV1, el equipo fortaleció su capacidad para comunicar oralmente los avances y resultados del proyecto, participando en la presentación de las evidencias y explicando de manera clara los aportes realizados durante el desarrollo del proyecto. |
| **3.c2. Comunica por escrito con efectividad a diferentes rangos de audiencia** | **AV1**<br>• Llamozas Diaz, Edson Diego: Services Documentation Evidence y Software Deployment Evidence.<br>• Reyes Muñoz, Joaquin Leonardo: Development Evidence y Team Collaboration Insights.<br>• Blancas Chavez, Carlos Franco: Sprint Backlog 1.<br>• Portal Inga, Waldo Alonso: Execution Evidence. | En la Av1, el equipo desarrolló y organizó la documentación correspondiente a los diferentes artefactos del proyecto, permitiendo comunicar de manera clara y estructurada los avances, actividades y resultados obtenidos durante el desarrollo. |









