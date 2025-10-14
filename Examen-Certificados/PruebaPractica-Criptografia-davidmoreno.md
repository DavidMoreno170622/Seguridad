# Prueba Práctica Criptografia

### Para sacar el enunciado de esta tarea simplemente e hecho un --decrypt y he mirado en la carpeta con interfaz grafica y estaba ahi, ya que parece ser que los pdf no los lee bien cuando estan encriptados, o al hacer un cat, porque son imagenes mas que un texto

### Aqui compruebo cual es el mensaje verdadero para saber cual es el zip a descargar

![captura](./img/1.png)

### Aqui hacemos el rsync de el backup y copiar el data entero pero no la carpeta Data

![captura](./img/2.png)

### Para hacer pruebas, borramos un fichero y modificamos otro y volvemos a ejecutar el comando,vemos como el borrado se borra y el modificado se modifica

![captura](./img/3.png)

### Ahora vamos a crear una clave ssh y la vamos a copiar en la ip y usuario que queremos para que no me pida contraseña al hacer el rsync, el cual ejecuta automaticamente un ssh

![captura](./img/4.png)

### Aunque en la captura de arriba se ve como ya no nos pide contraseña, pero para asegurarnos, vamos a volver a borrar un fichero y modificar otro y ejecutar el comando rsync, y ahora vemos como no nos pide contraseña al ejecutar el comando

![captura](./img/5.png)





