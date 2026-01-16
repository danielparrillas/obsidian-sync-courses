# Instalación de Wireshark en Windows, macOS y Linux

**Wireshark** es un programa que nos sirve para capturar el tráfico de nuestra red y poder inspeccionar los diferentes paquetes que viajan por ella. Su instalación es bastante sencilla por lo que a continuación te explico cómo puedes instalarlo en cada uno de los diferentes sistemas operativos.

**Windows y macOS**

**Wireshark** tiene su propio ejecutable de instalación rápida para cada uno de estos sistemas, por lo que sólo tendrás que dar clic en instalar para que funcione correctamente. Solo debes dar [clic en este enlace](https://www.wireshark.org/download.html) para descargar dependiendo de tu sistema operativo.

Ubuntu/Debian

Para instalar **Wireshark** en Ubuntu primero asegúrate de actualizar tus repositorios con:

`sudo apt update`

Una vez termine el comando de ejecutarse, instala **Wireshark** como cualquier otro programa desde la terminal con:

`sudo apt install wireshark`

Después solo búscalo en el menú e inicia la aplicación.

![](https://lh3.googleusercontent.com/FiuW-q1o5ocZ0fFt6mpZcd1dfG3rThsPEgiiFqx8-71VvNDC_hnUD9HxYjDgWHkdKgu7OkEzmMdDfXXNi1t0g4Epjxbxj3VYGbfbwOi0m9fFtGUkPuqmtbhYEcllcCZetXRRcRSC)

Si al momento de querer capturar tráfico no te permite continuar debido a un error en los permisos de ejecución, entonces puedes correr Wireshark directo desde la terminal como **superusuario** con:

`sudo wireshark`

Esto se debe a que **Wireshark** usa tu tarjeta de red con permisos de administrador para poder escanear el tráfico.

¡Listo! Con esto ya cuentas con **Wireshark**. Nos vemos en la siguiente clase para utilizarlo en la capa de aplicación.