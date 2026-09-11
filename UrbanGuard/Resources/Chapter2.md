## Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores

### 2.1.1. Análisis Competitivo

| Competitive Analysis Landscape | | | |
|---|---|---|---|
| **¿Por qué llevar a cabo este análisis?** | Identificar ventajas competitivas frente a soluciones existentes de monitoreo y seguridad en el transporte público peruano. | | |
| | **Avisum (Nuestra startup)** | **Competidor 1 : Visor ATU-PNP contra la extorsión (SICM)** | **Competidor 2 : Sistema IVU del Corredor Rojo (ATU)** |
| **Ventaja competitiva** | Verificación de identidad del conductor por código digital, botón de pánico individual con respuesta directa a la empresa, y monitoreo GPS accesible para consorcios pequeños y medianos sin depender de gestión estatal. | Cruza en un mismo mapa la ubicación de ~12,000 unidades de transporte con la de los patrulleros policiales, permitiendo respuesta coordinada con la PNP ante emergencias. | Permite que el propio conductor reporte en tiempo real robos, acoso o accidentes directamente a un Centro de Gestión y Control específico del corredor. |
| **Mercado objetivo** | Conductores y consorcios de transporte urbano formal e informal, sin importar su tamaño. | Empresas de transporte regular registradas ante la ATU, en coordinación con la PNP. | Conductores y operadores exclusivamente del Corredor Rojo (una sola ruta). |
| **Estrategia de posicionamiento** | Solución independiente y ágil, adoptable por cualquier consorcio sin depender de trámites o integración estatal. | Herramienta de fiscalización y seguridad pública, posicionada como respuesta directa del Estado a la crisis de extorsión. | Mejora puntual de experiencia y seguridad dentro de un corredor específico ya gestionado por el Estado. |
| **Productos y servicios** | Verificación de conductor, botón de pánico, panel de monitoreo de flota en tiempo real. | Mapa interactivo con ubicación de buses y patrulleros, mapas de calor de puntos críticos. | Reporte de incidentes por parte del conductor, tótems informativos, monitoreo desde un centro de control central. |
| **Costos / acceso** | Modelo de suscripción mensual por unidad, accesible para consorcios pequeños. | Gratuito para las empresas registradas, pero requiere cumplir los lineamientos técnicos de GPS exigidos por la ATU (IMEI, precisión de 3 metros, batería de respaldo de 5 horas, entre otros). | Gestionado íntegramente por el Estado; sin costo directo para el conductor, pero limitado a un solo corredor. |
| **Canales de implementación** | Registro directo vía web/app, sin trámites regulatorios previos. | Integración técnica obligatoria al Sistema Integrado de Control y Monitoreo (SICM) de la ATU. | Infraestructura fija instalada por el Estado (tótems, centro de control). |
| **Fortalezas** | Rapidez de adopción, foco en la experiencia individual del conductor, sin depender de trámites estatales. | Respaldo institucional y capacidad de coordinación directa con la PNP. | Ya operativo y probado en un corredor real, con reportes de incidentes funcionando en producción. |
| **Oportunidades** | Expandirse a consorcios que aún no califican para integrarse al sistema estatal por requisitos técnicos o de formalización. | Ampliar cobertura a más de las 12,000 unidades ya registradas conforme se sumen más empresas. | Replicar el modelo IVU a otros corredores complementarios. |
| **Amenazas** | Que el Estado extienda gratuitamente funcionalidades similares a más empresas, reduciendo el incentivo de pagar por una solución privada. | Dependencia de que las empresas cumplan con los estrictos requisitos técnicos de GPS exigidos por la nueva normativa 2026. | Alcance limitado a un solo corredor, sin capacidad de escalar rápido a toda Lima. |

### 2.1.2. Estrategia y tácticas frente a competidores

**Frente al Visor ATU-PNP contra la extorsión (SICM):**
Avisum se posiciona como un complemento ágil y no como un sustituto de la fiscalización estatal  mientras el sistema de la ATU depende de la integración regulatoria y de que la empresa cumpla especificaciones técnicas estrictas de GPS, Avisum puede adoptarse de inmediato por cualquier consorcio, sin trámites previos, funcionando como una primera capa de seguridad mientras la empresa eventualmente se integra (o no) al sistema estatal.

**Frente al Sistema IVU del Corredor Rojo:**
Avisum toma como validación de mercado que el propio Estado ya reconoce el valor de que un conductor pueda reportar incidentes en tiempo real , pero mientras el IVU está limitado a una sola ruta con infraestructura fija instalada por el Estado, Avisum está diseñado para escalar a cualquier consorcio de transporte urbano de Lima y Callao sin depender de inversión en infraestructura física.

