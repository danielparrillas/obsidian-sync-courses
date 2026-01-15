**Resumen**

La capa de transporte es el cuarto nivel del [modelo OSI](https://platzi.com/clases/2225-redes/35587-modelo-osi/) que sirve para regular el flujo de información desde el origen hasta el destino.

## ¿Que es la capa de transporte?

La capa de transporte es responsable de la transmisión de datos a través de la red. En este nivel, los datos no conceptualizan en términos de paquetes individuales, sino más bien en términos de una conversación. Para lograr esto, se utilizan protocolos que se definen como “reglas de la comunicación.

Los protocolos ven la transmisión completa de los muchos paquetes comprobando los errores en la conversación, reconociendo las transmisiones exitosas y solicitando la retransmisión de las mismas si se detectan errores.

La capa de red y la capa de transporte trabajan en conjunto como un sistema postal. La capa de red se ocupa de direccionar los datos, al igual que una persona se direcciona un sobre. A continuación, la capa de transporte actúa como la oficina local de correos del remitente, ordenando y agrupando todos los datos con la misma dirección de manera similar en envíos más grandes con destino a otras oficinas locales, donde estos datos serán entregados.

## **Protocolos de la capa de transporte**

### **SCTP (Stream Control Transmission Protocol - Protocolo de Transmisión de Control de Flujo)**

Es un protocolo de comunicación.

### **SSL (Secure Socket Layer - Capa de Puertos Seguros)**

El protocolo SSL es el predecesor del protocolo TLS y la tecnología estándar para mantener segura una conexión a Internet, así como para proteger cualquier información confidencial que se envía entre dos sistemas e impedir que los delincuentes lean y modifiquen cualquier dato que se transfiera, incluida información que pudiera considerarse personal.

Los dos sistemas pueden ser un servidor y un cliente (por ejemplo, un sitio web de compras y un navegador) o de servidor a servidor (por ejemplo, una aplicación con información que puede identificarse como personal o con datos de nóminas).

### **TLS (Transport Layer Security - Seguridad de la Capa de Transporte)**

Se trata de protocolos criptográficos que proporcionan privacidad e integridad en la comunicación entre dos puntos en una red de comunicación. Esto garantiza que la información transmitida por dicha red no pueda ser interceptada ni modificada por elementos no autorizados, garantizando de esta forma que sólo los emisores y los receptores legítimos sean los que tengan acceso a la comunicación de manera íntegra.

### TCP (**_Transmission Control Protocol)_**

Prioriza confiabilidad sobre rapidez, verifica del mensaje.

### UDP (User Datagram Protocol)

Prioriza rapidez sobre confiabilidad, solo envia el mensaje.