# Capítulo I: Introducción

## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup

**Avisum** nace como respuesta tecnológica a un problema que millones de peruanos enfrentan a diario sin darse cuenta: subir a un bus o combi sin saber realmente quién lo conduce, y sin ninguna garantía de que, si algo sale mal durante el trayecto, alguien pueda enterarse a tiempo.

El nombre "Avisum" resume la idea central del producto: un sistema que **avisa** — al pasajero sobre quién lo transporta, al conductor sobre que tiene respaldo ante una emergencia, y a la empresa sobre dónde y cómo está operando su flota en cada momento.

Concretamente, la plataforma resuelve tres necesidades simultáneas dentro del ecosistema del transporte público:

1. Confirmar que la persona al volante es quien dice ser, mediante un código de verificación asignado a cada conductor.
2. Dar al conductor una vía inmediata para pedir ayuda si percibe una amenaza — desde un asalto hasta una falla mecánica en zona de riesgo.
3. Permitir que la operadora del servicio sepa en todo momento dónde está cada unidad de su flota, sin depender de llamadas o reportes manuales.

**Misión:** Reducir la exposición al riesgo de quienes dependen del transporte público — pasajeros y conductores por igual — a través de herramientas digitales simples que verifiquen identidad, habiliten respuesta inmediata ante emergencias y den visibilidad operativa a las empresas de transporte.

**Visión:** Que ninguna persona en Latinoamérica tenga que subir a una unidad de transporte público sin la certeza de que existe un sistema vigilando su seguridad en tiempo real.

### 1.1.2. Perfiles de integrantes del equipo


|                     Foto de perfil                      | Nombre Completo                      | Carrera                | Habilidades                                                                                                         |
| :-----------------------------------------------------: | :----------------------------------- | :--------------------- | :------------------------------------------------------------------------------------------------------------------ |
| !  |    | Ingenieria de Software |                                                                        |
|     !     | Reyes Muñoz, Joaquin Leonardo | Ingenieria de Software |  C++, Java, MySQL,PostgreSQL,MongoDB, Python, C#                      |
| ![CarlosFoto](Resources/img/carlos.png) | Blancas Chávez, Carlos Franco      | Ingenieria de Software | Typscript, React,Vue, Java, MySQL,PostgreSQL,MongoDB, Python, C#                                                               |
| ! |                      | Ingenieria de Software |  |
|  !  |  | Ingenieria de Software |                    
---


## 1.2. Solution Profile

### 1.2.1. Antecedentes y problemática

Para entender mejor la problemática, aplicamos la técnica **5W's & 2H's**, complementada con evidencia estadística verificable de fuentes periodísticas y oficiales.

**What (Qué) — ¿Cuál es el problema?**

Los pasajeros del transporte público urbano no tienen forma de verificar si el conductor que opera la unidad es la persona autorizada, y los propios conductores no cuentan con ningún canal digital para pedir auxilio inmediato ante una situación de riesgo. A esto se suma que las empresas de transporte no tienen visibilidad en tiempo real de sus unidades una vez que salen a ruta.

**When (Cuándo) — ¿Cuándo sucede el problema?**

En cada servicio de transporte, con mayor incidencia en horarios nocturnos y en rutas con menor supervisión policial. Los ataques contra unidades de transporte ocurren en promedio 3 veces por semana según reportes recientes del sector (Infobae, julio 2026).

**Where (Dónde) — ¿Dónde ocurre el problema?**

El problema afecta principalmente Lima Metropolitana y Callao, con especial concentración en el Cono Norte, Cono Sur y Cono Este, zonas donde las organizaciones criminales se disputan el control de rutas mediante amenazas y cobro de cupos (Infobae, julio 2026).

**Who (Quién) — ¿A quiénes les sucede el problema?**

A los pasajeros, que no tienen forma de verificar la identidad del conductor; a los conductores, expuestos diariamente a extorsión, amenazas y ataques armados; y a las empresas operadoras, que no tienen visibilidad de sus unidades ni capacidad de respuesta oportuna ante incidentes.

**Why (Por qué) — ¿Cuál es la causa del problema?**

