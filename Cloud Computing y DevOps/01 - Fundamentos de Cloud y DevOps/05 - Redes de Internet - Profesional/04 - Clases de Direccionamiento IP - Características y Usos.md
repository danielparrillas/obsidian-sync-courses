**Resumen**

## ¿Qué es una dirección IP y cómo se divide?

Una dirección IP (Internet Protocol) es un número único que permite identificar y localizar una máquina dentro de una red. Las direcciones IP están divididas en clases y cada clase tiene características específicas que las diferencian.

### ¿Qué es la clase A?

La clase A de direcciones IP cuenta con las siguientes características:

- **Rango**: Desde 1.0.0.0 hasta 126.0.0.0
    
- **Detalle técnico**:
    
- El primer bit del primer octeto siempre está en cero.
    
- El rango va desde 0 hasta 127, pero los números 0 y 127 están reservados y no se utilizan.
    
- **Máscara de subred**:
    
    255.0.0.0
    
- **Usos**: Esta clase está diseñada para redes extremadamente grandes.
    
- Rango: **1.0.0.0 – 126.255.255.255**
    
- Bits de red: **8**
    
- Bits de host: **24**
    
- Hosts por red:  
    **2²⁴ − 2 = 16,777,214 hosts**
### ¿Qué es la clase B?

La clase B de direcciones IP presenta las siguientes características:

- **Rango**: Desde 128.0.0.0 hasta 191.255.0.0
    
- **Detalle técnico**:
    
- El primer bit del primer octeto está siempre en uno y el segundo bit está en cero.
    
- El primer octeto va desde 128 hasta 191.
    
- **Máscara de subred**:
    
    255.255.0.0
    
- **Usos**: Esta clase está destinada a redes de tamaño medio a grande.
  
- Rango: **128.0.0.0 – 191.255.255.255**
    
- Bits de red: **16**
    
- Bits de host: **16**
    
- Hosts por red:  
    **2¹⁶ − 2 = 65,534 hosts**

### ¿Qué es la clase C?

La clase C de direcciones IP se caracteriza por:

- **Rango**: Desde 192.0.0.0 hasta 223.255.255.0
    
- **Detalle técnico**:
    
- Los dos primeros bits del primer octeto están en uno y el tercer bit está en cero.
    
- El primer octeto va desde 192 hasta 223.
    
- **Máscara de subred**:
    
    255.255.255.0
    
- **Usos**: Esta clase está enfocada en pequeñas redes.
    
- Rango: **192.0.0.0 – 223.255.255.255**
    
- Bits de red: **24**
    
- Bits de host: **8**
    
- Hosts por red:  
    **2⁸ − 2 = 254 hosts**
### ¿Existe una Clase D?

Sí, la clase D está reservada para comunicaciones multicast y no para la asignación a dispositivos individuales o subredes.

- **Rango**: Desde 224.0.0.0 hasta 239.255.255.255
- **Usos**: Se utiliza en comunicaciones donde un grupo de máquinas comparten información, por ejemplo, enrutadores que envían actualizaciones entre ellos usando direcciones multicast.

### ¿Qué hay con la Clase E?

La clase E, aunque existe, no tiene aplicaciones directas sobre el direccionamiento tradicional de redes.

- **Rango**: Desde 240.0.0.0 hasta 255.255.255.255
- **Usos**: Reservadas para uso futuro o pruebas experimentales.

Mantén siempre en mente estos detalles clave sobre las clases de direcciones IP y sus características. Memorizar los rangos y máscaras de cada clase puede ser útil, pero comprender el por qué de estas divisiones te dará una ventaja considerable en la administración de redes. ¡Sigue aprendiendo y explorando!

- Rango: **224.0.0.0 – 239.255.255.255**
    
- 👉 **No permite hosts**
    
- Se usa para **multicast**, no para asignar IPs a dispositivos.

### Ejercicios
[[06 - EJERCICIO DE DIRECCIONAMIENTO]]