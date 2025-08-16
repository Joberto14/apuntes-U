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
	![[Pasted image 20250815221934.png|300]]
	- Multiplexación espacial: en el caso particular de la comunicacion inalambrica la multiplexación espacial se logra con el uso de varias antenas para enviar mensajes, normalmente manifestado en la tecnologia MIMO(multiple input multiple output) que a grandes rasgos hace que el fujo de informacion se separe -> sea transmitido por varias antenas -> y luego reconstruido por haber sido captado por varias antenas receptoras esta tecnología tiene hartas ventajas para mejorar la QoL y no voy a seguir detallando mucho aca aun
	- Multiplexación temporal: basicamente consiste en subdividir la informacion en ventanas de tiempo, es util ya que dependiend del caso de uso, si las ventanas de tiempo son suficientemente rapidas reulta imperceptible que el canal de informacion esta sirviendo varios flujos de informacion, asi mismo es un sistema legacy en su mayor parte utilizado en telefonía clásica pero también el bluethoot!