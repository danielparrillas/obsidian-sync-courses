# Dispositivos de Hardware de Red y su Función en la Arquitectura
**Resumen**

Los **dispositivos de red** son equipos físicos que se conectan a una red para transmitir y recibir datos. Su propósito es intercambiar paquetes de información entre una computadora o servidor local y otros dispositivos.

Estos equipos incluyen computadoras, impresoras, switchs, hubs, routers, repetidores, adaptadores de red, puntos de acceso inalámbricos y facilitan la transferencia de información entre los usuarios conectados a la red pública o privada.

## 8 tipos de dispositivos de red

Existen diferentes **tipos de dispositivos de redes** y estos son los más utilizados.

![tipos-dispositivos-de-red (1).png](https://static.platzi.com/media/user_upload/tipos-dispositivos-de-red%20%281%29-8cfaf3f0-4248-498b-bae3-2591f99f7667.jpg)

### 1. Hub

El **Hub** conecta computadoras en una red local, replicando y transmitiendo datos instantáneamente a todos los dispositivos conectados. No permite acceso a Internet ni envía información a computadoras específicas, ya que copia y envía la información recibida por igual a todos los dispositivos en la red.

### 2. Switch

El **switch** es un dispositivo que se emplea para conectar equipos en red, formando una red de área local (LAN) y se encarga de la interconexión de equipos cableados con Ethernet de una misma red.

- **Switch capa 2:** utiliza direcciones MAC, sin considerar IP u otros elementos de capas superiores.
- **Switch capa 3:** tiene tabla de direcciones MAC y tabla de enrutamiento IP, controla comunicación intra-VLAN y enrutamiento entre VLAN.

### 3. Módem

El **módem** es un dispositivo que convierte las señales digitales en analógicas y viceversa. También permite la conexión de dispositivos electrónicos a una red de comunicación, como Internet, facilitando la transmisión de datos a través de líneas telefónicas o cables de fibra óptica.

### 4. Repetidor

El **repetidor** es un dispositivo analógico que amplifica una señal de entrada, independientemente de su naturaleza. Gracias a su versatilidad desempeña un papel clave en la mejora de la calidad y el alcance de las señales en diferentes contextos y entornos de comunicación.

### 5. Firewall

**Un firewall** es un dispositivo de seguridad de la red que monitorea el tráfico de red entrante y saliente, y decide si permite o bloquea tráfico específico en función de un conjunto definido de reglas de seguridad.

También pueden ser lógicos, como un WAF (Web Application Firewall), que puede bloquear parte del tráfico web. Actualmente, existen de distintos tipos según sus funciones:

- **Firewalls Perimetrales**: también conocidos como Next Generation Firewalls, operan en capa 7 para identificar aplicaciones y establecer protecciones más allá de puertos/protocolos. Ejemplos: Palo Alto Networks, CheckPoint, Fortinet y Cisco.
    
- **Firewall de Aplicaciones Web** (WAF): protegen servicios web, locales o en la nube. Complementados con servicios de protección DDoS.
    
- Variante adicional: **Firewall de Base de Datos** (DBF), controla bases de datos, permite auditorías detalladas según funciones de cada DBA y enmascaramiento de BD.
    

### 6. Balanceador de cargas de red

Un **balanceador de cargas de red** distribuye el tráfico de TCP o UDP entre las instancias de máquina virtual (VM) de una misma región. Puede recibir tráfico de los siguientes servidores: cualquier cliente en Internet. VM de Google Cloud con IP externas.

### 7. Gateway

Un **gateway**, o puerta de enlace, se refiere a una tecnología que permite interconectar redes con protocolos y arquitecturas diferentes a todos los niveles de comunicación. Lo que hace es traducir la información del protocolo utilizado en una red al protocolo usado en la red de destino.

### 8. Puente

Por último, el **puente** de red es un equipo de interconexión de redes de computadoras que interconecta segmentos de red haciendo la transferencia de datos de una red hacia otra con base en la dirección física de destino de cada paquete.

## Tipos de switches

- Desktop
- Perimetrales no gestionables
- Perimetrales gestionables
- Troncales de prestaciones medias
- Troncales de altas prestaciones