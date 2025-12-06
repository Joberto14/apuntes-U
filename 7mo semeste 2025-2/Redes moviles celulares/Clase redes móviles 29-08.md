weas de handover y weas en desorden

### Arquitectura de la red 2G
Acceso al medio: FDMA y TDMA

Modulacion: GMSK

Hard handover, se esta conectado a una estacion BTS y para hacer el cambio se desconecta de una y se conecta a la otra, hay un periodo de desconexion

a nivel de ususario esta la **Mobile Station(MS)** que se divide en 2
- dispositivo identificado con **(IMEI)**
- tarjeta **Suscriber Identity Module (SIM)**
estos dispositivos de usuario se conectan a la **Base Transceiver Station(BTS)** esta es responsable de la comunicación , maneja encriptacion, multiplexacion y modulacion, esta estacion puede tener varias antenas para el uso de diversidad espacial

Diversidad espacial -> info redundante por varias antenas
Multiplexación espacial -> varias antenas mandando mensajes distintos

estos BTS son controlados por los **Base Station Controller(BSC)**

Al corazón de la red GSM están los **Mobile Switching Center(MSC)** que realiza la conmutación de llamadas, es decir la conexión, entre 2 personas puede ir de la siguiente manera MS -> BTS -> BSC -> MSC -> BSC -> BTS -> MS conecta BSC's y se conecta con otros switches

Esta también  el **Gateway Mobile Switching Center (GMSC)** que se encarga de conmutar llamadas entre operadores distintos, se "conecta" a la **Public Switch Telephone Network (PSTN)**

***Adicionalmente estan las siguientes bases de datos***

la **Home Localtion Register(HLR)** es una base de datos que tiene información del cliente su IMSI, IMEI, planes,cuotas de trafico, restricciones. 

La **Equipment Identy Register (EIR)** que una base de datos que mantiene la lista negra, gris y blanca
 
Asi mismo esta la **Visitor Location Register (VLR)** que es un subconjunto de la HLR, tiene la misma info pero de clientes en una determinada area para disminuir el numero de consulta al la HLR

![[red 2g.png]]

2.5G 
GPRS General Packet Radio Service
servicio de envio de datos para reforzar el gsm

usa el concepto best effort, que es aquel que no ofrece garantías de QoS, depende de la condiciones como la carga de trafico actual y la capacidad de hardware de la red, básicamente intenta enviar el mensaje nomas

2.7G
Mejora de GPRS, usa 8PSK en lugar de GMSK(Gaussian Minimum Shift Keying)

2.5G, 2.7G, 3G
Agregan las siguientes unidades para el manejo de pquetes de datos dentro de la red

**Serving GPRS Support Node (SGSN)**: soporta GPRS y UMTS envia paquetes entre celulares(MS y UE) en su zona geográfica, manejo de movilidad, registro de datos de usuario para facturacion

**Gateway GPRS Support Node (GGSN)**: es basicamente el router a internet de la red, aplica politicas y reglas de la navegacion asi como parte de la facturacion

### Arquitectura 3G
UTMS (Universal Mobile Telecomunication System)

Acceso al medio: WCDMA (Wideband Code Division Multiple Access)

modulaciones: QPSK - 16QAM

Uplink y Downlink duplexados en frecuencia FDD

Soft handover, el UE conoce hasta 3 nodos y se hace handover cuando hay mal nivel de señal o mal nivel de calidad

El 3G usa el mismo core que 2G pero cambia el tramo de celus a estaciones

MS ahora es **UE (User Equipment)**
Los UE se conecta a los **Nodos B** homólogos a los BTS
A su vez los nodos B se conectan a los **Radio Network Controller (RNC)** homologo a BSC

![[Arquitectura red 3g.png]]

3,5G y 3,7G
R99 y HSPA
canal dedicado fijo garantiza QoS con asignación de factor de ensanchamiento

High Speed Packet Access (HSPA)
misma modulación QPSK y 16QAM
Usa una canal dedicado para datos de alta velocidad, flexible no garantiza QoS

Evolved High Speed Packet Access+ (HSPA)
usa 64QAM cuando la señal es muy buena

R99 para voz análoga y HSPA/HSPA+ para datos

# 4G
Estándar: Long Terminal Evolution(LTE)

Acceso al medio: Orthogonal Frequency Division Multiple Access(OFDMA) downlink
uplink Single-Carrier Frequency Division Multiple Access (SC-FDMA)

Modulaciones: 64QAM 256QAM

red completamente de datos(paquetes IP)

Uplink y Downlink capaz de utilizar TDD

#### Arquitectura 4G
ENb(Evolved Node B) basicamente antena y estacion de control 
NodoB + RNC

Mobility Managment Entity(MME) maneja locacion, autenticacion, cifrado y conexiones  SGW y PGW

Serving Gateway(SGW) sirve como gestionador del plano del usuario para mitigar los efectos de movilidad entre el UE y los diferentes ENb

PND Gateway(PGW) es el router de los datos de la red hacia el internet

Home Suscriber Server(HSS) la base de dats con toda la info(validacion SIM, HLR, VLR, EIR)

Policy and Charzging Rules Fuction(PCRF) traficador de la red que maneja el tarifado, QoS de los usuarios