La ausencia de tecnología de identificación y trazabilidad en el transporte público. No existen canales de emergencia directos entre el conductor y una central de operaciones, ni herramientas que permitan a las empresas monitorear su flota en tiempo real.

**How (Cómo) — ¿Cómo afecta este problema?**

La violencia contra el transporte ha escalado de forma sostenida: según el Observatorio del Crimen y la Violencia, en 2025 fueron asesinados 239 transportistas a nivel nacional, un promedio cercano a 20 por mes (RPP, junio 2026). Esta violencia ha llevado a que algunos conductores opten por portar armas de fuego para defenderse (Diario Correo, 2026), y a que decenas abandonen sus puestos de trabajo por miedo.

**How Much (Cuánto) — ¿Qué datos respaldan la problemática?**

- Según el comandante general de la Policía Nacional del Perú (PNP), Óscar Arriola, **64 conductores de transporte público fueron asesinados** entre enero y junio de 2026 por bandas vinculadas a la extorsión y el sicariato (Infobae, junio 2026).
- Otro reportaje, con corte a fines de julio de 2026, eleva la cifra a **72 choferes asesinados** en lo que va del año, superando ya el total de ataques registrados en todo el 2025 (Diario Correo, 2026; La Noticia Perú, 2026).
- Según el Ministerio Público, durante el año 2025 murieron **75 personas** en hechos de extorsión vinculados al sector transporte a nivel nacional (Perú21, junio 2026), mientras que la Alianza Nacional de Transportistas eleva esa cifra a **más de 80 transportistas asesinados** en 2025 considerando todas las modalidades (mototaxistas, taxistas, colectiveros, camioneros) (Infobae, enero 2026).
- El director de la Cámara Internacional de Logística y Transporte, Martín Ojeda, reportó un promedio de **3 atentados armados por semana** contra empresas de transporte solo en Lima y Callao (Infobae, julio 2026).
- Frente a esta crisis, el Estado peruano promulgó la **Ley N.° 32490**, que contempla compensaciones e indemnizaciones para los deudos de conductores asesinados por extorsión (La República, marzo 2026) — evidencia de que el problema ya es reconocido a nivel estatal, aunque los propios transportistas denuncian que las medidas prometidas aún no se traducen en resultados concretos.

### 1.2.2. Lean UX Process

Aquí se aplica Lean UX Process y abarca la visión del modelo de negocio que será soportado por el producto de software, incluyendo Problem Statements (incluyendo aspectos como domain, customer segments, pain points, gap, visión/strategy, e initial segment), Assumptions e Hypothesis Statements según Lean UX Process. Finalizando esta sección se incluye el Lean UX Canvas.

#### 1.2.2.1. Lean UX Problem Statements

**Problem Statement 1 — Conductores de transporte público**

| Elemento | Descripción |
|---|---|
| **Domain** | Seguridad y respuesta ante emergencias en el transporte público urbano. |
| **Customer Segments** | Conductores (operarios) de unidades de transporte público en Lima Metropolitana y Callao. |
| **Pain Points** | Exposición constante a extorsión, amenazas armadas y agresiones durante su jornada laboral, sin ningún canal digital para pedir auxilio inmediato ante una emergencia. |
| **Gap** | No existe en el mercado peruano una solución accesible que conecte al conductor con una central de respuesta en tiempo real durante su turno de trabajo. |
| **Vision/Strategy** | Brindar al conductor una herramienta de verificación de identidad y alerta de pánico integrada a su flujo operativo diario, sin fricción y de respuesta inmediata. |
| **Initial Segment** | Conductores de empresas formales de transporte urbano dispuestas a pilotear la solución en rutas de alto riesgo. |

**Problem Statement 2 — Empresas o consorcios de transporte público**

