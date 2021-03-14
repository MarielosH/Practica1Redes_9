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
- Switch 4, Ventas: En este switch se configuró la vlan 29, para el acceso de la vpcs y la máquina virtual, ambas de tipo access, en los puertos 1 y 2 respectivamente,  así como la conexión con otro switch en el puerto 0 de tipo dot1q.
![Screenshot_227](https://user-images.githubusercontent.com/70044543/111055581-dddbb600-843c-11eb-911e-0ae03f795828.png)
- Switch 3, Informática: En este switch se configuró la vlan 19, para el acceso de la vpcs y la máquina virtual, ambas de tipo access, en los puertos 1 y 2 respectivamente,  así como la conexión con otro switch en el puerto 0 de tipo dot1q.
![Screenshot_228](https://user-images.githubusercontent.com/70044543/111055653-dd8fea80-843d-11eb-9917-126ba910e1e7.png)
- Switch 1, Contabilidad: En este switch se configuró la vlan 39, para el acceso de la vpcs y la máquina virtual, ambas de tipo access, en los puertos 2 y 3 respectivamente,  así como las conexiones para los otros switch en el puerto 0 y 1 de tipo dot1q.
![Screenshot_229](https://user-images.githubusercontent.com/70044543/111055668-0c0dc580-843e-11eb-8d39-73f5155ff5ec.png)
- Switch 2: Este switch es el que se conecta a la nube, así como las conexiones para los otros switch en el puerto 0 y 1 de tipo dot1q.
![Screenshot_230](https://user-images.githubusercontent.com/70044543/111055702-6149d700-843e-11eb-8d66-e92f7036b884.png)

#### Cofiguración de las VPCS
- Host:Informatica2, En esta VPCS se le asigno la siguiente dirección ip:192.168.19.30 mask:24, se conecto al switch 3.
![Screenshot_202](https://user-images.githubusercontent.com/58566059/111056712-e0430d80-8446-11eb-992a-79dcb2d72df7.png)

- Host:Ventas2, En esta VPCS se le asigno la siguiente dirección ip: 192.168.29.30 mask:24, se conecto al switch 4.
![Screenshot_200](https://user-images.githubusercontent.com/58566059/111056457-8d685680-8444-11eb-865b-fe4626492c74.png)
- Host:Contabilidad1, En esta VPCS se le asigno la siguiente dirección ip: 192.168.39.30 mask:24, se conecto al switch 1.
![Screenshot_203](https://user-images.githubusercontent.com/58566059/111056657-6448c580-8446-11eb-9359-3773fb11552d.png)


-Al finalizar la configuracion de las se verificaron estas configuraciones realizando ping sobre estas.
![Screenshot_204](https://user-images.githubusercontent.com/58566059/111056754-37e17900-8447-11eb-99c3-5f1bfac04445.png)
![Screenshot_205](https://user-images.githubusercontent.com/58566059/111056764-50519380-8447-11eb-9283-581fa7f1537f.png)
![Screenshot_206](https://user-images.githubusercontent.com/58566059/111056766-55164780-8447-11eb-88f9-706fa81b78ca.png)
![Screenshot_207](https://user-images.githubusercontent.com/58566059/111056768-58113800-8447-11eb-90d3-f4261a71251c.png)
![Screenshot_208](https://user-images.githubusercontent.com/58566059/111056769-5a739200-8447-11eb-850c-f2044784aa1a.png)


