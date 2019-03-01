# examen-semana2

## Patrón de diseño

En primera instancia la solución sería utilizar una combinación de dos patrones de diseño, uno para verificar qué
clientes han pagado y otro para llevar a cabo el proceso de enviar la canción.

### Verificar pago
El patrón de diseño usado aquí debería ser *Observer* debido a que no se debería verificar a cada momento si algún 
cliente ha hecho su pago. 

### Decidir destinatario
En esta sección se debe utilizar *Chain of responsability*, debido a que se debe automatizar el envío de la compra al
destinatario correcto y con este patrón de diseño es posible evaluar de manera eficiente a quien se debe enviar y nos 
permite escalar la funcionalidad.

### Método de envío
Debido a que la funcionalidad es general a cualquier medio y destinatario, se debe escoger de forma dinámica la forma de hacer llegar
el pedido al destinatario, esto se logra con el patrón *Strategy* además de que nos permite implementar más opciones 
para el envío del pedido en un futuro.



La implementación debe funcionar de la siguiente manera:

![art code](https://github.com/Destroy-Youth/examen-semana2/blob/master/documentacion/ER%20diagram/funcionamiento.jpg)

