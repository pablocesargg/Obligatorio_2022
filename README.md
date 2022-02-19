# Obligatorio 
#
### Taller Instalacion Servidores Linux

## Parte A:

Para realizar el escenario que pide la letra vamos a necesita contar con un equipo bastión con ansible instalado.

Con el comando (sudo apt install ansible) se instalan los paquetes y dependencias requeridas para poder utilizarlo.
Se repite el mismo procedimiento para git (sudo apt install git).

Luego se crearon dos máquinas virtuales, una corriendo Ubuntu Server 20.04 y la otra con Rocky 8.5.

Ambos servidores cuentan con dos interfaces de red, una configurada como NAT 
(para navegación a internet) y la otra definida como red Sólo Anfitrión (para la comunicación con el equipo bastión), y fueron instalados con las siguientes características:

1 GB de Memoria RAM
25 GB de disco duro

Al momento de hacer la instalación de los Sistemas Operativos se creó el siguiente esquema de particionamiento:

Se Configuró la instalación con el siguiente esquema de particionamiento

Una partición de 1G para /boot
LVM: un volumen lógico de 5GB para /, 5GB para /var, 1GB para /home, 5GB /opt
y 2 GB de Swap.


#### Entrega Obligatorio 22/2
#### Defensa Obligatorio 23/2
##### Defensa en Lab 113 

