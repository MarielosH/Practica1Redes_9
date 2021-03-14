# Manual de construcción y configuración
#### Integrantes grupo 9 
- 201503470 Yimmi Daniel Ruano Pernillo
- 201314852 Diego René Molina Roldán
- 201504399 María de Los Angeles Herrera Sumalé
- 201504254 Wendy Aracely Chamalé Boch

## Topología 1 
La topología 1 cuenta con 6 host, 3 de ellas con máquinas virtuales con sistema operativo .......  y las otras 3 son VPC

### Configuración de la topología 1

#### Configuración de los Switch 
- Switch 4, Ventas: En este switch se configuró la vlan 29, para el acceso de la vpc y la máquina virtual, ambas de tipo access, en los puertos 1 y 2 respectivamente,  así como la conexión con otro switch en el puerto 0 de tipo dot1q.
![Screenshot_227](https://user-images.githubusercontent.com/70044543/111055581-dddbb600-843c-11eb-911e-0ae03f795828.png)
- Switch 3, Informática: En este switch se configuró la vlan 19, para el acceso de la vpc y la máquina virtual, ambas de tipo access, en los puertos 1 y 2 respectivamente,  así como la conexión con otro switch en el puerto 0 de tipo dot1q.
![Screenshot_228](https://user-images.githubusercontent.com/70044543/111055653-dd8fea80-843d-11eb-9917-126ba910e1e7.png)
- Switch 1, Contabilidad: En este switch se configuró la vlan 39, para el acceso de la vpc y la máquina virtual, ambas de tipo access, en los puertos 2 y 3 respectivamente,  así como las conexiones para los otros switch en el puerto 0 y 1 de tipo dot1q.
![Screenshot_229](https://user-images.githubusercontent.com/70044543/111055668-0c0dc580-843e-11eb-8d39-73f5155ff5ec.png)
- Switch 2: Este switch es el que se conecta a la nube, así como las conexiones para los otros switch en el puerto 0 y 1 de tipo dot1q.
![Screenshot_230](https://user-images.githubusercontent.com/70044543/111055702-6149d700-843e-11eb-8d66-e92f7036b884.png)

#### Cofiguración de las VPC

