# **MANUAL DE CONFIGURACION**
## Topología 1
Pasos para configurar la topologia 1.
### Añadir maquina virtual de VMware:
- En GNS3 en la pestaña editar hay que seleccionar el boton preferencias, seleccionar la opcion VMware Y en la pestaña "Advance local settings" configurar cuantos vmnet interfaces se usaran.
- Crear la maquina virtual en VMware y configurar el network adapter para que utilice una de las interfaces vmnet previamente configuradas. 
- En GNS3 en la ventana de preferencias seleccionar la opcion VMware VMs y seleccionar nuevo, en la nueva ventana buscar la maquina virtual a utilizar y marcar la opcion "Use as linked base VM" para poder utilizar esa misma maquina varias veces.
- En la pestaña VMware VMs se podra ver la maquina virtual, seleccionar "type" el cual se encuentra en network y presionar editar, en la nueva ventana ir a la pestaña network y cambiar la opcion type a vmxnet3.
- Ahora podra usar la maquina virtual en su topologia.
 ### Diseñar la topologia
 - Se utilizaran 3 vpcs, 3 maquinas virtuales, 4 switch y un cloud. 
 - Se debe configurar el nombre de cada host.
 - Unir cada host con su respectivo switch.
### configurar host
-


## Topología 2
