
#              Obligatorio 
### Taller Instalacion Servidores Linux  


_Se puede encontrar toda la documentacion del trabajo obligatorio en la carpeta Doc_Obligatorio_

## Parte A:

Para realiza el escenario que pide la letra vamos a necesita contar con un equipo bastión con ansible instalado.
- Con el siguiente comando instalamos ansible: 
```bash
sudo apt install ansible
```
- Con el siguiente comndo instalamos git
```bash
sudo apt install git
```
Se crearon dos máquinas virtuales:
#Servidores
- Ubuntu Server 20.04 
- Rocky 8.5.

Ambos servidores cuentan con dos interfaces de red, una configurada como NAT 
(para navegación a internet) y la otra definida como red Sólo Anfitrión (para la comunicación con el equipo bastión), y fueron instalados con las siguientes características:

- 1 GB de Memoria RAM
- 25 GB de disco duro

Al momento de hacer la instalación de los Sistemas Operativos se creó el siguiente esquema de particionamiento:

Se Configuró la instalación con el siguiente esquema de particionamiento

Una partición de:
- 1G para /boot
LVM:
- 5GB para /
- 5GB para /var
- 1GB para /home
- 5GB /opt
- 2GB de Swap.
---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------
Ansible:
=======
~~~
Todos los volúmenes y particiones fueron generados en el asistente de instalación de los sistemas. 
Los volúmenes lógicos fueron creados con LVM y pertenecen a un mismo grupo de volúmenes (Volume
Group).
~~~
Se le dieron permisos para elevar privilegios (sudo) sin contraseña. Esto se logra
agregando la siguiente línea al final del archivo /etc/sudoers:
```bash
ansible ALL=(ALL) NOPASSWD:ALL
```
~~~
Una vez asegurada la conexión entre el bastión y los equipos a configurar, se copian las claves públicas
hacia cada uno de los servidores, para poder establecer la conexión vía SSH.
De esta forma, se podrá acceder vía SSH a los servidores sin necesidad de ingresar contraseña del
usuario ansible.
~~~

----------------------------------------------------------------------------------------------------
Playbooks:

Ejecutar main.yml para la instalacion del conjunto de paquetes requeridos
Editar vars.yml para agregar o quitar algun paquete de la lista de instalacion 


