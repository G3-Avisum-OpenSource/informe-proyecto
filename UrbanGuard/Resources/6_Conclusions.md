# Conclusiones

- Detrás de Avisum hay un problema que ya no se puede ignorar: la violencia y la extorsión contra el transporte público han escalado al punto de convertirse en una crisis documentada con cifras oficiales (Capítulo I). Frente a ese escenario, este proyecto confirma que una capa tecnológica de verificación y respuesta inmediata puede marcar una diferencia real en la seguridad de quienes dependen de este servicio a diario.

- Que un conductor pueda confirmar su identidad en segundos, activar una alerta ante cualquier señal de peligro, y que su unidad quede visible en todo momento para la central de operaciones, no es solo una mejora técnica — es lo que convierte la incertidumbre de "¿alguien se va a enterar si me pasa algo?" en la certeza de que sí. Esa diferencia es, precisamente, lo que hace que el sistema valga la pena adoptarlo.

- El alcance de Avisum va más allá de proteger a un conductor puntual: al conectar a conductores, empresas y, eventualmente, a las propias autoridades bajo un mismo flujo de información, el proyecto sienta las bases para que la seguridad en el transporte deje de depender de la suerte o de la reacción individual, y se convierta en un esfuerzo coordinado entre todos los actores involucrados.

# Sprint 3

1. **Se construyó el backend de Avisum con el contrato del frontend.** El API expone los recursos de conductores, unidades, turnos y alertas con los mismos formatos que usó la API simulada del Sprint 2, de modo que la integración del Sprint 4 no exige rediseñar el frontend.

2. **El código quedó organizado por *bounded contexts*.** Los contextos de identidad y turnos, emergencias y flota están separados en capas y se comunican por servicios, siguiendo el diseño del informe.

3. **Las reglas de negocio pasaron del frontend al servidor.** Quedaron implementadas la validación de conductores desactivados, el código de empleado asignado por el servidor, la unicidad del DNI y la placa, el turno único por conductor (US39) y la exigencia de turno activo para registrar una alerta (US03).

4. **El tiempo de respuesta ante alertas ahora queda registrado.** La hora de resolución de cada alerta se guarda en la base de datos, lo que permite calcular el indicador de la *Hypothesis Statement 2* con datos persistentes.

5. **La documentación interactiva facilita la verificación.** Swagger UI permite que cualquier integrante pruebe el API sin escribir código, y MySQL Workbench permite comprobar que cada operación se guardó.

6. **Quedan pendientes identificados para el Sprint 4.** La conexión con el frontend, la autenticación y los roles en el servidor, las notificaciones y las métricas en el backend, las reglas de detección de alertas y el despliegue en la nube.

# Recomendaciones

- Priorizar la seguridad de la información desde el diseño (cifrado de extremo a extremo, autenticación robusta, control granular de accesos), ya que el sistema maneja datos especialmente sensibles: la ubicación en vivo de personas y unidades, además de los detalles de cada alerta de pánico generada.

- No dar por cerrado el diseño una vez implementado: se recomienda monitorear de forma continua indicadores concretos (tiempo real de respuesta ante alertas, porcentaje de conductores y empresas que adoptan el sistema, frecuencia de uso sostenido en el tiempo), contrastándolos contra las Hypothesis Statements planteadas en el Capítulo I para validar o replantear el rumbo del producto.
