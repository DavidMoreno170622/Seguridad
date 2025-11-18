# EJERCICIO 2

## Vamos a repasar los diferentes errores que pueda tener esta configuracion para que sea funcional

## ERROR 1

### El primer error que encuentro es en el fichero .ovpn, el cual la remote ip, no es la que deberia de tener, 192.168.3.242 es la ip que tenia, cuando la ip publica del router de la empresa en este caso es la 192.168.3.209, eso es lo primero que hay que cambiar

## ERROR 2

### El fichero de acceso que tenemos no es correcto, vamos a modificarlo para que este bien, de client3 a client1

## ERROR 3

### En el profile de PPP el perfil que utilizamos no tiene DNS, en nuestro caso son los de la senia, vamos a adjuntarselo

## ERROR 4,5

### El siguiente error que tenia la configuracion es que al meterteen ppp OVPN Server, el certificado mostrado era el CA, cuando tiene que ser el server
### Tambien en auth, estaba seleccionado sha1 y md5, cuando en nuestra configuracion del .ovpn esta asignado que sea sha256 o sha256, esas dos mas el sha1 tienen que estar marcadas, arreglado estos errores, me ha funcionado y me a asignado la ip 192.168.200.199, que esta dentro del rango asignado

### Tengo que añadir tambien que si le cambiamos los nombres a los cerficados, tambien hay que hacerlo en el fichero

## DAVID MORENO RODRIGUEZ