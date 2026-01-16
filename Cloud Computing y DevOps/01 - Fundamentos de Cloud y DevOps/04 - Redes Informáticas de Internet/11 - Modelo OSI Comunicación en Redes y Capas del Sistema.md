# Modelo OSI Comunicación en Redes y Capas del Sistema
**Resumen**

El **modelo OSI** es un marco utilizado para comprender cómo funcionan juntos los diferentes sistemas de comunicación. Divide el proceso de envío y recepción de datos a través de una red en siete capas, cada una de las cuales realiza una función específica.

Este fue desarrollado por la **Organización Internacional para la Estandarización** (ISO), a fines de la década de **1970**, como una manera de estandarizar el trabajo de distintos sistemas de comunicación y proporcionar una estructura lógica y organizada para el intercambio de datos.

## ¿Cómo funciona el modelo OSI?

**El modelo cuenta con 7 capas** que enumeraremos de abajo hacia arriba.

- Capa física
- Capa de enlace de datos
- Capa de red
- Capa de transporte
- Capa de sesión
- Capa de presentación
- Capa de aplicación

![modelo OSI.png](https://static.platzi.com/media/user_upload/Captura%20de%20Pantalla%202022-01-26%20a%20la%28s%29%207.18.25%20p.m.-c9668c1c-6cea-4114-a78f-a37d97f00bea.jpg)

## ¿Cuáles son las siete capas del modelo OSI?

Este estándar de redes para computadoras se maneja por capas porque cada una involucra una tarea específica y se comunica con la capa inmediatamente inferior o superior para ejecutar su función y por eso a continuación **te explicaremos cada una de ellas de abajo hacia arriba.**

### 1. Capa física

![Capa 1](https://static.platzi.com/media/user_upload/Captura%20de%20Pantalla%202023-06-15%20a%20la%28s%29%207.29.53%20p.m.-27e9ff21-13c2-476c-a858-d42cc28eeeab.jpg)

La [capa física](https://platzi.com/clases/2225-redes/35588-capa-fisica/) se ocupa de la conexión física entre dispositivos. Por ejemplo, como la transmisión de datos a través de un cable de cobre o fibra óptica (electricidad, cables, hardware). Algunas de las funciones que tiene la capa física son:

- Establecer y mantener la conexión física entre dispositivos
- Especificar el tipo de medio de transmisión
- Controlar el flujo de datos
- Detectar y corregir errores
- Convertir datos en señales físicas

### 2. Capa de enlace de datos

![Capa 2](https://static.platzi.com/media/user_upload/Captura%20de%20Pantalla%202023-06-15%20a%20la%28s%29%207.29.59%20p.m.-37bea52b-da09-44ce-a528-5ceb84722fac.jpg)

Esta [capa de enlace de datos](ttps://platzi.com/clases/2225-redes/35590-capa-de-enlace-de-datos/) es responsable de establecer y mantener un enlace entre dispositivos, asegurando que los datos se transmitan de manera precisa y eficiente. También realiza la verificación y corrección de errores para garantizar que los datos se reciban correctamente.

En esta capa:

- Se envían los datos que se convirtieron a bits
- Se le añade información sobre el direccionamiento físico
- Se llega a la capa de red

### 3. Capa de red

![Capa 3](https://static.platzi.com/media/user_upload/Captura%20de%20Pantalla%202023-06-15%20a%20la%28s%29%207.30.05%20p.m.-780ba6a5-a96d-4132-9ee7-4a31fd035e26.jpg)

De otro modo, la [capa de red](https://platzi.com/clases/2225-redes/35591-capa-de-red/) se encarga de enrutar datos entre dispositivos en una red, también determina la ruta más eficiente para que viajen los datos y garantiza que lleguen a su destino. Algunas de las funciones de la capa de red son:

- Enrutamiento de datos
- Direccionamiento de dispositivos
- Fragmentación y reensamblaje de paquetes
- Control de congestión

### 4. Capa de transporte

![Capa 4](https://static.platzi.com/media/user_upload/Captura%20de%20Pantalla%202023-06-15%20a%20la%28s%29%207.30.12%20p.m.-9d858511-6992-4201-a416-618a6cb84d38.jpg)

Esta [capa de transporte](https://platzi.com/clases/2225-redes/35592-capa-de-transporte/) tiene el objetivo de garantizar que los datos se entreguen de manera confiable y en el orden correcto. Agrega control de flujo y comprobación de errores para garantizar que los datos no se pierdan ni se corrompan durante la transmisión. Se encuentran protocolos como TCP.

- Control de flujo
- Control de errores
- División y reensamblaje de paquetes (datos más pequeños)

### 5. Capa de sesión

![Capa 5](https://static.platzi.com/media/user_upload/Captura%20de%20Pantalla%202023-06-15%20a%20la%28s%29%207.30.19%20p.m.-496970b8-94ac-42b3-ba5b-8f6b3ca6e238.jpg)

Después, la [capa de sesión](https://platzi.com/clases/2225-redes/35593-capa-de-sesion/) tiene como fin establecer, mantener y terminar las conexiones entre dispositivos. Permite que los dispositivos se comuniquen entre sí y coordinen sus actividades. Entre sus funciones está:

- Establecer conexiones
- Mantener esos enlaces
- Dar fin a esas conexiones

### 6. Capa de presentación

![Capa 6](https://static.platzi.com/media/user_upload/Captura%20de%20Pantalla%202023-06-15%20a%20la%28s%29%207.30.25%20p.m.-22fd50ea-1439-454a-950c-9985c4257329.jpg)

Esta [capa de presentación](https://platzi.com/clases/2225-redes/35594-capa-de-presentacion/) es responsable de convertir los datos a un formato que pueda ser entendido por el dispositivo receptor. También maneja el cifrado y la compresión de datos para garantizar que se transmitan de manera segura y eficiente. Formatea los datos para transferirlos a la siguiente capa.

Entre las funciones de la capa de presentación está:

- Codificación y decodificación de datos
- Compresión y descompresión de datos

### 7. Capa de aplicación

![Capa 7](https://static.platzi.com/media/user_upload/Captura%20de%20Pantalla%202023-06-15%20a%20la%28s%29%207.30.36%20p.m.-aaf2a081-7950-40fc-a336-fb05d96841eb.jpg)

Esta [capa de aplicación](https://platzi.com/clases/2225-redes/35595-capa-de-aplicacion/) es el nivel más alto del modelo OSI y es responsable de brindar servicios al usuario. Permite a los usuarios interactuar con la red y acceder a los recursos que necesitan.

## Diferencia entre modelo OSI y modelo TCP/IP

A diferencia del Modelo OSI, el [Modelo TCP/IP](https://platzi.com/clases/2225-redes/35584-modelo-tcpip/) no se divide en capas separadas y definidas con la misma rigurosidad. En lugar de eso, consta de cuatro capas interconectadas que abordan diferentes aspectos de la comunicación en redes.

Si bien el Modelo OSI puede considerarse desactualizado en términos de implementación práctica, sigue siendo una herramienta valiosa para comprender los principios fundamentales de la comunicación en redes.

> Descubre más acerca de la [dirección MAC](https://platzi.com/clases/2225-redes/36043-direccionamiento-mac/)
