Lecturas recomendadas

- [What Is NsLookup? Use Our Online Tool To Query DNS Records - Network Tools](https://network-tools.com/nslookup/)

**Resumen**
## ¿Qué es un DNS y por qué es importante?

Las direcciones en internet están representadas en forma de números que solo las máquinas pueden entender. Sin embargo, como los humanos no somos buenos para recordar largas secuencias de números, se inventó una forma más amigable para las personas: la traducción de nombres en lugar de números. Esta traducción se lleva a cabo a través del servicio de DNS (Domain Name System).

## ¿Cómo funciona un DNS?

El DNS es un sistema que permite traducir nombres de dominio, como platzi.com, en direcciones IP numéricas que las máquinas pueden interpretar. Cuando ingresamos una dirección web en un navegador, el servicio de DNS se encarga de encontrar la dirección IP correspondiente para llevarnos al sitio deseado.

### ¿Qué son los registros DNS?

Los registros DNS son entradas que indican qué significa cada número en el sistema. Estos registros están clasificados en diferentes categorías:

- **SOA (Start of Authority)**: Es el registro principal, administra todos los registros asociados a un dominio.
- **Main Server**: Servidor de nombres que responde con la dirección IP de una máquina cuando se le pregunta por un nombre de dominio.
- **Secondary Main Servers**: Existen por redundancia para asegurar la disponibilidad del servicio.
- **Registro tipo A**: Mapea un nombre de dominio directamente a una dirección IP.
- **Registro CNAME**: Es un alias que permite asociar múltiples nombres de dominio a la misma dirección IP.

## ¿Cuáles son otros tipos de registros DNS?

Además de los tipos mencionados, existen otros registros importantes:

- **Registro MX**: Identifica el servidor de correo de un dominio.
- **Registro AAAA**: Similar al registro A, pero para direcciones IPv6.
- **Registro PTR**: usado para la validación inversa de servidores de correo.

### ¿Cómo consultar registros DNS?

Para consultar registros DNS, podemos utilizar herramientas como _dig_ (Domain Information Groper). Aquí un ejemplo de cómo hacerlo:

#### Consultar el tipo A de un dominio

```
dig platzi.com A
```

Esto devolverá la dirección IP asociada al dominio.

#### Consultar los servidores de correo de un dominio

```
dig platzi.com MX
```

Esto nos muestra los servidores de correo que atienden el dominio especificado.

### ¿Cómo configurar registros DNS?

El proceso de configuración de un registro DNS puede realizarse a través de consolas de administración de servicios de DNS de proveedores como GoDaddy. Aquí te mostramos un ejemplo general de cómo agregar un alias en un proveedor:

#### Agregar un alias en GoDaddy

1. Iniciar sesión en la consola de administración del servicio de DNS.
2. Ir a la sección de configuración de DNS.
3. Agregar un nuevo registro de tipo 'Alias' o 'CNAME'.
4. Especificar el nombre del alias y la dirección IP o nombre de dominio al que debe apuntar.
5. Configurar el tiempo de vida (TTL - Time To Live) del registro para controlar su expiración.

### Ejemplo práctico

Si deseas crear un alias llamado _prueba_ que apunte a la raíz del dominio:

```
Alias: prueba
Apunta a: @
TTL: 3600 (segundos)
```

Después de agregar el registro, es importante entender que la propagación de los cambios puede tardar hasta 24 horas. Para forzar la actualización y verificar los cambios, se puede utilizar el comando dig especificando el servidor DNS directamente.

#### Verificar actualización con dig

```
dig @servidor.dns prueba.hacemoscontactos.com
```

Esto devuelve la dirección IP actualizada del alias.

### Notas y consejos adicionales

- **Configuración redundante**: Asegúrate de tener servidores secundarios para evitar caídas del servicio.
- **Buena práctica IPv6**: Configura registros AAAA para asegurar la compatibilidad con la nueva versión del protocolo de Internet.
- **Validación de registros PTR**: Importante para conferir autoridad en servidores de correo.

El DNS es un componente esencial de la infraestructura de Internet que facilita la usabilidad para los usuarios y la eficiencia en la comunicación entre máquinas. Continúa aprendiendo y explorando más sobre la configuración y administración de DNS para mantener una comprensión sólida y actualizada en este campo.