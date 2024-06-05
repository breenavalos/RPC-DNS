# RPC-DNS

Este proyecto implementa un sistema básico de resolución de nombres de dominio utilizando RPC (Remote Procedure Call). Consiste en un cliente que envía un nombre de dominio a un servidor, el cual resuelve el nombre de dominio y devuelve las direcciones IP asociadas.

## Descripción

El proyecto se compone de dos partes principales:
1. **Cliente RPC (`IPS_CLIENT`)**
2. **Servidor RPC (`iPC_SERVIDOR`)**

### Cliente RPC (`IPS_CLIENT`)

El cliente envía una solicitud al servidor con el nombre de dominio que desea resolver. La función principal del cliente es `ips_programa_1`, la cual realiza lo siguiente:
- Crea un cliente RPC y establece la conexión con el servidor.
- Envía el nombre de dominio al servidor.
- Recibe y muestra las direcciones IP resueltas.

### Servidor RPC (`iPC_SERVIDOR`)

El servidor recibe la solicitud del cliente, resuelve el nombre de dominio utilizando `gethostbyname`, y devuelve las direcciones IP asociadas al cliente. La función principal del servidor es `ips_1_svc`, que realiza lo siguiente:
- Recibe el nombre de dominio del cliente.
- Llama a `funcionip` para resolver el dominio.
- Devuelve las direcciones IP resueltas al cliente.

## Relación con el DNS

Este proyecto representa una forma simplificada del funcionamiento del DNS (Sistema de Nombres de Dominio), que traduce nombres de dominio en direcciones IP. 
