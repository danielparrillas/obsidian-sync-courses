**Resumen**

Recuerda que no puedes elegir las IP libremente, ya que existe un organismo regulador global llamado [ICANN](https://www.icann.org/es) encargado de supervisar su uso.

## ¿Cómo se asignan las [direcciones IP](https://platzi.com/clases/2225-redes/35585-identificando-las-redes/)?

Hay dos organizaciones que asignan direcciones IP: El **ICANN** es el organismo que regula el uso global de las IP, y la **IANA** se encarga de su asignación.

## ¿Qué rangos de asignación existen?

Hay distintas clases de direcciones IP:

- Clase A (redes grandes)
- Clase B (redes medianas)
- Clase C (redes pequeñas)
- Clase D (multicast)
- Clase E (investigación)

El uso determina la clase de IP que se utilizará.

## Tabla de las clases para asignación de dirección IP

![clases y direcciones IP.png](https://static.platzi.com/media/user_upload/Captura%20de%20Pantalla%202022-01-26%20a%20la%28s%29%207.06.56%20p.m.-207132c7-4201-4ed4-a6b7-8344a3f91d2f.jpg)

## ¿**Cómo funcionan las direcciones IP y las máscaras subred?**

---

Las direcciones IP nos permiten identificar **hosts** o dispositivos conectados a internet.He aquí una dirección IPv4 de ejemplo:

```
192.168.22.87

```

También tenemos **máscaras de subred** las cuáles sirven para conocer nuestra **dirección de red** y las direcciones IP disponibles en esa red (puesto que son limitadas).He aquí una máscara de subred típica para redes **LAN** (usualmente redes de hogar):

```
255.255.255.0

```

Puedes conocer tu dirección IP y máscara de subred con los siguientes comandos:

**WIndows**

```
ipconfig

```

**MacOS/Linux**

```
ifconfig

```

### **La máscara de subred**

La máscara de subred al igual que una dirección IPv4 tiene 4 **octetos** o **bytes** y dependiendo de la clase de la red pueden ser de la siguiente manera:

```
255.255.0.0
255.255.255.252
255.255.224.0
...

```

El ejemplo más común para redes **LAN** es la **_255.255.255.0_** y se puede obtener la dirección de red (esta es otorgada por el ISP o Internet Service Provider cuando contratas el servicio de internet) de la siguiente manera:

1. Se convierten en binario cada octeto de la dirección IP y las máscara de subred:

```
11000000.10101000.00010110.01010111 --> 192.168.22.87
11111111.11111111.11111111.00000000 --> 255.255.255.0

```

1. Se compara cada bit con su bit correspondiente de tal manera que **_1 y 1 = 1_** y **_1 y 0 = 0_**

```
11000000.10101000.00010110.01010111 --> 192.168.22.87
11111111.11111111.11111111.00000000 --> 255.255.255.0
-------------------------------------------------------------
11000000.10101000.00010110.00000000 --> 192.168.22.0

```

Los primeros 3 octetos de la dirección IP representan la dirección de red y los últimos representan la dirección del dispositivo conectado. Es similar a una dirección en la que la calle es la dirección de red y el número de casa es la dirección del dispositivo. La máscara de subred tiene los primeros 3 octetos llenos (255.255.255) porque la dirección de red no cambia, y el último octeto vacío (.0) puede tener hasta 256 direcciones de dispositivos.

Sin embargo, hay 2 direcciones reservadas: la dirección de red (192.168.22.0) y la dirección de broadcast (192.168.22.255). Esto deja un rango de 254 direcciones disponibles (192.168.22.1 - 192.168.22.254).