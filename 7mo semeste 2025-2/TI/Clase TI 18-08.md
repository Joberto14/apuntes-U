suma en log -> muliplicación

básicamente cuando hay una suma de dBm/W + dB se puede sumar de manera lineal

sin embargo si se cuenta con una suma de dBm/W + dBm/W es necesario pasar los términos logarítmicos a términos lineales, sumarlos y luego pasarlos a dBm/W de nuevo

ej:

$10mW + 1dB + 2dB$ 
$=> 10dBm + 1dB + 2dB = 13dBm$

$10dBm + 10dB$ 
$=> 10mW + 10mW = 20mW = 13dB$

$0dBW + 0dBm$
$=> 1W + 1mW = 1000mW + 1mW = 1001mW =30dBm \vee 0dBW$

## Espectro radio electrico
![[Espectro radio electrico.png]]
Es infinito

comunicaciones de infrarrojo: poca distancia y poca permeabilidad(pasr a travez de obstáculos)

$\Large \lambda = \frac{c}{f}$              $\large 3*10^8$
A mayor frecuencia -> mas perdidas, menor tamaño d antena mayor necesidad de LOS,mas tasa de transmisión, menos cobertura

La lluvia solo afecta a las bandas de similar longitud de onda(1mm Mm wave)

Las empresas quieren explotar el espectro para enviar más datos a ma frecuencia, menos longitud de onda meno cobertura

Embotellamiento de ultima milla anillo -> concentrador -> comuna -> Hogar -> ultima milla
![[ultima milla.excalidraw|350]]
