Las aplicaciones de red son la razon de ser de una red de computadoras


# Principios de aplicaciones de red
Como se desarrolla una aplicación de red?

La aplicación a desarrollar se debe ejecutar en distintos end systems y permitir que se comuniquen a traves de la red. Por ej: en la Web, se tienen dos programas distintos que se comunican entre si: el navegador ejecutandose en el host del usuario; y el servidor Web ejecutandose en host del servidor. Otro ejemplo: en una aplicación de transferencia de archivos P2P hay una aplicación en cada host que participa de la comunidad P2P. En este caso, las aplicaciones son muy parecidas entre si, o incluso son la misma aplicación.

Lo importante es que la aplicación se ejecuta en los end systems, no en los dispositivos del nucleo de la red, como routers y switches de capa de enlace. 
<<<incluso si quisieses, no podrias, ya que estos dispositivos funcionan en otro nivel de capa>>>

imagen_2_1

## Arquitecturas de aplicaciones de red

Es importante distinguir la arquitectura de la red, de la arquitectura de la aplicacion. Para desarrollar la aplicacion de red, es irrelevante la arquitectura de la red, solo importan los servicios que se proveen a las aplicaciones.

### Cliente Servidor
Siempre hay un host "always-on", llamado `servidor`. Este atiende pedidos realizados por hosts `clientes`.
Por ej: la Web.

Notar que los clientes no se comunican entre sí. Los navegadores no se comunican entre ellos.

El servidor tiene una direccion IP fija, bien conocida.

imagen_2_2_a

Ej de aplicaciones cliente-servidor: Web, FTP, Telnet, Email.

Raramente un host servidor puede atender todos los pedidos que hagan los clientes; por ello es que existen los `data centers`, donde se ejecuta un servidor virtual (en multiples hosts). 

### P2P

En esta arquitectura, hay poca (o ninguna) confiabilidad en servidores dedicados para atender pedidos. Por el contrario, se aprovecha la conexion entre hosts `peers`. Los `peers` no son propiedad de un proveedor de servicios, si no de usuarios comunes.

Se llama peer-to-peer porque la comunicacion no pasa a traves de un servidor dedicado.

imagen_2_2_b

Algunas aplicaciones son una mezcla de ambas arquitecturas.

Esta arquitectura es auto-escalable. Por ej en una aplicacion de compartido de archivos P2P, a pesar de que cada host genera una carga al pedir archivos, tambien agrega capacidad de servicio al distribuir archivos a otros hosts.
Debido a su estructura descentralizada, las aplicaciones P2P se ven afectadas por desafios de seguridad, performace, y confiabilidad (robustés?) en el servicio.

## Procesos comunicándose

## Servicios de transporte disponibles

## Servicios de transporte provistos por la Internet

## Protocolos de capa de aplicacion

## Aplicaciones que veremos

# Web y HTTP

## Vista general de HTTP

## Conexiones persistentes y no persistentes

## Mensaje HTTP

## Cookies

## Cacheo

# E-mail

## SMTP

## Comparacion con HTTP

## Mensaje SMTP

## Protocolos de acceso a e-mail

# DNS

## Servicios que provee

## Vista general

## Registros DNS y Mensajes

# Compartido de archivos P2P


# Streaming y CDNs


# Socket

## Programacion de socket con UDP

## Programacion de socket con TCP

# Resumen

