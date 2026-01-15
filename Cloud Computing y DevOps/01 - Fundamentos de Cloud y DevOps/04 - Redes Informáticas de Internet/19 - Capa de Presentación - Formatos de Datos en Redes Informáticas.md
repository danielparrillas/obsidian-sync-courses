**Resumen**

Esta capa en el [modelo OSI](https://platzi.com/clases/2225-redes/35587-modelo-osi/) se encarga de representar la información para nuestro usuario final.

## Qué es la capa de presentación

La capa de presentación es donde los datos recibidos se convierten en un formato que la aplicación de destino puede entender. El trabajo realizado en esta capa es mejor entendido como un trabajo de traducción.

Por ejemplo, los datos se cifran con frecuencia en la capa de presentación antes de ser pasado a las otras capas para el envío. Cuando los datos se reciben, se descifran y se pasan a la aplicación de destino en el formato hizo que esta lo entiende.

## Funciones de la capa de presentación

- **Formateo de datos:** opera como traductor entre dos tipos diferentes de códigos, por ejemplo el código ampliado de caracteres decimal codificados en binario (EBCDIC), que es utilizado para representar los caracteres en la pantalla y el código americano normalizado para el intercambio de la información (ASCII), que tiene la misma función: dar formato a la información para visualizarla o imprimirla.
- **Cifrado de datos:** protege la información durante la transmisión.
- **Compresión de datos:** usa algoritmos para reducir el tamaño de los archivos, estos algoritmos, buscan patrones de bits repetidos en el archivo y entonces los reemplaza con un token (patrón de bit mucho más corto).
- **Aplicar a los datos** procesos criptográficos.
- **Definir la estructura** de datos a transmitir.

## Formatos de la capa de presentación

Algunos protocolos utilizados aquí son:

- HTML
- DOCS
- JPEG
- AVI
- MP3