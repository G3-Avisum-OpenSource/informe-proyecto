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
|     !     |  | Ingenieria de Software |                     |
| ![CarlosFoto](Resources/img/carlos.png) | Blancas Chávez, Carlos Franco      | Ingenieria de Software | Typscript, React,Vue, Java, MySQL,PostgreSQL,MongoDB, Python, C#                                                               |
| ! |                      | Ingenieria de Software |  |
|  !  |  | Ingenieria de Software |                    
---


## 1.2. Solution Profile

### 1.2.1. Antecedentes y problemática

**Qué:** Los pasajeros del transporte público urbano no tienen forma de verificar si el conductor que opera la unidad es la persona autorizada, y los propios conductores no cuentan con ningún canal digital para pedir auxilio inmediato ante una situación de riesgo. A esto se suma que las empresas de transporte no tienen visibilidad en tiempo real de la ubicación ni el estado de sus unidades una vez que salen a ruta.

**Cuándo:** El problema está presente en cada servicio de transporte, desde que el pasajero aborda hasta que llega a su destino, y se intensifica en horarios nocturnos o en rutas con menor supervisión policial.

**Dónde:** Esta problemática tiene una data de más de una década en el norte del Perú (Trujillo, Chiclayo, Piura) y hoy es igual de visible en Lima Metropolitana y Callao, donde conviven empresas formales con operadores informales bajo el mismo sistema de transporte urbano.

**Quién:** Afecta principalmente a tres actores: los pasajeros, que no tienen manera de saber si viajan con un conductor autorizado; los conductores, quienes en muchos casos son blanco directo de extorsión, asalto o violencia sin tener cómo pedir auxilio de forma rápida; y las empresas operadoras de transporte, que actúan "a ciegas" respecto a lo que ocurre con sus unidades una vez en ruta.

**Por qué:** La causa de fondo es la ausencia de herramientas tecnológicas accesibles: no existe un sistema que centralice identificación del conductor, comunicación de emergencia en tiempo real y visibilidad de ubicación para el transporte urbano promedio en el Perú.

**Cómo afecta:** La combinación de informalidad del sector y débil regulación tecnológica genera un entorno propicio para la violencia organizada contra el transporte, el cobro de cupos, la renuncia forzada de conductores por miedo, y un fuerte impacto psicológico tanto en quienes conducen como en quienes usan el servicio a diario.

**Cuánto:** La magnitud del problema está documentada con evidencia reciente y verificable:
- Casos como el de la empresa Translima muestran que los conductores son obligados a pagar cupos diarios, con amenazas de incremento de hasta 20 a 30 soles por unidad; producto de esta violencia, al menos dos conductores han perdido la vida desde 2025 y cerca de veinte han abandonado sus puestos por miedo.
- Solo entre enero y febrero de 2026, se registraron 898 denuncias de extorsión en Lima Centro, la cifra más alta reportada en el país durante ese periodo, según fuentes policiales.
- Se estima que cerca del 80% de las empresas de transporte formal de Lima realizó pagos a organizaciones criminales durante 2025, y que el monto total exigido al sector transporte supera los S/10 millones mensuales a nivel nacional.
- Como respuesta a esta crisis, el Estado peruano promulgó una nueva ley que exige a las empresas de transporte capacitar a su personal en la detección y denuncia de actos extorsivos — evidencia de que el problema ya es reconocido a nivel regulatorio, aunque aún sin una solución tecnológica integral como la que propone Avisum.

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements

> Como **pasajero de transporte público**, no tengo ninguna forma de confirmar que el conductor de la unidad en la que viajo es la persona autorizada para operarla, lo cual me genera desconfianza e inseguridad en cada viaje.

> Como **conductor de una unidad de transporte**, no cuento con ningún canal directo para pedir ayuda si me encuentro en una situación de peligro durante mi turno, lo que me deja completamente expuesto ante un asalto o emergencia.

> Como **empresa de transporte**, no tengo visibilidad de dónde se encuentran mis unidades ni de qué está pasando con ellas en tiempo real, lo cual me impide reaccionar a tiempo ante cualquier incidente.


### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements

> Como **pasajero de transporte público**, no tengo ninguna forma de confirmar que el conductor de la unidad en la que viajo es la persona autorizada para operarla, lo cual me genera desconfianza e inseguridad en cada viaje.

> Como **conductor de una unidad de transporte**, no cuento con ningún canal directo para pedir ayuda si me encuentro en una situación de peligro durante mi turno, lo que me deja completamente expuesto ante un asalto o emergencia.

> Como **empresa de transporte**, no tengo visibilidad de dónde se encuentran mis unidades ni de qué está pasando con ellas en tiempo real, lo cual me impide reaccionar a tiempo ante cualquier incidente.

#### 1.2.2.2. Lean UX Assumptions

- Un pasajero que puede verificar la identidad del conductor percibirá el servicio como más confiable, incluso sin haber tenido un mal momento previo.
- Un conductor usará un botón de pánico solo si confía en que la respuesta del otro lado será rápida y real, no simbólica.
- Las empresas de transporte adoptarán un sistema de monitoreo si perciben una reducción tangible en su exposición legal y reputacional ante incidentes.
- El seguimiento GPS constante no debe consumir batería ni datos de forma perceptible para el conductor, o dejará de usarse.
- La verificación de identidad debe tomar segundos, no minutos — cualquier fricción en el inicio de turno reduce la adopción.

#### 1.2.2.3. Lean UX Hypothesis Statements

> Creemos que si un conductor puede verificar su identidad con un código digital al iniciar su turno, los pasajeros percibirán mayor seguridad al abordar. Lo sabremos porque las quejas relacionadas a conductores desconocidos disminuirán y la percepción de confianza reportada por los usuarios aumentará.

> Creemos que si un conductor cuenta con un botón de pánico conectado en vivo a una central, el tiempo de respuesta ante una emergencia se reducirá drásticamente. Lo sabremos porque las alertas generadas serán atendidas en cuestión de minutos y los conductores reportarán sentirse respaldados durante su turno.

> Creemos que si las empresas de transporte cuentan con un panel de monitoreo en tiempo real de su flota, podrán reaccionar más rápido ante cualquier incidente reportado. Lo sabremos porque el tiempo entre la generación de una alerta y su resolución se reducirá de forma medible.

#### 1.2.2.4. Lean UX Canvas

*(Pendiente de formato visual — puedo redactar el contenido de cada bloque —problema de negocio, resultados esperados, usuarios, beneficios, soluciones propuestas, hipótesis, y qué validar primero— si me confirmas que armamos primero el texto antes de pasarlo a un diagrama)*

## 1.3. Segmentos objetivo

- **Pasajeros de transporte público urbano**, con especial atención a mujeres, adultos mayores y estudiantes escolares, quienes buscan mayor tranquilidad y certeza al momento de abordar una unidad.
- **Conductores de unidades de transporte**, que enfrentan a diario el riesgo de asalto o extorsión y necesitan un canal de auxilio inmediato durante su jornada.
- **Empresas operadoras de transporte público**, interesadas en tener trazabilidad de su flota y capacidad de respuesta ante cualquier incidente que involucre a sus unidades o conductores.