| Elemento | Descripción |
|---|---|
| **Domain** | Monitoreo operativo y gestión de riesgo de flotas de transporte público. |
| **Customer Segments** | Empresas y consorcios de transporte público con más de dos unidades en Lima Metropolitana y Callao. |
| **Pain Points** | Falta de visibilidad en tiempo real de sus unidades y conductores, lo que impide reaccionar oportunamente ante incidentes de extorsión, asalto o accidente. |
| **Gap** | Las herramientas de gestión de flotas existentes en el mercado están orientadas a logística y mantenimiento vehicular, no a la seguridad de las personas a bordo. |
| **Vision/Strategy** | Proveer a las empresas un panel de monitoreo en tiempo real que centralice la ubicación de sus unidades y las alertas generadas por sus conductores, permitiendo una respuesta operativa más rápida. |
| **Initial Segment** | Pequeños y medianos consorcios de transporte urbano formal que ya reportan haber sido víctimas de extorsión o ataques a sus unidades. |

#### 1.2.2.2. Lean UX Assumptions

- Un conductor usará un botón de pánico solo si confía en que la respuesta del otro lado será rápida y real, no simbólica.
- Un pasajero que puede verificar la identidad del conductor percibirá el servicio como más confiable.
- Las empresas de transporte adoptarán un sistema de monitoreo si perciben una reducción tangible en su exposición ante incidentes de extorsión y violencia.
- El seguimiento GPS constante no debe consumir batería ni datos de forma perceptible para el conductor, o dejará de usarse.
- La verificación de identidad debe tomar segundos, no minutos, o se reducirá su adopción.

#### 1.2.2.3. Lean UX Hypothesis Statements

**Hypothesis Statement 1:** Creemos que al permitir que el conductor verifique su identidad mediante un código digital antes de iniciar su turno, aumentaremos la percepción de seguridad de los pasajeros al abordar la unidad. Sabremos que esto es cierto cuando al menos el 60% de los pasajeros encuestados reporten mayor confianza en el servicio tras conocer la funcionalidad.

**Hypothesis Statement 2:** Creemos que al ofrecer un botón de pánico conectado en tiempo real a una central de operaciones, reduciremos el tiempo de respuesta ante una emergencia reportada por el conductor. Sabremos que esto es cierto cuando el tiempo entre la activación de la alerta y su primera atención sea menor a 2 minutos en al menos el 70% de los casos simulados.

**Hypothesis Statement 3:** Creemos que al brindar a las empresas de transporte un panel de monitoreo en tiempo real de su flota, mejoraremos su capacidad de reacción operativa ante incidentes. Sabremos que esto es cierto cuando el tiempo de identificación de una unidad en alerta se reduzca en al menos un 30% respecto al proceso manual actual.

#### 1.2.2.4. Lean UX Canvas

[LeanUxCanvas](LenUxCanvassAvisum.png) 

## 1.3. Segmentos objetivo

| Segmento objetivo | Perfil del segmento | Evidencia estadística |
|---|---|---|
| **Conductores (operarios) de transporte público** | Hombres y mujeres desde los 24 años, a cargo de una o dos unidades asignadas por una empresa-ruta. Concentrados en Lima Metropolitana y Callao, especialmente en zonas de mayor incidencia delictiva como el Cono Norte, Cono Sur y Cono Este. Su prioridad diaria es llegar a casa sin incidentes, tanto para ellos como para sus pasajeros. | Entre enero y junio de 2026, la PNP reportó **64 conductores de transporte público asesinados** por bandas de extorsión y sicariato (Infobae, junio 2026); para fines de julio, otro reportaje eleva la cifra a **72 choferes** en lo que va del año (Diario Correo, 2026). Ante esta violencia, algunos conductores han optado por portar armas de fuego para defenderse. |
| **Empresas o consorcios de transporte público** | Representantes legales o administradores desde los 28 años, a cargo de flotas de más de dos unidades operando bajo rutas formalizadas en Lima Metropolitana y Callao. Su prioridad es mantener la operación activa sin exponer a sus conductores ni pasajeros, y evitar pérdidas económicas por ataques a su flota. | Según el director de la Cámara Internacional de Logística y Transporte, las empresas de Lima y Callao enfrentan un promedio de **3 atentados armados por semana** contra sus unidades (Infobae, julio 2026). Como respuesta a la crisis, el Estado promulgó la **Ley N.° 32490**, que contempla indemnizaciones para los deudos de conductores asesinados por extorsión (La República, marzo 2026). |
