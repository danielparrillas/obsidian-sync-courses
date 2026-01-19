**Resumen**

## ¿Cómo calcular máscaras de red utilizando valores binarios?

Calcular máscaras de red puede parecer complicado al principio, pero aplicando los conceptos de números binarios podemos simplificar este proceso. En esta guía, entenderás cómo calcular estos valores cruciales para redes informáticas usando una tabla en Excel y algunos ejemplos prácticos.

### ¿Qué son las máscaras de red y cómo se construyen en Excel?

Los números binarios y las máscaras de red están estrechamente relacionados. Las máscaras de red indican cuántas máquinas puede tener una red específica. Vamos a usar Excel para visualizar y construir estas máscaras.

1. **Inicializar la tabla**:

- Comienza con todas las posiciones en ceros. Esto significa que el valor inicial es 0.

1. **Actualizar los valores de manera secuencial**:

- Primera posición en uno, seguida de siete ceros: 128
- Dos posiciones en uno, seguidas de seis ceros: 192 (128 + 64 = 192)
- Tres posiciones en uno, seguidas de cinco ceros: 224 (192 + 32 = 224)

```plaintext
| Binario   | Decimal |
|-----------|---------|
| 10000000  | 128     |
| 11000000  | 192     |
| 11100000  | 224     |
| 11110000  | 240     |
| 11111000  | 248     |
| 11111100  | 252     |
| 11111110  | 254     |
| 11111111  | 255     |
```

Estos valores se derivan sumando consecutivamente potencias de dos adyacentes.

### ¿Cómo se forman las máscaras válidas?

Las máscaras válidas siempre tienen una secuencia de unos seguidos de ceros. Por ejemplo:

- 00000000 = 0
- 10000000 = 128
- 11000000 = 192
- 11111111 = 255

Lo más importante es que los unos van primero y una vez que aparece un cero, los siguientes serán todos ceros.

### ¿Cómo afectan los unos y ceros en una máscara?

La porción de "unos" en una máscara define qué parte del IP corresponde al identificador de red, mientras que los "ceros" definen la parte referente al número de hosts. Contar el número de ceros te ayudará a determinar cuántas máquinas puedes direccionar en una red utilizando la fórmula (2^N - 2), donde (N) es el número de ceros.

### Ejemplos de cálculo de hosts

1. **Con 8 ceros**:

- ( 2^8 - 2 = 256 - 2 = 254 ) hosts

1. **Con 12 ceros**:

- ( 2^{12} - 2 = 4096 - 2 = 4094 ) hosts

1. **Con 16 ceros**:

- ( 2^{16} - 2 = 65536 - 2 = 65534 ) hosts

### ¿Cómo calcular la máscara para un número determinado de hosts?

1. Si necesitas 60 hosts:

- La potencia de dos más cercana por encima de 60 es ( 2^6 = 64 ).
- La fórmula sería ( 2^6 - 2 = 64 - 2 = 62 ) hosts.
- Una máscara con 6 ceros: 255.255.255.192

1. Si necesitas 7000 hosts:

- La potencia de dos más cercana por encima de 7000 es ( 2^{13} = 8192 ).
- La fórmula sería ( 2^{13} - 2 = 8192 - 2 = 8190 ) hosts.
- Una máscara con 13 ceros: 255.255.240.0

### Ejercicio para practicar

A continuación, te dejo con un reto para que apliques lo aprendido:

- **Problema**: Calcula la máscara necesaria para una red que necesita 500 hosts.
- **Pista**: Encuentra la potencia de dos más cercana a 500 y recuerda restar 2 para las direcciones de red y broadcast.

Practica estos cálculos y refuerza tu entendimiento sobre el tema. Cada vez que trabajes con más ejemplos, verás cómo se simplifican estos procesos. ¡Continúa practicando y expandiendo tus conocimientos!

- Tabla 1

| 2^7 | 2^6 | 2^5 | 2^4 | 2^3 | 2^2 | 2^1 | 2^0 | Resultado |
| --- | --- | --- | --- | --- | --- | --- | --- | --------- |
| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |           |
| 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0         |
| 1   | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 128       |
| 1   | 1   | 0   | 0   | 0   | 0   | 0   | 0   | 192       |
| 1   | 1   | 1   | 0   | 0   | 0   | 0   | 0   | 224       |
| 1   | 1   | 1   | 1   | 0   | 0   | 0   | 0   | 240       |
| 1   | 1   | 1   | 1   | 1   | 0   | 0   | 0   | 248       |
| 1   | 1   | 1   | 1   | 1   | 1   | 0   | 0   | 252       |
| 1   | 1   | 1   | 1   | 1   | 1   | 1   | 0   | 254       |
| 1   | 1   | 1   | 1   | 1   | 1   | 1   | 1   | 255       |
- Tabla 2


- [[03 - EJERCICIO DE CÁLCULO DE TAMAÑO DE MÁSCARAS]]