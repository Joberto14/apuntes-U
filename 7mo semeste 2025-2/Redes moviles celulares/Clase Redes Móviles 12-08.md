Diversidad de antena 
- Diversidad en frecuencia, una antena envia info en mas de una banda de frecuencia
- Diversidad espacial una antena hacia varios receptores
Existe:
- a) SIMO single input multiple output
- b) MISO multiple input single output
- c) MIMO multiple input multiple output
![[Boceto de tecnologia MIMO.excalidraw|330]]
- d) y SISO...
Arreglos de antenas
ejemplos: antenas de radio difusión(es po redundancia), Arreglos de antenas del ALMA
## Beamforming
ofrece construir el patron de radiación en base a la demanda
## Massive MIMO
combina el beamforming y la multiplexación espacial
## Zonas de Frenell
 punto mas eficiente entre 2 antenas, debe estar libre
 ![[zonas de fresnell.png|450]]
 ![[modelo zonas de fresnell.png|500]]
 $\huge r =17,32 \sqrt\frac{d1*d2}{d*f}$ 
 calculo del radio de la primera zona de fresnell, la obstruccion maxima permisible es de 40% pero se recomienda un 20% o menos

#### Perdida en el espacio libre (Loss in Free Space LSF)
![[diagrama perda de espacio libre.png]]

$LFS = 92,45 + 20 log(D) + 20log(f)$ 
f -> GHz
D -> Km
## Modelos de propagación

ecuaciones que pretenden modelar las perdidas por obstáculos, geografías y en general todo lo que obstruya la radiocomunicación 
#### Terrestrial path with one terminal in woodland
![[terrestrial path with one terminal in woodland model.png]]
 Woodland = bosque
 $\huge A_{ev}=A_m[1-e^{\frac{d*\gamma}{A_m}}][dB]$ 
 $\gamma$ es la atenuación especifica para vegetación de baja altura  
 $A_m$ es la máxima atenuación de un terminal para un tipo de vegetación en especifico
 
 Debe ser sumado con ademas la perdida de espacio libre
### ITU terrain model
### Modelo Hata
### Cost 231: (Hata model PCS extension)

#### Redes móviles
Problemas: atenuación por shadowing, multitrayectos, Doppler, mantener conexión estable estable, cobertura, mantener costo eficiencia

handover, handoff

objetivos -> permitir movilidad, servicio continuo, servicio aceptable

