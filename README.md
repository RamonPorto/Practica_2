# Practica_2
## Ejercicio 1
Para descargar la imagen de apache usaremos el siguiente comando
~~~
docker pull httpd
~~~

Para comprobar que está en nuestro equipo usamos este comando
~~~
docker images
~~~
## Ejercicio 2
Utilizaremos este comando para crear el contenedor llamado asir_apache

~~~
docker run -dit --name asir_apache -p 8000:80 -v "$PWD"/htdocs:/usr/local/apache2/htdocs/ httpd:2.4
~~~

## Ejercicio 3
Utilizamos el comando anterior para mapear los puertos de la máquina con el del contenedor gracias a 
~~~
-p 8000:80
~~~
Siendo 8000 el puerto de la máquina y 80 el puerto del contenedor.

## Ejercicio 4
También usaremos el mismo comando para que el directorio apache2 este montado en el directorio htdocs de nuestro pc gracias a 
~~~
-v "$PWD"/htdocs:/usr/local/apache2/htdocs/
~~~




