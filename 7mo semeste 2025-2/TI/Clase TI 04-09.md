## Nivel MAC

red Ad-hoc o BSS(Basic service set)

Servicio básico, las tramas se transmiten de emisor a receptor y los host estan conectado entre si para hacer la comunicación, sin un ap, ej: audifonos bluethoot, limitado por cobertura y potencia del dispositivo
![[Red Ad-hoc.png]]

[[CSMA-CA]]

**Colisiones**
Posibles pero se intenta minimizar, en CSMA/CA cuando no se recibe un ack los transmisores esperan un tiempo aleatorio que aumenta exponencialmente hasta que ocurra la transmisión exitosa

**Fragmentación** 
otra solución a para asegurar el envio y recepcion de mensajes es la fragmentacion, que consiste en dividir tramas grandes en tramas mas pequeñas lo que entre otras cosa permite establecer una comunicación eficiente en entornos con mucho ruido, el problema de esta tecnica es que aumenta el overhead de los paquetes, es decir, se manda mas metadata

**Problema de la estación oculta**
![[Estación oculta.png]]

Colisión de A y C en B pues A y C creen que el medio esta libre

solución -> info en la trama (overhead)
A -> RTS(request to send), C -> (espera broadcast)
B -> CTS(Clear to Send)

**Red con AP**
![[Topología red con AP.png]]
**Topología Extended Service Set**
básicamente el mismo sistema de la U, mismo nombre de red pero son distintos AP's
![[Topología Extended Service SET.png]]

**Red con AP cableado y repetidor**
![[AP cableado y repetidor.png]]
**Handover**
Ej: dentro de la U 