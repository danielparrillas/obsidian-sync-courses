**Resumen**

## ¿Qué son las rutas y cómo se configuran?

Hablar sobre redes y telecomunicaciones puede parecer complicado, pero vamos a descomponerlo para entender mejor cómo funcionan y se configuran las rutas en una red. Para empezar, es importante saber que las rutas se configuran en dispositivos llamados enrutadores (routers en inglés). Estos dispositivos son responsables de recibir paquetes de datos y dirigirlos a su destino a través de la red.

### ¿Cómo funcionan los enrutadores?

Los enrutadores toman decisiones cruciales sobre dónde enviar los paquetes de datos basados en las direcciones de origen y destino. Este proceso incluye identificar el puerto de entrada del paquete y decidir a través de cuál de los otros puertos debe enviarlo para alcanzar su destino.

### ¿Qué son las rutas estáticas?

Las rutas estáticas son una forma fundamental y manual de configurar la visión de un enrutador sobre toda la topología de la red a la que está conectado. Aquí detallamos el proceso paso a paso para tener una mejor compresión:

- **Configuración Manual:** En las rutas estáticas, se debe configurar manualmente cada conexión en la topología de la red. Es decir, se especifica manualmente al enrutador todas las redes a las que va a estar conectado y las rutas para alcanzar las redes no directamente conectadas.
    
- **Ejemplo Práctico:** Pensemos en una ciudad. Si estás en una casa particular, hay calles cercanas a ti, pero también habrá otras que están más alejadas. Para llegar a otra ciudad, podrías usar una autopista que conecta tu ciudad con la de destino. Al conducir, necesitas conocer la ubicación de esa autopista y las calles que te llevan a ella. De la misma manera, en una ruta estática, el enrutador necesita saber todas las "calles" y "autopistas" de la red.
    

### Ventajas y desventajas de las rutas estáticas

Como toda tecnología, las rutas estáticas tienen sus pros y contras, las cuales se resumen a continuación:

- **Ventajas:**

1. **Simplicidad:** Son fáciles de entender y configurar en topologías pequeñas.
2. **Estabilidad:** No cambian a menos que se reconfiguren manualmente, lo que puede reducir la variabilidad en el funcionamiento de la red.

- **Desventajas:**

1. **Escalabilidad:** Requieren un esfuerzo considerable para configurarse en topologías grandes, siendo poco prácticas.
2. **Mantenimiento:** Cada cambio en la red requiere una actualización manual de las rutas.

### ¿Qué sigue después de las rutas estáticas?

Aunque las rutas estáticas son útiles en redes pequeñas, se vuelven imprácticas a medida que la topología de la red crece en tamaño y complejidad. Por esto, en redes más grandes, se utilizan métodos más avanzados y eficientes que veremos más adelante.

---

Recuerda, aunque este tema puede parecer técnico, entender los fundamentos permite tener una base sólida sobre cómo fluye la información en nuestras redes cotidianas.