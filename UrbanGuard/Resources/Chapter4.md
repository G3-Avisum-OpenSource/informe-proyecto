
# Capítulo IV: Product Design

## 4.1. Style Guidelines

Una guía de estilos enumera las elecciones visuales y de interacción adoptadas por el equipo, manteniendo consistencia entre diseño y desarrollo a lo largo de todo el producto.

### 4.1.1. General Style Guidelines

El estilo visual de Avisum busca transmitir vigilancia, control y respuesta inmediata — no es una app de consumo masivo, sino una herramienta de seguridad operativa, por lo que cada decisión de diseño prioriza la lectura rápida de información crítica por sobre la estética decorativa.

**Branding**

Elegimos estos colores porque buscamos transmitir vigilancia constante, urgencia cuando es necesario, y control tecnológico. El negro simboliza precisión y seriedad, siendo el color base de toda la interfaz. El verde neón aporta la sensación de "sistema activo" — como el testigo verde de un panel de monitoreo real — y se reserva para indicadores de estado normal y acciones principales. El rojo se usa exclusivamente para alertas y pánico, reforzando su asociación inmediata con peligro.

Buscamos que el usuario perciba el sistema como:
- Seguro
- Preciso
- Siempre activo
- Con respuesta inmediata ante emergencias

(( **Color Palette** ))

(( **Imagen a insertar:** Captura o diseño en Figma con 3 muestras de color en formato círculo/swatch, igual al ejemplo de referencia — cada una con su nombre y código hexadecimal debajo. Guardar como `Resources/img/paleta-colores-avisum.png`. ))

