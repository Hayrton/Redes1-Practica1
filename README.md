###### Universidad de San Carlos de Guatemala
###### Facultad de Ingeniería
###### Escuela de Ciencia y Sistemas
###### Redes de Computadoras 1
###### Nombre: Hayrton Omar Ixpatá Coloch
###### Carnet: 201313875

# Manual: Configuracion de Topología Practica 1
1. ## Topologia realizada
![Texto alternativo](/image/topologia_p1.png "Topologia")

2. ## Configuracion de Rauter c3725
  - Comandos utilizados
    - conf t
    - int f0/0  -> elegimos la interfaz a configurar
    - ip add {ip} {Mascara de subred}
    - no shut
    - exit
    - exit
    - sh ip int br -> Mostramos el estado de las interfaces
    
![Texto alternativo](/image/conf-rauter.png "Rauter")

3. ## Configuracion de VPC
  - Comandos utilizados
    - ip {ip} {Mascara de subred} gateway {ip de interfaz}
    - sh ip -> Muestra la configuracion de red de la vpc
  - #### VPC1
  
![Texto alternativo]( /image/conf-vpc1.png "Vcp1")
  - #### VPC2
![Texto alternativo]( /image/conf-vpc2.png "Vpc2")
  - #### VPC3
![Texto alternativo]( /image/conf-vpc3.png "Vpc3")
  
  - #### Configuracion de maquina virtual linux
    - Distribuicion de linux utilizada [Tiny core](http://tinycorelinux.net)
    
![Texto alternativo]( /image/conf-linuxv.png "Tiny core")

4. ## Pruebas de comunicacione entre las VPC y la maquina Virtual linux
  - ##### Prueva desde maquina virtual
![Texto alternativo]( /image/ping-virtual-vpcs.png "ping tiny")
  - ##### Prueba desde VPC1
![Texto alternativo]( /image/ping-vpc1.png "ping vpc1")
 - ##### Prueba desde VPC2
![Texto alternativo]( /image/ping-vpc2.png "ping vpc2")
 - ##### Prueba desde VPC3
![Texto alternativo]( /image/ping-vpc1.png "ping vpc3")
