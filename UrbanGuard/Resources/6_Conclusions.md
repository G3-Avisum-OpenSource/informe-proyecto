# Conclusiones

1. **Se construyó el backend de Avisum con el contrato del frontend.** El API expone los recursos de conductores, unidades, turnos y alertas con los mismos formatos que usó la API simulada del Sprint 2, de modo que la integración del Sprint 4 no exige rediseñar el frontend.

2. **El código quedó organizado por *bounded contexts*.** Los contextos de identidad y turnos, emergencias y flota están separados en capas y se comunican por servicios, siguiendo el diseño del informe.

3. **Las reglas de negocio pasaron del frontend al servidor.** Quedaron implementadas la validación de conductores desactivados, el código de empleado asignado por el servidor, la unicidad del DNI y la placa, el turno único por conductor (US39) y la exigencia de turno activo para registrar una alerta (US03).

4. **El tiempo de respuesta ante alertas ahora queda registrado.** La hora de resolución de cada alerta se guarda en la base de datos, lo que permite calcular el indicador de la *Hypothesis Statement 2* con datos persistentes.

5. **La documentación interactiva facilita la verificación.** Swagger UI permite que cualquier integrante pruebe el API sin escribir código, y MySQL Workbench permite comprobar que cada operación se guardó.

6. **Quedan pendientes identificados para el Sprint 4.** La conexión con el frontend, la autenticación y los roles en el servidor, las notificaciones y las métricas en el backend, las reglas de detección de alertas y el despliegue en la nube.

# Recomendaciones

- Priorizar la seguridad de la información desde el diseño (cifrado de extremo a extremo, autenticación robusta, control granular de accesos), ya que el sistema maneja datos especialmente sensibles: la ubicación en vivo de personas y unidades, además de los detalles de cada alerta de pánico generada.

- No dar por cerrado el diseño una vez implementado: se recomienda monitorear de forma continua indicadores concretos (tiempo real de respuesta ante alertas, porcentaje de conductores y empresas que adoptan el sistema, frecuencia de uso sostenido en el tiempo), contrastándolos contra las Hypothesis Statements planteadas en el Capítulo I para validar o replantear el rumbo del producto.
