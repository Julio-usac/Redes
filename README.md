# **MANUAL DE CONFIGURACION**
## Topología 1
Pasos para configurar la topologia 1.
### Añadir maquina virtual de VMware:
- En GNS3 en la pestaña editar hay que seleccionar el boton preferencias, seleccionar la opcion VMware Y en la pestaña "Advance local settings" configurar cuantos vmnet interfaces se usaran.

<p align="center">
  <img src="imagen/Captura de pantalla (78).png" width="600">
</p>

- Crear la maquina virtual en VMware y configurar el network adapter para que utilice una de las interfaces vmnet previamente configuradas. 

<p align="center">
  <img src="imagen/Captura de pantalla (81).png" width="600">
</p>

- En GNS3 en la ventana de preferencias seleccionar la opcion VMware VMs y seleccionar nuevo, en la nueva ventana buscar la maquina virtual a utilizar y marcar la opcion "Use as linked base VM" para poder utilizar esa misma maquina varias veces.

<p align="center">
  <img src="imagen/Captura de pantalla (70).png" width="600">
</p>

- En la pestaña VMware VMs se podra ver la maquina virtual, seleccionar "type" el cual se encuentra en network y presionar editar, en la nueva ventana ir a la pestaña network y cambiar la opcion type a vmxnet3.

<p align="center">
  <img src="imagen/Captura de pantalla (69).png" width="600">
</p>

- Ahora podra usar la maquina virtual en su topologia.
 ### Diseñar la topologia
- Se utilizaran 3 vpcs, 3 maquinas virtuales, 4 switch y un cloud. 
- Se debe configurar el nombre de cada host.
- Unir cada host con su respectivo switch.

<p align="center">
  <img src="imagen/Captura de pantalla (66).png" width="600">
</p>

### Configurar host
- Encender la vpc, abrir la ventana de comandos, utilizar el comando "ip 'tu ip'/'tu gateway' 'tu puerta de enlace'".

<p align="center">
  <img src="imagen/Captura de pantalla (56).png" width="600">
</p>

- ingresar el comando save para guardar los cambios y repetir el proceso con todas las vpc.

<p align="center">
  <img src="imagen/Captura de pantalla (57).png" width="600">
</p>

- Encender la maquina virtual, ir a "conexiones de red", entrar en Local area conection, ir a propiedades, ir a protocolo de internet(TCP/IP) y modificar la ip.

<p align="center">
  <img src="imagen/Captura de pantalla (62).png" width="600">
</p>

<p align="center">
  <img src="imagen/Captura de pantalla (63).png" width="600">
</p>

- En este punto ya todos los hosts fueron configurados

### Configurar switch
- Hacer click en el switch, para configurar el puerto conectado a un host colocar el puerto a modificar en port, colocar la VLAN en VLAN y seleccionar aplicar.
- En la misma ventana, para configurar el puerto conectado a otro switch o cloud, colocar el puerto a modificar en port, en type seleccionar dot1q y seleccionar aplicar.

<p align="center">
  <img src="imagen/Captura de pantalla (71).png" width="600">
</p>

## Topología 2
