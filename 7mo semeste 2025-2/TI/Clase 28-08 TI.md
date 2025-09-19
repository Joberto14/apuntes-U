## Redes inalambricas

![[cuadro resumen de redes inalambricas.png]]

## Tecnicas WWAN
**OFMA**
Se utiliza para conseguir que un conjunto de usuarios de un sistema de telecomunicaciones puedan compartir el espectro de un cierto canal. El acceso múltiple se consigue dividiendo el canal en un conjunto de subportadoras que se reparten en grupos en función de la necesidad de cada uno de los usuarios.

![[OFDMA.png]]
**Masive MIMO:** muchas antenas de input y output
![[Boceto de tecnologia MIMO.excalidraw]]
**beamforming**:
![[Beamforming.png]]

## Tenicas WLAN
**MU-MIMO:** router que se conecta a la vez con todos los dispositivos de los usuarios
![[MU-MIMO.png]]

[[FHSS]] 
[[DSSS]]
[[OFDM]]

Roaming: uso de redes prestadas aparte del contrato con la empresa de telefonía proveedora

*Preguntable: técnicas de radio, roaming*

Velocidad de WPAN limitado por la potencia de las antenas

## Modelo de Fris
Asume que el unico camino entre receptor y transmison es la LOS, no hay obstaculos, no hay multitrayecto, no hay rebotes y las antenas son omnidireccionales

![[modelo de Fris]]

$\huge P_r =P_t*G_t*G_r*(\frac{ \lambda }{4*\pi*d})^2$
$(\frac{ \lambda }{4*\pi*d})^2$ -> path loss que depende de la frecuencia de la onda
el elevado se le llama exponente de perdidas y cuando es igual a 2 es que se llama modelo de Fris

Puede ser usado de modelo de referencia

*Ganancia:* intrínseco de la antena, las antenas mas simples son omnidireccionales

![[Historia WLAN.png]]
![[historia WLAN p2.png]]
