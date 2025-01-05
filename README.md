# Proyecto-Final-SO
Evaluación Final.

Alumnos: 
Hernández Mendoza Alan Emanuel
Ontañon Ortiz Jhonatan Jazael
Sierra Estrada Daniela


Especificación del Mensaje y Flujo de Comunicación en el Sistema de Mensajería

El sistema implementará un esquema de comunicación entre un productor y un consumidor utilizando un Broker Buffer MQTT (Mosquitto), empleando tópicos y sub-tópicos para la transmisión de datos. A continuación, se describe el mensaje que será enviado por el productor:

Estructura del Mensaje
Matrícula: INT
Nombre: CHAR
Apellido Paterno: CHAR
Apellido Materno: CHAR
Materia: CHAR
Calificación: CHAR
Carrera: CHAR
Flujo de Comunicación
Emisión del Mensaje:
El productor generará y enviará el mensaje descrito anteriormente mediante un tópico/subtópico configurado en el broker MQTT.

Transmisión del Mensaje:
El mensaje será encolado en el sistema de mensajería basado en MQTT (Mosquitto), asegurando que llegue de manera asíncrona al consumidor suscrito al tópico correspondiente.

Procesamiento del Mensaje por el Consumidor:
El consumidor utilizará una librería de consulta para procesar los datos recibidos.

Almacenamiento en la Base de Datos:
La información contenida en el mensaje será almacenada en una base de datos relacional, específicamente en MariaDB/MySQL, para garantizar su persistencia y disponibilidad.

Objetivo del Sistema
Este flujo asegura un mecanismo robusto para la transmisión, procesamiento y almacenamiento de datos, permitiendo una comunicación eficiente entre los componentes del sistema y garantizando la integridad de la información.