**Diferenciación tecnológica y funcional:**
1. **Verificación de identidad como puerta de entrada.** A diferencia de los sistemas estatales, que se centran en monitorear la unidad, Avisum parte de verificar primero que la persona al volante sea quien dice ser  una capa de seguridad que ningún competidor actual ofrece de forma accesible para consorcios pequeños.
2. **Botón de pánico orientado al conductor individual.** Mientras los sistemas estatales priorizan la coordinación institucional (ATU-PNP), Avisum pone el control directamente en manos del conductor, con una respuesta que llega primero a su propia empresa.
3. **Sin barrera de entrada regulatoria.** Cualquier consorcio, formal o en proceso de formalización, puede empezar a usar Avisum sin esperar a cumplir los lineamientos técnicos exigidos por la ATU para integrarse al SICM.

**Posicionamiento y enfoque de mercado:**
1. **Seguridad como valor central, no como cumplimiento normativo.** Avisum se comunica como una herramienta de protección real para el conductor, no como una obligación regulatoria.
2. **Foco inicial en consorcios pequeños y medianos.** Se prioriza el segmento que hoy queda fuera del alcance de los sistemas estatales por no cumplir los requisitos técnicos de integración.
3. **Adaptación al contexto real peruano.** El diseño de Avisum parte de la problemática documentada de extorsión y sicariato contra transportistas, no de un modelo genérico importado de otro país.
4. **Alianzas a futuro con el Estado.** Aunque Avisum nace como solución privada, se identifica como oportunidad a mediano plazo la interoperabilidad con el SICM de la ATU, para complementar —no competir con— los esfuerzos estatales de fiscalización.

### 2.2. Entrevistas

#### 2.2.1. Diseño de entrevistas

**Segmento: Conductores (operarios) de transporte público**

1. ¿Cómo es un día típico para ti desde que inicias hasta que terminas tu jornada manejando?
2. ¿En qué momentos del día te sientes más expuesto al peligro o inseguro mientras trabajas?
3. ¿Qué tan frecuente es que los conductores reciban amenazas, cobros de cupo o extorsión?
4. ¿Qué medidas de seguridad tienes actualmente en tu unidad?
5. ¿Qué tan importante crees que sería que alguien monitoree tu ubicación en tiempo real?
6. ¿Qué tan rápido puedes pedir ayuda hoy en día si pasa algo dentro del vehículo?
7. ¿Qué sientes que falta para que tu trabajo sea más seguro?
8. ¿Qué tan cómodo te sentirías usando una app que verifique tu identidad y monitoree tu turno?
9. ¿Qué opinas de validar tu identidad con un código digital antes de manejar?
10. ¿En qué momento del día usarías más una solución como esta?

**Segmento: Empresas o consorcios de transporte público**

1. ¿Cómo gestionan actualmente la seguridad de sus conductores y pasajeros?
2. ¿Cuáles son los principales problemas de seguridad que enfrentan hoy?
3. ¿Qué tan frecuente es enfrentar extorsión, robos o incidentes dentro de las unidades?
4. ¿Qué impacto tienen estos problemas en su operación (costos, reputación, continuidad)?
5. Cuando ocurre una emergencia, ¿cómo se enteran y qué tan rápido pueden actuar?
6. ¿Qué tan difícil es supervisar en tiempo real lo que sucede en cada unidad?
7. ¿Cómo verifican actualmente que el conductor asignado sea el correcto?
8. ¿Han tenido problemas con conductores no autorizados o mal identificados?
9. Con una herramienta digital en tiempo real, ¿qué aspectos les ayudaría a mejorar?
10. Si implementaran este sistema, ¿qué les preocuparía antes de usarlo?

#### 2.2.2. Registro de entrevistas

User: Conductores (operarios) de transporte público

Entrevistado: Matías Aguilar

•	Edad
•	Distrito
•	Link del video:	https://youtu.be/Rs30FpZu3PA 


   

*(Pendiente — se completará una vez el equipo realice las entrevistas reales a conductores y representantes de empresas de transporte. Formato sugerido por entrevistado: nombre, edad, distrito, link de video, y resumen de 5-8 líneas destacando su rutina, percepción de riesgo, medidas de seguridad actuales, y disposición a usar Avisum.)*

#### 2.2.3. Análisis de entrevistas

*(Pendiente — se completará tras el registro de entrevistas)*

### 2.3. Needfinding

Para identificar las necesidades reales de nuestros usuarios, complementamos las entrevistas con herramientas de needfinding que nos permiten representar y comprender a profundidad a cada segmento objetivo.

#### 2.3.1. User Personas

**Segmento #1: Conductores (operarios) de transporte público**

