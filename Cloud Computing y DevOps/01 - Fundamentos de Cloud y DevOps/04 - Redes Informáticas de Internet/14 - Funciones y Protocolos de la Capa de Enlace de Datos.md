https://platzi.com/cursos/redes/capa-de-enlace-de-datos/
**Resumen**

La capa de enlace de datos es responsable de la transferencia fiable de información a través de un circuito de transmisión de datos. Es la segunda capa del [modelo OSI](https://platzi.com/clases/2225-redes/35587-modelo-osi/).

## ¿Qué es la capa de enlace de datos?

La capa de enlace de datos recibe peticiones de la capa de red y utiliza los servicios de la capa física.

Lo que hace esta capa para evitar errores es que divide los datos en “tramas” (unidad de envío de datos que verifica que no sean muy chicas [runts](https://community.cisco.com/t5/other-network-architecture/what-is-a-giant-and-a-runt/td-p/85513) y ni muy grandes [giants](https://community.cisco.com/t5/other-network-architecture/what-is-a-giant-and-a-runt/td-p/85513)) haciéndola más confiable ya que también verifica que se hayan recibido bien los datos.

## Protocolos de la capa de enlace de datos

### **Ethernet**

Es un estándar de redes de área local para computadoras, por sus siglas en español Acceso Múltiple con Escucha de Portadora y Detección de Colisiones. Su nombre procede del concepto físico de éter.

#### **Subcapas LLC y MAC**

Dentro de la capa de enlace de datos (DLL), la IEEE 802 seccionó la misma en dos sub-capas, la subcapa LLC (Logical Link Control) o subcapa de control de enlace lógico y la subcapa MAC (Media Access Control) o subcapa de control de acceso al medio.

**MAC:** se refiere a los protocolos que sigue el host para acceder a los medios físicos, fijando así cuál de los computadores transmitirá datos binarios. Se encarga de la topología lógica de la red y del método de acceso a esta, cabe destacar que cada tecnología de red tiene una subcapa MAC diferente, y en esta residen las direcciones MAC.

**LLC:** transporta los datos de protocolo de la red, un paquete IP, y agrega más información de control para ayudar a entregar ese paquete IP en el destino, agregando los componentes de direccionamiento: el Punto de Acceso al Servicio Destino (DSAP) y el Punto de Acceso al Servicio Fuente (SSAP). Luego este paquete IP reempaquetado viaja hacia la subcapa MAC para que la tecnología específica requerida le adicione datos y lo encapsule.

[Referencias de MAC y LLC](https://www.mindmeister.com/es/711847057/funcionamiento-de-ethernet-subcapas-llc-y-mac)

### **VLAN (Virtual Local Area Network - Red de Área Local Virtual)**

Método para crear redes lógicas independientes dentro de una misma red física.

### **ATM (Asyncronous Transfer Mode - Modo de Transferencia Asíncrona)**

Transporte de una gama completa de tráfico de usuarios, incluidas las señales de voz, datos y video.

### **HDP (Heterogeneous Data Protocol - Protocolo de Datos Heterogéneos)**

Se considera como base para el intercambio de datos entre diferentes nodos en un sistema de software distribuido. Se propone una implementación software de este protocolo, que permite estandarizar la transmisión de datos manteniendo su mínimo volumen posible.

### **Frame Relay**

Es una técnica de comunicación mediante retransmisión de tramas para redes de circuito virtual

### **HDLC (High-Level Data Link Control - Control de Enlace de Datos de Alto Nivel)**

Es un protocolo de comunicaciones de propósito general punto a punto que opera a nivel de enlace de datos.

### **PPP (Point-to-Point Protocol - Protocolo de Punto a Punto)**

Establece una conexión directa entre dos nodos de una red.

### **Q.921**

Este protocolo multiplexa varias conexiones en un solo canal real entre usuarios.

### **Token Ring**

Este testigo permite a cualquier estación emisora de la red (anillo) enviar datos cuando llega el testigo a esa ubicación.