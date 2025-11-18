# PREGUNTAS TEORICAS

**¿Es necesario crear un perfil en el apartado PPP? Razona la respuesta.**

### No lo es en verdad, pero como nosotros en el fichero .ovpn tenemos la regla auth-user-pass si que necesitariamos el perfil, en resumen, si nosotros le decimos al servidor openvpn que nos vamos a conectar con un perfil y contraseña, si que lo necesitamos, si no, no es necesario

**¿Qué indica Local Address si creamos un perfil en el apartado PPP?**

### Local address en el apartado de perfil en PPP significa el gateway que va a tener la red que nos dara, por eso le tenemos que poner una ip del rango que le asignemos en el pool, tiene que estar fuera de este pero tiene que ser de la misma red, por ejemplo pool de la 192.168.0.50-192.168.0.100/24, si este es nuestro pool, nuesta local address tiene que estar entre la 192.168.0.0 y la 192.168.0.255, obviando que de la 50 y 100 no podemos utilizar porque son las ip que va a recibir los equipos que se conecten a la vpn, en resumen, si ponemos 192.168.0.254 en local address y tenemos la pool 192.168.0.50-192.168.0.100/24, al conectarnos nos dara una ip entre la 50 y la 100 y nuestro gateway sera 192.168.0.254

**En el fichero de configuración del cliente OpenVPN se referencia la CA y los ficheros .crt y . key. Sin embargo en el servidor OpenVPN del MikroTik no se hace  referencia para nada a los ficheros .crt y .key. Explica entonces para qué sirven y por qué funciona la conexión y es fiable.**

### Sirver como seguridad, ya que estas son como si fuera la clave publica y la clave privada, asi solo se pueden conectar aquellos que de verdad tengan el fichero, y la contraseña de este

**¿Por qué es necesario añadir una ruta a la red interna de la empresa en el fichero de configuración del cliente OpenVPN?**

### Porque en verdad esta en otra red, aunque este conectado a una vpn de la empresa, si no hacemos esa ruta no vamos a llegar a la empresa, porque aun conectandonos, realmente no esta en la misma red

**Tal y como está configurada la red, es decir, simulando que la red del aula es Internet, ¿funcionaría la VPN si la red interna de la empresa fuera 192.168.3.0/24? Explica por qué tanto si la respuesta es que sí como si es que no.**

### Yo diria que no ya que esta solapando la misma red que tiene el aula, aunque en el aula sea /23 y la empresa /24, al final es casi lo mismo pero sin poder llegar a la 4.0