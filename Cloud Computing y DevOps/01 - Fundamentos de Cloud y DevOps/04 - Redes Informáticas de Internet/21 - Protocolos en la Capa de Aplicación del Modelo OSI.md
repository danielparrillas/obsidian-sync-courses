Lecturas recomendadas
- [SampleCaptures - The Wireshark Wiki](https://wiki.wireshark.org/SampleCaptures)

**Resumen**

La capa de aplicación es la capa final del [modelo OSI](https://platzi.com/clases/2225-redes/35587-modelo-osi/), donde tenemos contacto directo con los usuarios finales, también agrega un cierto nivel de seguridad.

## ¿Qué es la capa de aplicación?

La capa de aplicación está compuesta por:

- **Aplicaciones:** programas que utiliza el usuario final para comunicarse en la red, sean programas de mensajería, navegadores web, clientes de correo electrónico, etc.
- **Servicios:** los servicios son los programas que el usuario no ve, pero que son necesarios para que las aplicaciones funcionen correctamente. Estos servicios son por ejemplo, la transferencia de archivos, funciones de prioridades en red, cola de impresión en red, etc.  
    Los servicios deben implementar varios protocolos, ya que son muchas las distintas aplicaciones que se comunican en una red.
- **Protocolos:** los protocolos establecen reglas para el intercambio de datos entre las diferentes aplicaciones y servicios instalados en los dispositivos de origen y destino dentro de una red. Además, los protocolos son los encargados de estructurar los mensajes que se envían entre origen y destino.

## **Protocolos de la capa de aplicación**

### **Telnet (Tel**etype **Network - Red de teletipo)**

Nos permite acceder a otra máquina para manejarla remotamente como si estuviéramos sentados delante de ella.

### **POP (Post Office Protocol - Protocolo de oficina de correo)**

Es usado para recuperar mensajes de correo electrónico de un mail server a un cliente de correo, la versión más reciente es **POP3.**

---

☝ Todos estos protocolos nos proporcionan la información de control y su formato necesario para las funciones de comunicación más comunes dentro de Internet.

---

### **Banderas:**

En el campo **“Flags”** se pueden activar distintas acciones TCP para organizar la comunicación y el procesamiento de datos. Las flags, que se ajustan o no para estas activaciones, son las siguientes:

- **URG**. La etiqueta “Urgent” (en español, “urgente”) señaliza a la aplicación TCP que los datos de uso hasta el Urgent-Pointer (véase más abajo) fijado se deben procesar inmediatamente.
- **ACK**. Junto con el número de confirmación, ACK sirve para confirmar la recepción de paquetes TCP. Si no se ha ajustado la etiqueta, el número de confirmación se convierte en inválido de forma automática.
- **PSH**. “Push” sirve para facilitar un segmento TCP inmediatamente sin tener que pasar por el buffer de datos del emisor y el receptor.
- **RST**. Si ha surgido un error durante la transmisión, la aplicación se puede restablecer mediante un paquete TCP con _flag_ RST (“Reset”) ajustado.
- **SYN**. Los mensajes con una etiqueta SYN representan el primer paso del triple apretón de manos, es decir, inician el establecimiento de conexión.
- **FIN**. “Finish” señaliza a la contraparte que uno de los interlocutores de la comunicación ha finalizado la transmisión.