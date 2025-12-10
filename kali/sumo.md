# SUMO 

### Encontramos como hemos hecho en la practica anterios que puertos tiene abiertos, como hemos visto el 80, vamos a entrar por ahi, vemos que hay estos directorios

![cap](../img/sumo1.png)

### Entramos en el hint y vemos en el codigo fuente que hay algo escondido, vamos a desecriptarlo

![cap](../img/sumo2.png)

### Esto dice

![cap](../img/sumo3.png)

### Entramos en el fotocd y vemos esto que buscamos y sabemos que es un brainfuck

![cap](../img/sumo4.png)

### Aqui encontramos que ficheros hay escondidos, vemos que hay uno que se llama entry.js, que sera el usuario

![cap](../img/sumo5.png)

![cap](../img/sumo6.png)

### Aqui esta la traduccion del brainfuck, vemos que esta encriptado, en base 32

![cap](../img/sumo7.png)

### Lo desecriptamos y nos da la contraseña del usuario de arriba

![cap](../img/sumo8.png)

### Entramos y vemos que hemos conseguido la primera bandera, y el fichero .zip que nos da esta ruta en el http

![cap](../img/sumo9.png)

### Le pasamos el .zip a john porque tiene contraseña, y la averiguamos 

![cap](../img/sumo10.png)

### Esto es lo que hay dentro del zip

![cap](../img/sumo11.png)

### Encontramos los ficheros que tienen permisos para que podamos entrar

![cap](../img/sumo12.png)

### Entramos dentro de masayuki y vemos esto que tenemos

![cap](../img/sumo13.png)

## Encontramos el fichero user2.txt de esta manera

![cap](../img/sumo14.png)

### Tambien encontramos este fichero note.txt

![cap](../img/sumo15.png)

### Pasamos a base 32 y vemos que esta es la contraseña de masayuki

![cap](../img/sumo16.png)

### Ya podemos entrar dentro de masayuki

![cap](../img/sumo17.png)

### Entramos dentro de ftp que tiene permisos de sudo, y ya dentro entramos en una shell que es root, y ya podemos entrar en la carpeta de root que es lo que nos pedia y vemos el txt que nos dice que nos hemos pasado el juego al encontrar la ultima bandera

![cap](../img/sumo18.png)

## DAVID MORENO RODRIGUEZ