*(Pendiente )*

**Segmento #2: Empresas o consorcios de transporte público**

*(Pendiente *

#### 2.3.2. User Task Matrix

**Segmento objetivo #1 — Conductores**

| Actividades | Frecuencia | Importancia |
|---|---|---|
| Iniciar jornada y verificar el estado de la unidad antes de salir | Con frecuencia | Alta |
| Confirmar la ruta asignada y horario de salida con la empresa | Con frecuencia | Alta |
| Cobrar pasaje y controlar el flujo de pasajeros | Con frecuencia | Alta |
| Reportar incidentes al encargado de la empresa | A veces | Alta |
| Evaluar zonas de riesgo durante la ruta y tomar desvíos si es necesario | Frecuente | Alta |
| Pagar cuota o cupo a personas externas que operan en la ruta | Frecuente | Media |
| Comunicarse con otros conductores ante situaciones de riesgo | A veces | Alta |
| Registrar el cierre de turno y entregar la unidad al siguiente conductor | Con frecuencia | Alta |

**Segmento objetivo #2 — Empresas de transporte**

| Actividades | Frecuencia | Importancia |
|---|---|---|
| Supervisar las unidades de transporte en ruta | Con frecuencia | Alta |
| Coordinar con conductores durante la jornada | Con frecuencia | Alta |
| Atender incidentes o reportes de seguridad | Con frecuencia | Alta |
| Comunicarse con autoridades ante emergencias | A veces | Alta |
| Verificar documentación e identidad de conductores | A veces | Media |
| Gestionar problemas de extorsión o amenazas | Con frecuencia | Alta |
| Revisar estado operativo de las unidades | Con frecuencia | Alta |
| Evaluar la implementación de nuevas tecnologías de seguridad | A veces | Media |

#### 2.3.3. User Journey Mapping

*(Pendiente — se construirá en Figma representando el recorrido del conductor durante un cambio de turno: desde que recibe la unidad hasta que la entrega, marcando puntos de fricción y emociones en cada etapa. Mismo ejercicio para el representante de empresa durante su jornada de supervisión.)*

#### 2.3.4. Empathy Mapping

*(Pendiente — mapa de empatía por segmento cubriendo qué piensa, siente, ve, dice y hace cada usuario, y sus frustraciones y motivaciones principales frente al problema de inseguridad en el transporte.)*

### 2.4. Big Picture EventStorming

*(Pendiente — sesión de Event Storming a realizar con el equipo, cubriendo los pasos: 1. Exploración no estructurada de eventos, 2. Líneas de tiempo, 3. Puntos de dolor, 4. Puntos pivote, 5. Comandos, 6. Políticas, 7. Read Models, 8. Agregados. Documentar cada paso con una captura del tablero colaborativo, en Miro o FigJam.)*

### 2.5. Ubiquitous Language

**Transport Unit (Unidad de Transporte):** Vehículo que forma parte del sistema y es objeto de monitoreo, sobre el cual se realiza seguimiento de ubicación, estado y eventos.

**Driver (Conductor):** Persona responsable de operar una unidad de transporte durante un recorrido, asociada a una unidad y capaz de generar eventos relevantes durante la operación.

**Route (Ruta):** Trayecto definido que sigue una unidad de transporte, incluyendo punto de inicio, paradas y destino final.

**Trip (Viaje):** Recorrido específico realizado por una unidad dentro de una ruta en un periodo determinado.

**Real-Time Monitoring (Monitoreo en Tiempo Real):** Seguimiento continuo de la ubicación y estado de las unidades durante la operación.

**Unit Status (Estado de Unidad):** Condición actual de una unidad dentro del sistema — en operación, detenida o en alerta.

**Security Event (Evento de Seguridad):** Situación relevante ocurrida durante un viaje que puede afectar la operación o la seguridad.

**Panic Alert (Alerta de Pánico):** Señal de emergencia activada manualmente por el conductor ante una situación de peligro.

**Critical Alert (Alerta Crítica):** Notificación de alta prioridad generada ante un riesgo que requiere atención inmediata.

**Fleet (Flota):** Conjunto de unidades de transporte gestionadas dentro del sistema.

**Incident (Incidente):** Evento inesperado que afecta el desarrollo normal de un viaje, pudiendo requerir intervención.

**Tracking (Seguimiento):** Proceso de observar y registrar la ubicación de una unidad a lo largo del tiempo.

**Operational Control (Control Operativo):** Supervisión general de unidades, viajes y eventos para asegurar el correcto funcionamiento del servicio.

**Alert Level (Nivel de Alerta):** Clasificación de la gravedad de una alerta, que permite priorizar su atención.
