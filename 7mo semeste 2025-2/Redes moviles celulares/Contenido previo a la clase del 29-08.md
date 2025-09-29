Tópicos de redes móviles
- Cobertura
- Calidad
- Capacidad

##### Evolución de las redes móviles 
1G
Servicio únicamente de voz, conmutación de circuitos
-> 2G 
Servicios de voz mejorados y SMS
conmutación de circuitos para voz
inicio de envio de datos con la 2.5(GPRS) y 2.7(EDGE)
-> 3G 
conmutación de circuitos para voz, introduccion de paquetes ip para datos
-> 4G
Servicio de datos, VoIP, conmutación de paquetes ip

##### Estandares
2G -> GSM(Global System for Mobile comunications)
acceso al medio
FDMA
TDMA
2.5G ->GPRS (General Packet Radio Service)
2.7 -> EDGE (Enhanced Data for GSM Evolution)
3G -> UMTS (Universal Mobile Telecomunication Sistem)
WCDMA
3.5G -> HSPA (High Speed Packet Access)
3.99G -> HSPA+ (High Speed Packet Access+)
4G -> LTE y LTE+
OFDMA

### Elementos de una red movil:
- estacion base
- estaion de control de la estacion base
- estaciones moviles
- uplinks y downlinks
esto constituye una celda ya que da servicio a un sector determinado

esta estructura trae ventajas pero introduce un problema -> el handover

sectorzación: utilizar antenas direccionales dentro de una celda para aumentar conectividad, la suma de estas direccionalidades en su conjunto dan el efecto de cobertura 360°

Uplink y Donwlink:
enlace de subida y enlace de bajada (uplink peticiones de usuario downlink contenido que recibe el usuario) estas se manejan mediante la duplexión ya sea por tiempo(TDD) o por frecuencia (FDD) 2G y 3G TDD 4Gy 5G FDD ya que se usa mucho mas downlink que uplink por lo que no conviene establecer una comunicación permanente de este tipo

modo IDLE: sin trafico de red, solo mensajes de paging(acá estoy)

Modo conectado: traficando datos

### Identificaciones numericas

###### MSISDN(Mobile Station International Subscriber Directory Number)
básicamente un número de teléfono, consta de 
Country code(CC), 56
Nacional Destination Code(NDC) 9
Suscriber number(SN) 68285124


