Archivos de la clase

- [14-rutas-estaticas-ejercicio.pkt](https://static.platzi.com/media/public/uploads/14-rutas-estaticas-ejercicio_772af466-d250-4de7-a34f-5db599cd07fa.pkt)

**Resumen**

## ¿Cómo configurar rutas estáticas en una red?

Configurar rutas estáticas en una red es esencial para garantizar la correcta transmisión de datos entre diferentes segmentos de red que no se encuentran directamente conectados. Aquí aprenderás a configurar rutas estáticas utilizando comandos básicos y a verificar su funcionamiento.

### ¿Qué es una ruta estática?

Una ruta estática es una dirección específica añadida manualmente a la tabla de enrutamiento de un enrutador. A diferencia de las rutas dinámicas, que se actualizan automáticamente, las rutas estáticas deben ser configuradas manualmente, proporcionando mayor control sobre el tráfico de la red.

### ¿Cómo identificar las redes en la topología?

Para empezar, debemos identificar las redes presentes en nuestra topología:

- **Red Local (LAN)**
- **Red entre enrutadores (WAN)**
- **Red de destino lejana**

Cada enrutador tendrá conocimiento de las redes a las cuales está directamente conectado. Sin embargo, no tendrá información sobre las redes más allá de sus conexiones directas a menos que se configure de manera explícita.

### ¿Cómo configurar una ruta estática?

Para configurar una ruta estática, utilizamos el comando `ip route`. Este comando requiere tres parámetros principales:

1. **Red de destino**: la red que queremos alcanzar.
2. **Máscara de subred**: para la red de destino.
3. **Próximo salto**: la IP del enrutador vecino que tiene conocimiento de cómo alcanzar la red de destino.

Supongamos que tenemos dos enrutadores que necesitan conocer las redes de la oficina opuesta. Vamos a ver cómo configurar esto.

#### Ejemplo de configuración en enrutador cero (R0):

```
ip route 192.168.1.0 255.255.255.0 192.168.0.2
```

En este caso:

- **192.168.1.0/24** es la red de la oficina dos.
- **192.168.0.2** es la IP del enrutador uno (R1) que sí tiene conocimiento de la ruta a la oficina dos.

#### Ejemplo de configuración en enrutador uno (R1):

```
ip route 192.168.0.0 255.255.255.0 192.168.1.1
```

Aquí:

- **192.168.0.0/24** es la red de la oficina uno.
- **192.168.1.1** es la IP del enrutador cero (R0) que conoce la ruta a la oficina uno.

### ¿Cómo verificar la tabla de enrutamiento?

Una vez configuradas las rutas estáticas, podemos verificar la tabla de enrutamiento utilizando el comando `show ip route`. Este comando muestra:

- **Rutas conectadas directamente**: Redes que el enrutador conoce por la configuración de sus puertos.
    
- **Rutas estáticas**: Redes configuradas manualmente para alcanzar destinos lejanos.
    
    show ip route
    

### ¿Cómo validar la correcta configuración del enrutamiento?

Para verificar que la configuración es correcta y que el enrutamiento funciona adecuadamente, realizamos una prueba de conexión. Por ejemplo, desde un servidor web con la IP `192.168.1.2`, intentamos acceder al servidor desde un computador en la red local.

Usando un navegador web, accedemos a la dirección `http://192.168.1.2`. Si la conexión es exitosa y podemos ver la Intranet, esto significa que el enrutamiento ha sido configurado correctamente.

### ¿Qué problemas comunes pueden surgir?

Al configurar rutas estáticas, pueden surgir ciertos problemas comunes:

- **Errores en la dirección IP**: Asegúrate de especificar correctamente la IP del próximo salto.
- **Máscara de subred incorrecta**: Verifica que la máscara de subred sea la adecuada para la red de destino.
- **Interrupciones en la conectividad**: Revisa que no existan fallos físicos en las conexiones de red.

### ¿Cómo practicar la configuración de rutas estáticas?

Práctica recomendada para afianzar el conocimiento:

1. **Configurar rutas estáticas en una topología simulada**: Utiliza simuladores de red como Cisco Packet Tracer.
2. **Modificar las configuraciones**: Cambia las IPs y subredes para adaptarse a diferentes escenarios.
3. **Realizar pruebas de conectividad**: Verifica el enrutamiento accediendo a diferentes servidores o utilizando herramientas como `ping` y `traceroute`.

¡No olvides probar diferentes configuraciones y escenarios! La práctica constante te ayudará a dominar la configuración de rutas estáticas y asegurar una red eficiente y confiable.