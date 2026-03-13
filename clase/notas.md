# 🗒️ Registro de Trabajo en Clase - Taller 4

## 📆 Fecha de la sesión
_7 de marzo de 2026_

## 👥 Integrantes presentes
- Bryam Diaz
- Jose Guzman
- Juan Abril

## 🧠 Actividades realizadas en clase

Describa brevemente qué se hizo durante la sesión:

- ¿Qué se discutió con el equipo?

Durante la sesión de trabajo, analizamos el caso de la plataforma logística RedExpress con el objetivo de identificar los principales componentes de su infraestructura tecnológica y comprender cómo interactúan entre sí para soportar las operaciones del sistema. Se discutió cómo fluye la información desde los usuarios que utilizan la aplicación móvil y la plataforma web hasta los servicios backend y la base de datos centralizada.

- ¿Qué decisiones de modelado se tomaron?

A partir de esta discusión, se tomaron decisiones de modelado orientadas a representar la arquitectura en capas. Se definieron cuatro niveles principales: usuarios o clientes, entrada al sistema, servicios de aplicación y capa de datos e infraestructura. Dentro de estas capas se incluyeron componentes como el load balancer, API Gateway, servicios de rastreo de paquetes, motor de rutas, gestión de envíos, notificaciones, servidores regionales de procesamiento y la base de datos central con réplicas de lectura. También se incorporaron elementos externos como el proveedor de notificaciones y el sistema de monitoreo, con el fin de reflejar una infraestructura más completa y cercana a un entorno real.

- ¿Qué herramientas se usaron (papel, pizarra, draw.io, Astah)?

Para la construcción del mapa de infraestructura se utilizó la herramienta draw.io, la cual permitió organizar visualmente los componentes y sus conexiones. Inicialmente se discutieron las ideas en equipo y luego se procedió a plasmar el modelo directamente en el diagrama digital, estableciendo las relaciones entre los distintos servicios y recursos de infraestructura.

- ¿Qué parte del trabajo se alcanzó a desarrollar?

Durante la sesión se logró desarrollar un mapa preliminar de la infraestructura lógica del sistema, identificando el flujo principal de solicitudes desde los clientes hacia el backend y la base de datos. Asimismo, se comenzaron a detectar posibles áreas críticas del sistema, como la dependencia de la base de datos central, la carga sobre el API Gateway y la necesidad de monitoreo para garantizar disponibilidad y rendimiento. Este avance permitió contar con una primera representación visual de la arquitectura sobre la cual se podrá continuar el análisis técnico en las siguientes etapas del taller.


## 🧩 Boceto inicial del modelo

![Borrador mapa](mapa-borrador.png)

1. ¿Donde esta el cuello de botella?

La base de datos central porque todos los servicios dependen de ella.

2. ¿Dónde hay riesgo de falla?

Puntos críticos:
- API Gateway
- Base de datos principal
- Motor de rutas

3. ¿Dónde puede haber latencia?

Tracking Service → Database ya que el rastreo es tiempo real.

## 🔁 Tareas definidas para complementar el taller

Anote las responsabilidades acordadas entre los miembros del equipo para completar la entrega final:

| Tarea asignada | Responsable | Fecha estimada |
|----------------|-------------|----------------|
| Modelado final en draw.io | Jose Guzman | 10/08 |
| Redacción del informe     | Bryam Diaz | 11/08 |
| Investigación y referencias | Juan Abril | 12/08 |

---

_Este documento resume el trabajo colaborativo realizado durante la sesión del taller 4 en el curso AREM - Universidad de La Sabana._
