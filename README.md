# despr2_1

# 1.Creacion de la VM

Crea una VM como clon enlazado de la VM base Ubuntu-Server-Base.ova proporcionada en el repositorio del curso:

[Captura 1](https://github.com/braiscastro/despr2_2/blob/main/img/Captura.png)

Con gura la red: Adaptador 1 en NAT + Port-Forward (host 8082 → guest 80; host 2224 →
guest 22; host 8444 → guest 443):

[Captura 2](https://github.com/braiscastro/despr2_2/blob/main/img/Captura2.png)

# 2.Preparacion del entorno 

Inicia la VM y accede por SSH desde el host:

[Captura 3](https://github.com/braiscastro/despr2_2/blob/main/img/Captura3.png)

Arranca la VM y actualiza paquetes:

[Captura 4](https://github.com/braiscastro/despr2_2/blob/main/img/Captura4.png)

Instala nginx

[Captura 5](https://github.com/braiscastro/despr2_2/blob/main/img/Captura5.png)

Con gura el rewall para permitir trá co HTTP y HTTPS:

[Captura 6](https://github.com/braiscastro/despr2_2/blob/main/img/Captura6.png)


# 3.Comprobación básica

Comprueba que el servicio está activo:

[Captura 7](https://github.com/braiscastro/despr2_2/blob/main/img/Captura7.png)

Desde el host, accede a http://localhost:8082/ y comprueba que ves la página por defecto de Nginx. Haz una captura de pantalla.

[Captura 8](https://github.com/braiscastro/despr2_2/blob/main/img/Captura8.png)


# 5.Con gurar un bloque de servidor (server block)

Desactiva el sitio por defecto y activa tu con guración:

[Captura 9](https://github.com/braiscastro/despr2_2/blob/main/img/Captura9.png)

# 6.Vericación
 
  Accede desde el host a http://localhost:8082 y comprueba navegación, imágenes y estilo.
  Si ves la página "Welcome to nginx!" en lugar de tu sitio, ve a la sección de Troubleshooting más abajo.
  
[Captura 10](https://github.com/braiscastro/despr2_2/blob/main/img/Captura10.png)

