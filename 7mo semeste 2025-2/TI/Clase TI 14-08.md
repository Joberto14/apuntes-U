continuación de la ppt 0, conceptos basicos

- modulación:
	Alterar algun parametro de una señal auxiliar en funcion de una señal de información
	Modulaciones AM, FM, PM:
	![[modulacion AM, FM y PM.png|550]]
	Modulaciones complejas: BPSK QPSK, QAM...4QAM...64QAM
	
	A mayor complejidad de modulation más probabilidad de errores
	Es necesario contar con un mayor SNR para poder usar modulaciones mas complejas 
	Cuando un buen nivel de SNR no es garantía se deben usar modulaciones mas simples
	
	los sistemas modernos son inteligentes y aceptan varias modulaciones para afrontar la variabilidad en la SNR
	
	se mapea a través de símbolos enviados, baudios
- Ecualización: Ajuste en determinadas frecuencias de una señal generando atenuaciones u amplificaciones
- Paquete: conjunto de información enviada en un medio
- Trama: Conjunto de paquetes
- Tipos de mensaje:
	Boradcast presente en cosas como la radio y la TV
	Multicast ejemplos como IPTV, IGMP(Internet Group management protocol)
	Unicast presente en las búsquedas por internet y la descaga de archivos
- Estrategias de duplexión: 
	Full duplex: en el mismo canal se recibe y se envía en simultaneo como: en la telefonía
	half duplex: se puede decidir entre recibir o se enviar nunca ambos como: en los walkie-takies
	simplex: solo se envia o solo se recibe, único propósito como: en las radios(el dispositivo) ya que este solo capta las señales para su reproducción
- Mecanismos de acceso al medio: Organización pa que puedan hacer uso del canal los usuarios
	esto se logra ya sea con estrategia basadas en tiempo, en frecuencia y en código
	existen mecanismos (CSMA)
	con contienda:que pueden existir colisiones, timeout y mecanismo de reenvió
	sin contienda: donde los usuarios son organizados(Aloha, slotted Aloha)
- Mecanismos ARQ (automated Repeat request) es un mecanismo simple sobre las primeras 2 capas que hace que el receptor envié un acknowledge al transmisor antes de un timeout para de esta manera tener una transmisión confiable sobre un canal no confiable	 
- Quality of service (QoS) engloba varias metricas de red para asegurar una comunicacion de buena calidad, cosas como la cobertura, baja perdida de paquetes, bajo retraso(tiempo entre que se envia el paquete y su receptor) y bajo jitter(flujo irregular de paquetes) etc
## EJERCICIOS

0db + 0db es igual!!! a 0db
hay que pensar que dado que los decibeles estan en escala logaritmica la suma es una multiplicacion de sus argumentos por los que $0 * 0 = 0$ 
