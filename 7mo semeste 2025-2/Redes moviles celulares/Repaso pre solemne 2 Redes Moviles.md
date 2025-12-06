RE - > expresion minima una subcarrier con un timeslot
RB - canal fisico con 12 subportadoras y 7 timeslots
2 RB -> PRB es lo que se entrega al aire
prefijo cíclico - padding para evitar ISI

OFDMA -> downlink
SC - OFDMA -> uplink

HARQ -> mecanismo desde 3G que se qued con algunos paquetes para repararlo

Eclo

RSRP -> recived signal recived power
RSRQ -> recived signal recived quality
RSSI -> recived signal  strengt indication

el celu siempre prefiere mejores tecnologias
#### Arquitectura
MME estacion base que controla varios EnodosB
HSS base de datos que concentra el VLR, HLR, AuC y EIR -> home suscriber center
	S-GW pasarela entre la red EPC y ETRAN basicamente entre ENodosB y el core de la red
P-GW router para dar salida a internet
PCRF modulo que aplica politicas de cobro y gestiona la calidad de servicio y filtro de paquete
el que se encarga de gestionar a nivel usuario qn tiene acceso a que cosa
![[Evolved Packet Core.png]]

S1 user plan S1 y S- GW para comunicacion
S1 control plane S1 y MME para control

X2 entre EnodosB para handover y gestion de recursos de radio

#### Protocolos en la interfaz de radio

**Packet Data Convergence Protocol (PDCP)** entrega y recibe paquete de IPentre los usuarios y el core de la red
**Radio Link Control (RLC)** envio de paquetes PDCP entre eNB y UE, usa ARQ
**Medium Access Control (MAC)** controla el acceso al canal de radio y multiplexa paquetes RLC, usa HARQ
Radio Resource Control(RRC) transporta el contro entre el EPC y el eNB

SCTP -> 4 way handshake y mensajes desordenados

S1 y X2 usan SCTP para transporte, para usuario utilizan GTP-U
#### Gestión de sesión
LTE da conexión a internet, red de ISP's, intranet o red del operador
estas redes tienen una etiqueta llamada APN (Acces Point Network)

hay un radio bearer para ver la calidad de servicio entre el celu y las redes externas y existen ciertos servicios que tienen prioridad y por ender garantias de calidad y otros son best effort.
Estos tienen QCI (QoS Class identifier)

#### Radio Bearers
**RRC** controla el comportamiento del UE cuando esta en modo **online**
y especifica la señal paging cuando esta en modo **idle**

hay 2 radio bearers 
DRB Data Radio Bearer -> palno usuario
SRB Signaling Radio Bearer -> plano control, mensajes RRC

DRB
2 tipos default bearer para solicitar los servicios de treafico
dedicated bearer para el trafico en si

agupados en  DTCH (Dedicated Traffic Channel)

hay un dedicated bearer por cada tipo de servicio  que se este ejecutando

SRB
SRB0 transmite mensajes RRC y se mapeal al CCCH (Common Control Channel)
SRB1 transmite mensajes NAS
SRB2 Transmite mensajes RRC de alta prioridad
Ambos de mapear al DCCH (Dedicated Control Channel)

#### Canales lógico

DTCH Dedicated Traffic Channel
	transmite info ente eNB y UE determinado
	existe en UL y DL
BCCH Broadcast Control Channel
	Lo utiliza el eNB para mandar info a los UE de su cobertura
	Existe en DL
PCCH Paging Control Channel
	Para ubicar en que eNB esta un determinado UE
	Existe en UL
CCCH Common Control Channel
	transmite informacion de control para establecer la conexión
	existe en DL y UL
DCCH Dedicated Control Channel
	canal punto a punto para transmitir información de control entre la red y el UE
	existe en UL y DL
#### Canales de Transporte
BCH Broadcast Channel
	canal asociado al BCCH
PCH Paging Channel
	Llama a los UE y los informa de actualizaciones
DL-SCH	Donwlink Shared Channel
	transporta trafico de usuario y señalización en el downlink
UL-SCH Uplink Shared Channel
	transporta trafico de usuario y señalización en el uplink
RACH Random Access Channel
	para peticiones de acceso al sistema
#### Canales fisicos downlink
PDSCH Physical Downlink Shared Channel
	transmite info de usuario
PBCH	Physical Broadcast Channel
	transmite en broadcast unos ciertos parámetros para el acceso de los UE a la celda
PDCCH Physical Downlink Control Channel
	transporta info de asignación de recursos de trafico de usuarios y recursos de canales de transporte
PHICH Physical HARQ Indicator Channel
	transporta los ACK y NACK para el funcionamiento del HARQ
PCFICH Physical Control Format Indicator
	informa al UE sobre el numero de simbolos utilizado en el PDCCH
PUSCH Physical Uplink Shared Channel
	Transmite info del usuario
PUCCH Physical Uplink Control Channel
	informacion de control del uplink, peticion de asignacion de recursos y mecanismo HARQ
PRACH Physical Random Access Channel
	gestiona el proceso de acceso aleatorio
#### scheduler LTE
scheduling de paquetes
	asigna subportadoras a cada usuario o cada proceso de usuario
	toma en cuenta:
	- requesitos de QoS
	- estado del canal
	- capacidad de transporte del eNB
Adaptación de enlace
	se adapta el enlace para que tenga modulaciones de mayor o menor nivel dependiendo de las condicones de SINR del enlace representado por el CQI Channel Quality Indicator
#### Voz en LTE
CSFB Circuit Switching FallBack
básicamente es bajar de tecnologia a 2G o 3G para hacer la llamada

VoLTE
básicamente mandar la voz como paquetes IP (VoIP) y como se esta haciendo sobre la interfaz de radio LTE se le llama VoLTE

OTT Over The Top
No usan sistemas dedicados para la voz si no que la mandan como cualquier otro paquete de datos por lo que esta sujeto a la conexion del canal y no da QoS

#### LTE Advanced
carrier agregation
	utilizar simultáneamente más de una banda de frecuencia para mejorar la velocidad
#### Dimensionamiento LTE RAN
calculo de cantidad de sitios para capacidad y cobertura deseada
Morfología
	Dense Urban
	Urban
	Suburban
	Rural
	High Speed Railway
Consideraciones
	BW de la portadora
	Uso MIMO
	Esquema de modulación
	bandas LTE
Se estiman todos los elementos del enlace que de ganancias o perdidas para obtener MAPL
con esto, un modelo de propagacion y una simulacion se puede obtener el cell radius

MODELOS DE PROPAGACIÓN EN LTE
![[Pasted image 20251206195124.png]]

POTENCIA POR SUBCARRIER EN UL
La máxima potencia que puede irradiar
un UE por estándar 3GPP es de 200mw (23 dBm).
GANANCIA ANTENA DE TRANSMISIÓN
TX CABLE LOSS
SENSIBILIDAD DE RECEPCIÓN
![[Pasted image 20251206195248.png]]
INTERFERENCE MARGIN
Considera la interferencia de las celdas vecinas. Este margen de interferencia en la
practica depende en gran medida de la capacidad planificada para la red

Generalmente se utiliza un valor como media de 3dB

SHADOW FADING MARGIN
El fading es un evento probabilístico el cual sigue una distribución normal, por ende la
desviación estándar del desvanecimiento muestra la distribución de la intensidad de la
señal de radio en diferentes puntos de prueba a distancias similares del transmisor

UMBRAL DE CORTE
El umbral de corte es el nivel de señal en el cual se cumplen las condiciones de
velocidad establecidas en el diseño de la red celular, para un usuario que se ubica en
el borde de la celda.