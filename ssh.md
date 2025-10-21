# Tarea 4 SSH

### Instalamos ssh con el siguiente comando:

````bash
sudo apt install openssh-server
````

### • Deshabilitar passwords en blanco

![cap](./img/ssh1.png)

### • Cambiar el puerto por defecto

![cap](./img/ssh2.png)

### • Deshabilitar el login de root a través de ssh

![cap](./img/ssh3.png)

### • Deshabilitar el protocolo 1 de ssh

### Esta opcion no esta por defecto, no hace falta deshabilitarla

### • Configurar un intervalo de inactividad de la sesión

![cap](./img/ssh4.png)

### • Permitir el acceso únicamente a ciertos usuarios

![cap](./img/ssh5.png)

### Con el contenido del fichero ssh que esta en github, podemos crear una clave, pasarsela al servidor, y despues conectarnos al servidor sin contraseña, ya que tiene nuestra clave publica

![cap](./img/ssh8.png)