- **Negro (#000000):** Base de toda la interfaz. Aporta seriedad y genera un entorno visual libre de distracciones, reforzando la percepción de vigilancia constante.
- **Verde neón (#C3F400):** Color principal de acento, usado en botones, indicadores de estado activo y títulos. Se asocia a monitoreo digital y confirmación de que "todo está en orden". Como color secundario de contraste se usa un verde oscuro (#596D0B).
- **Rojo:** Reservado únicamente para elementos críticos — botón de pánico, alertas activas y estados de emergencia — para que el usuario lo asocie de inmediato con "atención urgente" y no lo confunda con ninguna otra acción del sistema.

 (( **Typography** ))

Usamos **Space Grotesk** para títulos y **Inter** para texto de lectura, porque ambas tipografías tienen alta legibilidad en pantallas oscuras y una estética técnica que refuerza la identidad de "sistema de monitoreo" que buscamos para Avisum.

| Elemento | Tipografía | Tamaño |
|---|---|---|
| Títulos | Space Grotesk Bold | 96px |
| Subtítulos | Space Grotesk Bold | 48-60px |
| Párrafos | Inter Light/Bold | 12-24px |

(( **Imagen a insertar:** Captura de la jerarquía tipográfica en Figma, mostrando una muestra de cada tamaño con su etiqueta. Guardar como `Resources/img/tipografia-avisum.png`. ))

**Spacing y Layout**

El diseño se organiza mediante espacios consistentes en múltiplos de 2px, y estructuras tipo tarjeta para agrupar información relacionada (por ejemplo, los datos de una unidad o de una alerta).

- **Grid:** Márgenes de 24px para mantener armonía visual entre secciones.
- **Breakpoints:** Ancho de referencia de 1440px para escritorio.

 **Imagen a insertar:** Diagrama simple en Figma mostrando el sistema de espaciado (ej. una tarjeta con las medidas de padding marcadas). Guardar como `Resources/img/spacing-avisum.png`.

**Componentes visuales**

- **Botones:** Verde neón para acciones principales, rojo para acciones críticas (pánico, resolver alerta), gris para acciones secundarias.
- **Cards:** Contenedores oscuros con borde sutil, usados para mostrar unidades, alertas y conductores de forma organizada.
- **Iconografía:** Estilo lineal simple, de fácil reconocimiento incluso a tamaños pequeños.

 **Imagen a insertar:** Captura de Figma mostrando los 3 estilos de botones lado a lado (principal, crítico, secundario). Guardar como `Resources/img/botones-avisum.png`.

**Responsive Design Standards (Mobile-first)**

- **Mobile (hasta 768px):** Diseño de una sola columna, menú tipo hamburguesa, botones grandes para uso táctil (relevante porque el conductor interactúa con la app mientras maneja).
- **Tablet (769px-1024px):** Layout de hasta dos columnas.
- **Desktop (1025px+):** Layout de dos o tres columnas, navegación principal siempre visible (pensado para el panel de administración, usado típicamente en escritorio).

**Accessibility**

- Contraste de color según pautas WCAG 2.1 AA en todos los estados.
- Navegación completa mediante teclado.
- Elementos interactivos con dimensión mínima de 48×48px, crítico para el botón de pánico bajo condiciones de estrés.

**Tono de comunicación**

El tono de Avisum es serio, directo y profesional — evitamos lenguaje informal porque el contexto de uso es de seguridad real, donde la claridad del mensaje puede afectar el tiempo de reacción ante una emergencia.

### 4.1.2. Web Style Guidelines

 **Imagen a insertar:** Captura de Figma mostrando el navbar y los estados de los botones (normal, hover, activo) del entorno web. Guardar como `Resources/img/navbar-botones-avisum.png`.

---

## 4.2. Information Architecture

En esta sección se plantean las decisiones y el sustento que dirigen cómo se organiza el contenido en la experiencia web de Avisum. Las propuestas están orientadas a que conductores, empresas y visitantes se adapten con facilidad a la funcionalidad del producto, reduciendo la carga cognitiva y facilitando que cada usuario llegue a la información que necesita sin esfuerzo.

### 4.2.1. Organization Systems

Para la Landing Page se combina una organización **jerárquica** (el usuario accede a secciones clave desde la barra de navegación) con una organización **secuencial** (el contenido se ordena como una narrativa de conversión: propuesta de valor, problema, solución, beneficios, comparación y llamado a la acción).

Para la aplicación web se usa además un **esquema según audiencia**, dividiendo la experiencia en tres flujos distintos según el rol del usuario:

- **Conductor:** El recorrido inicia al verificar su identidad. Su acción principal es iniciar turno y, si ocurre una emergencia, activar el botón de pánico. El flujo termina al finalizar el servicio.

 **Imagen a insertar:** Diagrama de flujo simple en Figma/draw.io con la secuencia: `Verificar identidad → Iniciar turno → Ver mapa/ruta → (Activar pánico si aplica) → Finalizar servicio`. Guardar como `Resources/img/flujo-conductor-avisum.png`.

- **Central de operaciones / Empresa:** El recorrido inicia de forma reactiva, al recibir una alerta. La empresa consulta el panel de control, revisa la unidad y el conductor involucrado, y marca la alerta como resuelta una vez atendida.

 **Imagen a insertar:** Diagrama de flujo con la secuencia: `Recibe alerta → Ingresa al panel → Revisa detalle (conductor, unidad, ubicación) → Atiende → Marca como resuelta`. Guardar como `Resources/img/flujo-empresa-avisum.png`.

| Nivel | Sección | Propósito dentro de la arquitectura |
|---|---|---|
| Global | Header (Navbar) | Acceso rápido a las secciones principales y al inicio de sesión. |
| Principal | Hero section | Presenta la propuesta de valor de Avisum con llamada a la acción. |
| Contextual | Problem section | Explica la problemática de inseguridad en el transporte público. |
| Funcional | Main features section | Agrupa las funcionalidades: verificación de identidad, botón de pánico, monitoreo en tiempo real. |
| Explicativo | How it works section | Explica el flujo de funcionamiento de Avisum en etapas. |
| Persuasivo | Benefits section | Resume los beneficios para conductores y empresas. |
| Confianza | Trust section | Explica cómo Avisum reduce el riesgo y genera confianza. |
| Comercial | Pricing section | Presenta los planes disponibles. |
| Soporte | FAQ section | Resuelve dudas frecuentes. |
| Cierre | Footer section | Repite accesos clave y enlaces de contacto. |

### 4.2.2. Labeling Systems

Colocamos las etiquetas de navegación en la parte superior de forma clara y directa, ajustando su lenguaje al contexto de seguridad del producto (evitando términos ambiguos o demasiado comerciales).

| Etiqueta | Tipo | Uso dentro de la landing |
|---|---|---|
| Cómo funciona | Navegación principal | Explica el flujo operativo de Avisum. |
| Beneficios | Navegación principal | Dirige a la sección de beneficios. |
| Planes | Navegación principal | Muestra las opciones de suscripción. |
| Iniciar sesión | Acción de acceso | Acceso de conductores y empresas ya registradas. |
| Comenzar ahora | CTA principal | Dirige al flujo de registro. |
| Da el siguiente paso | CTA final | Refuerza el llamado a registrarse. |

### 4.2.3. SEO Tags and Meta Tags

Definimos la siguiente estructura de etiquetas `<title>` y `<meta>`, enfocada en captar tráfico orgánico de empresas de transporte que busquen soluciones de seguridad:

```html
<title>Avisum | Seguridad en Tiempo Real para el Transporte Público</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<meta name="description" content="Avisum verifica la identidad de los conductores, activa alertas de pánico en tiempo real y da a las empresas de transporte visibilidad total de su flota.">
<meta name="keywords" content="seguridad transporte público, botón de pánico, monitoreo GPS flota, verificación conductor, Perú">
<meta name="author" content="Avisum Team">
<link rel="icon" type="image/png" href="/assets/avisum-icon.png" />
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<meta property="og:title" content="Avisum | Seguridad en Tiempo Real para el Transporte Público">
<meta property="og:description" content="Verificación de identidad, alertas de pánico y monitoreo GPS para conductores y empresas de transporte.">
<meta property="og:type" content="website">
```

### 4.2.4. Searching Systems

Para que las empresas no se sientan perdidas al gestionar decenas de conductores y unidades, la plataforma ofrece dos mecanismos de búsqueda:

| Sistema de búsqueda | Descripción | Beneficio para el usuario |
|---|---|---|
| **Búsqueda por nombre parcial** | Permite ubicar a un conductor escribiendo solo parte de su nombre, filtrando la lista en tiempo real. | Útil cuando la empresa no recuerda el nombre completo del conductor. |
| **Búsqueda por filtro de categoría/estado** | Permite filtrar unidades o conductores por su estado actual (activo, en alerta, inactivo). | Permite a la central priorizar de inmediato qué unidades requieren atención. |

### 4.2.5. Navigation Systems

- **Menús de navegación:** En web se ubican en el header (para el sitio informativo) y en un sidebar lateral fijo (para la aplicación operativa de conductor y administración).
- **Etiquetas de estado:** Cada conductor y unidad se identifica visualmente con una etiqueta de color según su estado (activo, en alerta, inactivo), permitiendo reconocimiento inmediato sin necesidad de leer texto.
- **Barra de búsqueda:** Disponible en el panel administrativo, integrada con los sistemas de búsqueda descritos en el punto anterior.

---

## 4.3. Landing Page UI Design

### 4.3.1. Landing Page Wireframe

 **Imágenes a insertar:** 2-3 capturas de Figma mostrando el wireframe (en escala de grises, sin color final) de la Landing Page completa, dividida en bloques por sección (Hero, Problema, Funcionalidades, etc.). Guardar como `Resources/img/wireframe-landing-1.png`, `wireframe-landing-2.png`, `wireframe-landing-3.png`.

### 4.3.2. Landing Page Mock-up

 **Imagen a insertar:** Captura del mock-up final con color, de la Landing Page completa (o un scroll largo). Guardar como `Resources/img/mockup-landing-avisum.png`.

---

## 4.4. Web Applications UX/UI Design

### 4.4.1. Web Applications Wireframes

Los wireframes definen la estructura funcional de las pantallas principales del sistema antes de aplicar estilo visual, permitiendo validar la distribución de información según las tareas identificadas en el User Task Matrix del Capítulo 2.

 **Imagen a insertar:** Wireframe de las pantallas principales del conductor (login/verificación, dashboard, mapa, pánico). Guardar como `Resources/img/wireframe-conductor-avisum.png`.

 **Imagen a insertar:** Wireframe de las pantallas principales de administración (panel de control, gestión de conductores, alertas). Guardar como `Resources/img/wireframe-admin-avisum.png`.

### 4.4.2. Web Applications Wireflow Diagrams

 **Imagen a insertar:** Diagrama de wireflow conectando las pantallas anteriores con flechas de navegación, mostrando cómo el usuario se mueve entre ellas. Guardar como `Resources/img/wireflow-avisum.png`.

### 4.4.3. Web Applications Mock-ups

 **Imágenes a insertar:** Mock-ups finales con color de: (1) pantalla de verificación/acceso del conductor, (2) pantalla de inicio/dashboard del conductor, (3) mapa en tiempo real, (4) panel de control del administrador. Guardar como `Resources/img/mockup-acceso-conductor.png`, `mockup-dashboard-conductor.png`, `mockup-mapa-avisum.png`, `mockup-panel-admin.png`.

### 4.4.4. Web Applications User Flow Diagrams

 **Imagen a insertar (Admin):** Diagrama de flujo del recorrido del administrador desde que recibe una alerta hasta que la resuelve. Guardar como `Resources/img/userflow-admin-avisum.png`.

 **Imagen a insertar (Conductor):** Diagrama de flujo del recorrido del conductor desde que verifica su identidad hasta que finaliza su turno. Guardar como `Resources/img/userflow-conductor-avisum.png`.

---

## 4.5. Web Applications Prototyping

### Introducción y criterios de diseño

El prototipo interactivo de Avisum simula la navegación y los flujos principales de la aplicación, permitiendo evaluar la coherencia de la experiencia antes del desarrollo. Fue construido en Figma con conexiones de prototipado entre frames, replicando fielmente los comportamientos definidos en los User Flow Diagrams.

**Orientación al rol y al flujo operativo de urgencia:** Para el conductor, el botón de pánico es el elemento más prominente de su pantalla, visible desde que inicia sesión. Para la central de operaciones, el panel de alertas activas por nivel de gravedad es la primera vista al ingresar.

**Consistencia en los patrones de interacción:** Se usan 4 patrones a lo largo de toda la app: (1) Sidebar para cambiar de módulo según el rol activo, (2) Drawer lateral para formularios que no requieren cambio de contexto, (3) Modal para acciones críticas que requieren confirmación (finalizar turno, resolver alerta), y (4) Toast/Snackbar para retroalimentación inmediata sin interrumpir el flujo.

**Prevención de errores en acciones de alto impacto:** Acciones como activar el botón de pánico o finalizar un turno incluyen una capa de confirmación mediante modal, dado que una acción incorrecta puede afectar la trazabilidad de un incidente real.

**Retroalimentación inmediata:** El panel de alertas se actualiza al instante al recibir una nueva alerta, y la posición de cada unidad en el mapa se actualiza en tiempo real sin necesidad de recargar la página.

**Accesibilidad y objetivos táctiles:** Todos los elementos interactivos tienen mínimo 48×48px, relevante porque el conductor interactúa con la app mientras maneja. El botón de pánico usa dimensiones ampliadas y alto contraste para garantizar su activación bajo estrés.

 **Imagen a insertar:** Captura general del prototipo de Figma mostrando varios frames conectados con las líneas de prototipado visibles. Guardar como `Resources/img/prototipo-general-avisum.png`.

### Flujos de interacción cubiertos por el prototipo

**Flujo 1 — Verificación e inicio de servicio del conductor**

 **Imagen a insertar:** Captura del flujo interactivo desde la verificación de identidad hasta la pantalla de servicio activo. Guardar como `Resources/img/flujo-verificacion-avisum.png`.

**Flujo 2 — Activación y gestión de alertas de emergencia**

 **Imagen a insertar:** Captura del flujo desde la activación del botón de pánico hasta la recepción y resolución de la alerta en el panel de la central. Guardar como `Resources/img/flujo-alerta-avisum.png`.

**Flujo 3 — Monitoreo de flota por la empresa administradora**

 **Imagen a insertar:** Captura del flujo del dashboard con el estado en tiempo real de todas las unidades activas. Guardar como `Resources/img/flujo-monitoreo-avisum.png`.

---

## 4.6. Domain-Driven Software Architecture

### 4.6.1. Design-Level Event Storming

Avisum es una plataforma orientada a mejorar la seguridad del transporte público mediante monitoreo en tiempo real, verificación de identidad y respuesta inmediata ante emergencias entre conductores, empresas y central de operaciones.

 **Imágenes a insertar:** Capturas del tablero de Event Storming a nivel de diseño (Miro/FigJam), una por cada bounded context: **Autenticación de conductores**, **Monitoreo de flota**, **Gestión de alertas**. Guardar como `Resources/img/eventstorming-auth-avisum.png`, `eventstorming-monitoreo-avisum.png`, `eventstorming-alertas-avisum.png`.

### 4.6.2. Software Architecture Context Diagram

 **Imagen a insertar:** Diagrama de contexto (nivel C4 - System Context) mostrando Avisum como sistema central, y sus actores externos (Conductor, Empresa, Central de Operaciones). Guardar como `Resources/img/context-diagram-avisum.png`.

### 4.6.3. Software Architecture Container Diagrams

 **Imagen a insertar:** Diagrama de contenedores (nivel C4 - Container) mostrando el frontend web, el backend API REST y la base de datos. Guardar como `Resources/img/container-diagram-avisum.png`.

### 4.6.4. Software Architecture Components Diagrams

 **Imagen a insertar:** Diagrama de componentes mostrando los bounded contexts del backend (Autenticación, Monitoreo, Alertas) y sus relaciones internas. Guardar como `Resources/img/components-diagram-avisum.png`.

---

## 4.7. Software Object-Oriented Design

Esta sección presenta el diseño orientado a objetos de la RESTful API de Avisum (Spring Boot + Spring Data JPA + Java), correspondiente a los tres Epics del Product Backlog con lógica de dominio propia: **EPAV01 – Verificación de identidad**, **EPAV02 – Gestión de emergencias** y **EPAV03 – Monitoreo de flota** (ver 3.1. User Stories). El Epic EPAV05 (API RESTful) no introduce clases de dominio adicionales, ya que corresponde a la capa de exposición (controllers/DTOs) sobre estos mismos modelos; el Epic EPAV04 (Plataforma web informativa) corresponde al sitio estático del Landing Page y no requiere diseño orientado a objetos de dominio.

El diseño se organiza en tres Bounded Contexts, cada uno con su propio Class Diagram: **Gestión de Identidad y Turnos**, **Gestión de Emergencias** y **Monitoreo de Flota**. Estos contextos son consistentes con los Aggregates propuestos en el Big Picture EventStorming (Turno, Alerta de Pánico, Unidad de Transporte — ver 2.4) y con los términos definidos en el Ubiquitous Language (ver 2.5).

Para todos los diagramas se aplica la siguiente notación UML estándar de visibilidad de miembros: `-` atributo/método **private**, `+` **public**, `#` **protected**. Las relaciones se anotan con nombre de rol (calificación), dirección de navegación cuando aplica, y multiplicidad en ambos extremos, según lo requerido. Las clases marcadas con el estereotipo `<<reference>>` representan una referencia liviana (por identificador) a un Aggregate Root que pertenece a otro Bounded Context, evitando duplicar su modelo completo — práctica estándar en Domain-Driven Design para mantener la autonomía de cada contexto.


### 4.7.1. Class Diagrams

**Bounded Context 1 — Gestión de Identidad y Turnos (Identity & Shift Management)**

```mermaid
classDiagram
    class Company {
        -id: UUID
        -businessName: String
        -ruc: String
        -contactEmail: String
        +registerDriver(driver: Driver) void
    }

    class Driver {
        -id: UUID
        -firstName: String
        -lastName: String
        -licenseNumber: String
        -phone: String
        -status: DriverStatus
        +authorize() boolean
        +deactivate() void
        +getFullName() String
    }

    class Shift {
        -id: UUID
        -startTime: LocalDateTime
        -endTime: LocalDateTime
        -status: ShiftStatus
        +start() void
        +close() void
        +verifyIdentity(code: String) boolean
        +isActive() boolean
    }

    class VerificationCode {
        -code: String
        -issuedAt: LocalDateTime
        -expiresAt: LocalDateTime
        +isValid() boolean
        +isExpired() boolean
    }

    class TransportUnit {
        <<reference>>
        -id: UUID
    }

    class DriverStatus {
        <<enumeration>>
        ACTIVE
        INACTIVE
        SUSPENDED
    }

    class ShiftStatus {
        <<enumeration>>
        PENDING_VERIFICATION
        ACTIVE
        CLOSED
        REJECTED
    }

    Company "1" --> "0..*" Driver : employs
    Driver "1" --> "0..*" Shift : performs
    Shift "1" *-- "1" VerificationCode : validatesWith
    Shift "0..*" --> "0..1" TransportUnit : assignedTo
    Driver ..> DriverStatus
    Shift ..> ShiftStatus
```

Este contexto cubre EPAV01 y las historias US01, US02, US14, US15, US25, US26, US39. `Driver` representa al conductor y expone `authorize()` para soportar la validación de autorización (US14); `Shift` es el Aggregate Root del turno de trabajo, con `verifyIdentity()` implementando la verificación por código (US01) y `isActive()` dando soporte a la regla de negocio de US39 (un conductor no puede tener más de un turno activo simultáneamente — esta invariante se valida antes de ejecutar `Shift.start()`). `VerificationCode` es un Value Object compuesto dentro de `Shift` (composición `"1" *-- "1"`, ya que no tiene identidad ni ciclo de vida propio fuera del turno). `Company` emplea (`"1" --> "0..*"`) a sus `Driver`, y `Shift` se asocia opcionalmente (`"0..1"`) a una `TransportUnit`, referenciada aquí solo por su identificador porque su modelo completo pertenece al Bounded Context de Monitoreo de Flota.


**Bounded Context 2 — Gestión de Emergencias (Emergency & Alert Management)**

```mermaid
classDiagram
    class PanicAlert {
        -id: UUID
        -triggeredAt: LocalDateTime
        -severity: AlertLevel
        -status: AlertStatus
        -respondedAt: LocalDateTime
        -confirmedAt: LocalDateTime
        +trigger() void
        +classify() AlertLevel
        +escalate() void
        +confirmReception() void
        +assignResponse(response: Response) void
        +close() void
        +getResponseTime() Duration
    }

    class GeoLocation {
        -latitude: double
        -longitude: double
        -recordedAt: LocalDateTime
    }

    class Response {
        -id: UUID
        -assignedTo: String
        -assignedAt: LocalDateTime
        -contactedDriver: boolean
        -authoritiesNotified: boolean
        +assign() void
        +notifyAuthorities() void
    }

    class NotificationRecipient {
        -id: UUID
        -name: String
        -contactInfo: String
        -preferredChannel: NotificationChannel
        +notify(alert: PanicAlert) void
    }

    class NotificationChannel {
        <<interface>>
        +send(alert: PanicAlert, recipient: NotificationRecipient) void
    }

    class AbstractNotifier {
        <<abstract>>
        #buildMessage(alert: PanicAlert) String
        +send(alert: PanicAlert, recipient: NotificationRecipient) void
    }

    class SmsNotifier {
        -gatewayNumber: String
    }

    class EmailNotifier {
        -smtpAccount: String
    }

    class Shift {
        <<reference>>
        -id: UUID
    }

    class AlertLevel {
        <<enumeration>>
        LOW
        MEDIUM
        HIGH
        CRITICAL
    }

    class AlertStatus {
        <<enumeration>>
        SENT
        RECEIVED
        CONFIRMED
        ESCALATED
        RESOLVED
        CLOSED
    }

    NotificationChannel <|.. AbstractNotifier
    AbstractNotifier <|-- SmsNotifier
    AbstractNotifier <|-- EmailNotifier
    PanicAlert "1" *-- "1" GeoLocation : occurredAt
    PanicAlert "1" --> "0..1" Response : handledBy
    PanicAlert "1" --> "1..*" NotificationRecipient : notifies
    PanicAlert "0..*" --> "1" Shift : reportedDuring
    NotificationRecipient "1" --> "1" NotificationChannel : prefers
    PanicAlert ..> AlertLevel
    PanicAlert ..> AlertStatus
```

Este contexto cubre EPAV02 y las historias US03, US04, US05, US16, US23, US24, US33, US34, US40, US41, US42. `PanicAlert` es el Aggregate Root: `classify()` asigna el `AlertLevel` (US40), `escalate()` soporta el reenvío ante alertas sin atender (US41, US24), `confirmReception()` cubre US23, y `getResponseTime()` da soporte al cálculo de tiempos de atención (US34). `GeoLocation` se compone dentro de `PanicAlert` para registrar dónde ocurrió el evento (US42). Para atender el requisito de notificar a más de un destinatario (US33), se introdujo la interfaz `NotificationChannel` con la clase abstracta `AbstractNotifier` (método protegido `#buildMessage()`, reutilizado por las subclases `SmsNotifier` y `EmailNotifier`) — esta estructura permite añadir nuevos canales de notificación sin modificar `PanicAlert` ni `NotificationRecipient`. `PanicAlert` se asocia con `"0..*" --> "1"` hacia `Shift`, referenciado del Bounded Context de Identidad, ya que toda alerta ocurre durante un turno activo.


**Bounded Context 3 — Monitoreo de Flota (Fleet & Real-Time Monitoring)**

```mermaid
classDiagram
    class Fleet {
        -id: UUID
        -name: String
        +addUnit(unit: TransportUnit) void
        +getActiveUnits() List~TransportUnit~
        +compareUnits() FleetReport
    }

    class TransportUnit {
        -id: UUID
        -plateNumber: String
        -status: UnitStatus
        -lastLocation: GeoLocation
        -lastSignalAt: LocalDateTime
        +updateLocation(location: GeoLocation) void
        +updateStatus(status: UnitStatus) void
        +isInactive(threshold: Duration) boolean
        +detectRouteDeviation() boolean
    }

    class Route {
        -id: UUID
        -name: String
        -startPoint: GeoLocation
        -endPoint: GeoLocation
        -waypoints: List~GeoLocation~
        +isWithinPath(location: GeoLocation) boolean
    }

    class GeoLocation {
        -latitude: double
        -longitude: double
        -recordedAt: LocalDateTime
    }

    class Company {
        <<reference>>
        -id: UUID
    }

    class UnitStatus {
        <<enumeration>>
        OPERATIONAL
        STOPPED
        ALERT
        INACTIVE
    }

    Fleet "1" --> "1..*" TransportUnit : contains
    TransportUnit "0..*" --> "1" Route : follows
    TransportUnit "1" *-- "1" GeoLocation : lastKnownAt
    Company "1" --> "1" Fleet : owns
    TransportUnit ..> UnitStatus
```

Este contexto cubre EPAV03 y las historias US06, US07, US17, US27, US28, US35, US36, US43, US44. `Fleet` es el Aggregate Root que agrupa (`"1" --> "1..*"`) a las `TransportUnit` de una empresa; `compareUnits()` da soporte a US44. `TransportUnit.isInactive()` implementa la detección de unidades sin señal (US17), y `detectRouteDeviation()` compara la última ubicación contra la `Route` asignada para soportar US36; `Route.isWithinPath()` encapsula esa regla geográfica. `TransportUnit` compone (`"1" *-- "1"`) su última `GeoLocation` conocida, reutilizada como Value Object desde el contexto de Gestión de Emergencias. `Company` se referencia aquí de forma liviana como dueña (`"1" --> "1"`) de la `Fleet`.

---

## 4.8. Database Design

Esta sección traduce los Class Diagrams de 4.7 a un modelo relacional (PostgreSQL/MySQL vía Spring Data JPA), manteniendo la misma organización por Bounded Context. Los tres contextos residen en un único esquema físico —Avisum expone una sola RESTful API, no un despliegue de microservicios independiente por contexto—, por lo que las referencias cruzadas entre contextos (mostradas como entidades `<<reference>>` en 4.7) se implementan aquí como **foreign keys reales**, no solo como identificadores lógicos.

Se aplican las siguientes decisiones de mapeo objeto-relacional:

- **Claves primarias:** todas las tablas usan `id` de tipo `UUID`, consistente con los atributos `id: UUID` de cada Aggregate en 4.7.
- **Value Objects embebidos:** `VerificationCode` (dentro de `Shift`) y `GeoLocation` (dentro de `PanicAlert` y `TransportUnit`) no reciben tabla propia — al no tener identidad ni ciclo de vida independiente, se mapean como columnas embebidas en la tabla de su Aggregate dueño (`@Embeddable` de JPA), evitando joins innecesarios.
- **Colecciones de Value Objects:** `Route.waypoints` sí requiere tabla propia (`route_waypoint`), porque es una colección de tamaño variable y no puede aplanarse en columnas fijas.
- **Enumeraciones:** `DriverStatus`, `ShiftStatus`, `AlertLevel`, `AlertStatus` y `UnitStatus` se mapean como columnas `VARCHAR` con `CHECK constraint` sobre los valores permitidos, en lugar de tablas de catálogo separadas, dado que son conjuntos cerrados y estables de valores.
- **Interfaz y jerarquía de notificadores:** `NotificationChannel` / `AbstractNotifier` / `SmsNotifier` / `EmailNotifier` (ver 4.7.1, BC2) colapsan en una sola tabla `notification_recipient` con una columna discriminadora `channel_type` (`SINGLE_TABLE` de JPA), en vez de una tabla por subclase, ya que las subclases no agregan columnas propias significativas.


### 4.8.1. Database Diagrams

**Bounded Context 1 — Gestión de Identidad y Turnos**

```mermaid
erDiagram
    COMPANY {
        uuid id PK
        string business_name
        string ruc UK
        string contact_email
    }
    DRIVER {
        uuid id PK
        uuid company_id FK
        string first_name
        string last_name
        string license_number UK
        string phone
        string status
    }
    SHIFT {
        uuid id PK
        uuid driver_id FK
        uuid transport_unit_id FK
        string verification_code
        timestamp code_issued_at
        timestamp code_expires_at
        timestamp start_time
        timestamp end_time
        string status
    }
    TRANSPORT_UNIT {
        uuid id PK
    }

    COMPANY ||--o{ DRIVER : employs
    DRIVER ||--o{ SHIFT : performs
    TRANSPORT_UNIT o|--o{ SHIFT : assignedTo
```

`shift.driver_id` es `NOT NULL` (todo turno pertenece a exactamente un conductor), mientras que `shift.transport_unit_id` es `NULLABLE` — reflejando la multiplicidad `"0..1"` del Class Diagram, ya que un turno puede estar pendiente de verificación antes de asignársele una unidad. `driver.license_number` y `company.ruc` llevan restricción `UNIQUE` al ser identificadores naturales del negocio. `transport_unit` aparece aquí solo con su `id`, como referencia liviana a la tabla completa definida en el Bounded Context de Monitoreo de Flota (4.8.1, BC3) — la foreign key existe a nivel de base de datos, pero el modelo completo de esa entidad no se duplica en este contexto.

**Bounded Context 2 — Gestión de Emergencias**

```mermaid
erDiagram
    PANIC_ALERT {
        uuid id PK
        uuid shift_id FK
        timestamp triggered_at
        string severity
        string status
        decimal latitude
        decimal longitude
        timestamp location_recorded_at
        timestamp responded_at
        timestamp confirmed_at
    }
    ALERT_RESPONSE {
        uuid id PK
        uuid panic_alert_id FK, UK
        string assigned_to
        timestamp assigned_at
        boolean contacted_driver
        boolean authorities_notified
    }
    NOTIFICATION_RECIPIENT {
        uuid id PK
        uuid panic_alert_id FK
        string name
        string contact_info
        string channel_type
    }
    SHIFT {
        uuid id PK
    }

    SHIFT ||--o{ PANIC_ALERT : reportedDuring
    PANIC_ALERT ||--o| ALERT_RESPONSE : handledBy
    PANIC_ALERT ||--|{ NOTIFICATION_RECIPIENT : notifies
```

`panic_alert.latitude/longitude/location_recorded_at` son las columnas embebidas del Value Object `GeoLocation` (US42). `alert_response.panic_alert_id` lleva `UNIQUE` además de `FK`, forzando a nivel de base de datos la multiplicidad `"0..1"` (una alerta tiene, cuando mucho, una respuesta asociada). `panic_alert` se relaciona con `notification_recipient` como `"one-or-many"` (`||--|{`), no `"zero-or-many"`, porque toda alerta activada debe notificar al menos a un destinatario (US33). `shift` aparece aquí solo como referencia liviana desde el Bounded Context de Identidad, ya que `panic_alert.shift_id` es `NOT NULL` (US03: no puede activarse una alerta sin un turno activo).


