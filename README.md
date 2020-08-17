###### Universidad de San Carlos de Guatemala
###### Facultad de Ingeniería
###### Escuela de Ciencia y Sistemas
###### Redes de Computadoras 1
###### Nombre: Hayrton Omar Ixpatá Coloch
###### Carnet: 201313875

# Manual: Configuracion de Topología Practica 1
## 1. Topologia realizada
![Texto alternativo](/image/topologia_p1.png "Topologia")

## 2. Configuracion de Rauter c3725
  - Comandos utilizados
    - conf t
    - int f0/0  -> elegimos la interfaz a configurar
    - ip add {ip} {Mascara de subred}
    - no shut
    - exit
    - exit
    - sh ip int br -> Mostramos el estado de las interfaces
    
![Texto alternativo](/image/conf-rauter.png "Rauter")

## 3. Configuracion de VPC
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

## 4. Pruebas de comunicacione entre las VPC y la maquina Virtual linux
  - ##### Prueva desde maquina virtual
![Texto alternativo]( /image/ping-virtual-vpcs.png "ping tiny")
  - ##### Prueba desde VPC1
![Texto alternativo]( /image/ping-vpc1.png "ping vpc1")
 - ##### Prueba desde VPC2
![Texto alternativo]( /image/ping-vpc2.png "ping vpc2")
 - ##### Prueba desde VPC3
![Texto alternativo]( /image/ping-vpc1.png "ping vpc3")

## 5. Glosario
  - #### Direccion ip:
    Es un conjunto de numeros que nos permiten comunicarnos en la mayoria de nuestras redes, para ello se le asigna una direccion
    unica e irepetible a cada dispositivo al cual se le desa conectar a internet, este dispositivo puede ser un switch, rauter, pc, etc.
  - #### FastEthernet:
    es el nombre de una serie de estándares de IEEE de redes Ethernet de 100 Mbps, está basada en el estándar Ethernet por lo que 
    es compatible con cualquier red Ethernet, independientemente del tipo que sea, ya que los adaptadores de red (las tarjetas de red) 
    automáticamente ajustan su velocidad al adaptador más lento, de forma que todos los equipos puedan estar conectados
  - #### Gateway:
    es el dispositivo que actúa de interfaz de conexión entre aparatos o dispositivos, y también posibilita compartir recursos entre 
    dos o más ordenadores.
  - #### GNS3:
    es un simulador gráfico de red lanzado en 2008, que te permite diseñar topologías de red complejas y poner en marcha simulaciones 
    sobre ellos,  permitiendo la combinación de dispositivos tanto reales como virtuales.
  - #### Host:
    se referirse a las computadoras u otros dispositivos (tabletas, móviles, portátiles) conectados a una red que proveen y utilizan 
    servicios de ella, un host es todo equipo informático que posee una dirección IP y que se encuentra interconectado con uno o más 
    equipos y que funciona como el punto de inicio y final de las transferencias de datos.
  - #### Maquina Virtual:
    es un software que crea una capa independiente donde se emula el funcionamiento de un ordenador real con todos los componentes de 
    hardware que necesita para funcionar y que puede ejecutar cualquier sistema operativo o programa, tal y como lo haría un ordenador real.
  - #### Mascara de subred:
     Su función es indicar a los dispositivos qué parte de la dirección IP es el número de la red, incluyendo la subred, y qué parte 
     es la correspondiente al host.
   - #### Router:
     es un dispositivo que permite interconectar computadoras que funcionan en el marco de una red. Su función: se encarga de establecer 
     la ruta que destinará a cada paquete de datos dentro de una red informática.
   - #### Switch
    Un switch o conmutador es un dispositivo de interconexión utilizado para conectar equipos en red formando lo que se conoce como una 
    red de área local (LAN) y cuyas especificaciones técnicas siguen el estándar conocido como Ethernet (o técnicamente IEEE 802.3).
  - #### Topologia:
    el mapa físico o lógico de una red para intercambiar datos. En otras palabras, es la forma en que está diseñada la red, sea en el 
    plano físico o lógico.
