### Nivelación
Definiciones:

- medio físico:
	vías por las cuales se transporta la información como lo puede ser el aire, un cable(cables coaxiales, cables de par trenzado) o un circuito eléctrico(PCB)
- medio confinado:
	medio donde se propaga la info sin salir de este, dependiendo del caso puede ser afectado por los campos electromagnéticos que se propagan desde otras vías, como se menciono anteriormente estos son medios como los cables, la fibra optica y los circuitos eléctricos
- Espectro:
	Se refiere a espectro electromagnético que no es mas que el rango total de frecuencias de la radiación electromagnética, de esto destacar el subconjunto del espectro radioeléctrico que constituyes a las longitudes de onda de entre 3kHz y 300GHz. Importante: en el caso de Chile el espectro radioeléctrico es un bien nacional de uso publico, es decir ,que le pertenece a todos los chilenos y es regulado por la [Subtel](https://www.subtel.gob.cl/)
- Multiplexación: 
	Es el envío de multiples flujos de información en 1 o mas vías de comunicación, existen varios tipo de multiplexación tales como:
	- Multiplexación en frecuencia: consiste en subdividir las bandas de frecuencia para poder enviar varios flujos de información a la vez a través de un mismo medio, es común ver esto en la radio o television donde el consumidor debe sintonizar un canal(frecuencia) para recibir la estación o canal de television a su vez el proveedor puede enviar una señal broadcast con la información ya sea que una estación de radio pueda emitir su frecuencia al aire y esta no interferirá con otra estación pues están en bandas de frecuencia distintas
	![[Multiplexación en frecuencia.png|300]]
	- Multiplexación espacial: en el caso particular de la comunicacion inalambrica la multiplexación espacial se logra con el uso de varias antenas para enviar mensajes, normalmente manifestado en la tecnologia MIMO(multiple input multiple output) que a grandes rasgos hace que el fujo de informacion se separe -> sea transmitido por varias antenas -> y luego reconstruido por haber sido captado por varias antenas receptoras esta tecnología tiene hartas ventajas para mejorar la QoL y no voy a seguir detallando mucho aca aun.
		![[Boceto de tecnologia MIMO.excalidraw|350]]
	- Multiplexación temporal: básicamente consiste en subdividir la información en ventanas de tiempo, es util ya que dependiendo del caso de uso, si las ventanas de tiempo son suficientemente rápidas resulta imperceptible que el canal de information esta sirviendo varios flujos de información, así mismo es un sistema legacy en su mayor parte utilizado en telefonía clásica pero también el Bluetooth!
- dB: 
	decibelios representación logarítmica de relación entre input y output	![[Caja negra decibeles]]
	en este caso la caja negra amplifica el input 2 veces $O/I = 2mW/1mW = 2$ $veces$
					            $\Large 10 * log(\frac{output}{input}) = XdB$
	**dBm** -> relación de potencias respecto a un mili Watt
	**dBW** -> relación de potencias respecto a un Watt
- SNR  
	Relación señal a ruido (Signal to noise ratio)
	Según Venegas el ruido es cualquier señal no deseada
	Según Carreño es la contaminación de señales y un una baseline en toda comunicacion
	Según Wikipedia el ruido es  un error operturbacion aleatoria no deseada de una señal de información util en un canal de telecomunicación. El ruido es la suma de de perturbaciones y energia no deseada ya sea de funtes de la naturaleza
	
	A menor SNR nivel de SNR no se logra una comunicacion eficiente 
	
	Diferencia  de potencia de señal captada y potencia del ruido 
- SNIR
	Diferencia de niveles de potencia a la señal a la señal deseada vs las otras señales que se están enviando en la misma banda de frecuencia
- Ancho de banda(bandiwidth)
	Rang de frecuencia de utilización
- Eficiencia espectral ($\eta$)
	$\Large \log_2(1 + SNR)$ $\Huge [\frac{Bps}{Hz}]$ $\Huge \frac{E_o}{N_o} = SNR$
	![[Eficiencia espectral.excalidraw|300]]
	capacidad de transmisión en un hertz sistema
	$\eta * BW$ -> capacidad maxima de eficiencia espectral teórica del sistema
	