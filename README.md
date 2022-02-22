#              Obligatorio 
### Taller Instalacion Servidores Linux

* Se puede encontrar toda la documentacion del trabajo obligatorio en la carpeta Doc_Obligatorio*

##Parte A:
Para realizar el escenario que pide la letra vamos a necesita contar con un equipo bastión con ansible instalado.
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



#### Entrega Obligatorio 22/2
#### Defensa Obligatorio 23/2
##### Defensa en Lab 113
##Prueba 

Hasta las 21:00Hs del martes 22

=======
# Obligatorio_2022

