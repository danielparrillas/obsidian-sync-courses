![[Pasted image 20260120080656.png]]
*Esta imagen estaba en el doc word de los ejercicios, pero no parece tener ninguna relación con los tales.*

Usando lo aprendido en la clase responde:

1.       **¿Cuál es la máscara para una red donde quepan 1000 hosts?**
	- 255.255.252.0
	- Prefijo: /22
	- Bits de host: 10
	- Hosts utilizables: 1022

2.       **¿Cuál es la máscara para una red donde quepan 1.000.000 hosts?**
	- 255.240.0.0
	- Prefijo: /12
	- Bits de host: 20
	- Hosts utilizables: 1,048,574

3.       **¿Cuál es la máscara para una red donde quepan 128 hosts?**
	- 255.255.255.0
	- Prefijo: /24
	- Bits de host: 8
	- Hosts utilizables: 254

4.       **¿Cuál es la máscara para una red donde quepan 126 hosts?**
	- 255.255.255.128
	- Prefijo: /25
	- Bits de host: 7
	- Hosts utilizables: 126

5.       **¿Por qué las preguntas 3 y 4 tienen respuestas diferentes?**
Porque se debe tomar en cuenta solo la cantidad de hosts utilizables, si se llega a pasar deberá utilizarse una máscara de red que permitá una cantidad mayor o igual.

Cuántos hosts son capaces de albergar las siguientes máscaras

| Máscara       | Hosts |
| ------------- | ----- |
| 255.248.0.0   |       |
| 255.255.248.0 |       |
| 255.255.128.0 |       |
| 255.192.0.0   |       |
| 255.255.255.0 |       |
### Clases
[[04 - Clases de Direccionamiento IP - Características y Usos]]
[[05 - Fundamentos de programación en Python para principiantes]]
[[06 - Direccionamiento de Redes Empresariales - Máscaras y Topologías]]
[[Tabla CIDR IPv4 1 - 32]]

