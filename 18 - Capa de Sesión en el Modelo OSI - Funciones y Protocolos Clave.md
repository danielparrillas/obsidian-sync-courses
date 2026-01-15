**Resumen**

La capa de sesión sincroniza el intercambio de datos entre capas inferiores y superiores del [modelo OSI](https://platzi.com/clases/2225-redes/35587-modelo-osi/). También se le define como comunicación entre hosts.

## ¿Qué es la capa de sesión?

La capa de sesión es donde se realizan, se mantienen y se terminan las conexiones. Esto generalmente se refiere a solicitudes de aplicaciones para los datos a través de la red.

Mientras que la capa de transporte se encarga del flujo real de datos, la capa de sesión actúa como un anunciador, asegurándose que las solicitudes y envíos de datos de los programas y aplicaciones conozcan si sus solicitudes han sido completadas. En términos técnicos, la capa de sesión sincroniza la transmisión de datos.

esta capa establece un control entre quien está enviando y quien está recibiendo, para mantener este control se utilizan los "_tokens",_ que es una sustitución de datos sensibles por otros aleatorios y que se utilizarán para verificar que el que recibió los datos sea el mismo usuario y así volver a la forma inicial, como una especie de encriptación.

Otro punto importante de esta capa es que debe tener sincronización, por si algo falla pueda continuar desde el punto en el que se quedó.

## **Protocolos de la capa de sesión**

### **SIP (Session Initiation Protocol - Protocolo de inicio de sesión)**

Para la iniciación, modificación y finalización de sesiones.

### **RTP (Real Time Transport Protocol - Protocolo de Transporte en Tiempo Real)**

Define un formato de paquete estándar para el envío de audio y video sobre Internet.

### **RPC (Remote Procedure Call - Llamada a Procedimiento Remoto)**

Es un programa que utiliza una computadora para ejecutar código en otra máquina remota sin tener que preocuparse por las comunicaciones entre ambas.

### **Named Pipe**

Es la canalización unidireccional o dúplex para la comunicación entre el servidor de canalización y uno o más clientes de canalización. Se pueden utilizar para proporcionar comunicación entre procesos en la misma computadora o entre procesos en diferentes computadoras a través de una red.