# 🍯 Pottery

![](https://lh5.googleusercontent.com/WOnTIh4kzjRQlJJqxzR5TmYNi0L1AAKlUIk1zU4Gy8ZjJtRM5fJD2L9X\_z2vB7V7iUw3Y4sakDtxHX9l5-gw9dv8UwmEMnll6iqobkohlLO1on1PLWRsLm\_8ZJdbP2Lbm8PEfawS8HWxIlG2Wb-Rz4vDemag7oRU)

Pottery combina el Stake Bloqueado de CAKE con la lotería para darle la oportunidad de ganar un mayor rendimiento en su Stake de CAKE. Es fácil y seguro ya que siempre al menos recuperarás todo el CAKE que depositaste.

## Instrucciones:

* Deposita CAKE en la sección de POTTERY con un mínimo de 1 CAKE.&#x20;
* El depósito cierra el primer lunes de cada mes para cada serie de POTTERY diferente (23:59 UTC de ese lunes) y está abierto desde el viernes anterior alrededor de las 10:00 UTC, a menos que haya arreglos especiales que se anunciarán con anticipación (la primer Pottery cerrará el 8 de agosto de 2022 a las 23:59 UTC)&#x20;
* Durante la etapa beta del producto, hay un límite para el depósito total de CAKE para cada serie (el límite máximo de depósito es de 600 000 CAKE)&#x20;
* Los CAKE depositados se dirigirán al Pool de Stake bloqueado y se bloqueará durante diez (10) semanas. El 80% de las recompensas totales del Pool de Stake se enviarán al Pool de Pottery para el sorteo, el 20 % se reservará para su retiro.&#x20;
* Para cada serie de POTTERY (una por mes), habrá diez (10) sorteos en total, uno por semana, cada viernes (al mediodía UTC) al depositar, produciendo ocho (8) ganadores por semana. Cada wallet puede ganar más de uno de los ocho premios para ganadores. cada semana&#x20;
* Cuanto mayor sea su depósito en relación con el fondo general, mayor será la posibilidad de ganar, los ganadores pueden reclamar su premio a continuación de cada sorteo.&#x20;
* Cada serie de POTTERY tiene su sorteo por separado.&#x20;
* Solo después de 10 semanas a partir de la fecha de bloqueo de la serie de POTTERY, puedes retirar tus CAKE&#x20;
* POTTERY utiliza la implementación de VRF de Chainlink para una aleatoriedad verdadera y segura

## SERIES DE POTTERY (POTTERY COHORT)

El primer lunes de cada mes, se abrirá una serie de POTTERY para que deposites CAKE y participes en ella durante las próximas 10 semanas. Este arreglo combina el depósito para dirigirlo al Pool de Stake bloqueado, de modo que el contrato de la serie de Pottery pueda coordinar las recompensas de Stake del depósito del Stake bloqueado. Cada fecha de depósito y bloqueo será una serie separada, una para cada mes, por ejemplo: todos los depósitos del 5 de septiembre de 2022 estarán en una serie, todos los depósitos del 3 de octubre de 2022 estarán en otra serie. Si bien los sorteos pueden ocurrir simultáneamente para diferentes series , los premios acumulados para cada serie están separados para ser justos.

![(Solo con fines ilustrativos, la fecha de bloqueo de la serie real para la primera POTTERY se fijó para el 8 de agosto de 2022)](https://lh4.googleusercontent.com/8uGcM0vvN9g2O6YIQRotgIx24YhQxFQ4Q09orn0\_vmZvtkRErhoy0ly4daJu4B1tiqDWZA7xEa-miUXyVpxqBJ6CaCUeCfrGrQTrWDqrDO8shVBgACcfA62utARylSb-zJLoOFXox\_OoXZo6XT3Ez4brUQtnvutK)

Por ejemplo, hay 2 sorteos separados el 9 de septiembre de 2022, uno para la serie del 1 de agosto como el sexto sorteo semanal y otro para la serie del 5 de septiembre como el primer sorteo semanal. Si la serie del 1 de agosto tiene un total de 100 000 CAKE depositados y la serie del 5 de septiembre tiene un total de 300 000 CAKE depositados, el premio semanal para la serie del 1 de agosto solo provendrá de las recompensas de stake de esos 100 000 CAKE, mientras que el premio semanal de la serie del 5 de septiembre solo provendrá de las recompensas de participación de esos 300,000 CAKE. Si solo depositó CAKE en la serie del 1 de agosto, tiene la oportunidad de ganar el premio semanal el 9 de septiembre según las recompensas de apuesta de 100,000 CAKE. Si depositó CAKE tanto en la serie del 1 de agosto como en la del 5 de septiembre, tiene la oportunidad de ganar los dos premios semanales el 9 de septiembre.

## Financiación de premios y asignación de recompensas de stake

Los depósitos se agrupan en series mensuales para un arreglo más eficiente de las recompensas de Stake que también se agrupan para cada serie. Las recompensas de Stake se utilizan para financiar el premio acumulado y algunas recompensas de Stake por depositar en Pottery.&#x20;

El 80% de las recompensas de Stake se destinarán a financiar el fondo de premios de 10 sorteos semanales y el 20% restante se reservará como recompensas de Stake cuando retire su depósito de CAKE después de 10 semanas.&#x20;

Sin embargo, dado que las recompensas de Stake del Pool bloqueado de CAKE solo se distribuyen después de la duración del bloqueo, 10 semanas en este caso, para una mejor experiencia del producto y para facilitar los sorteos semanales inmediatamente después de la fecha de depósito, el contrato toma prestado el 80% de la Recompensas de Stake totales estimadas de la serie de la tesorería de CAKE en función del APY en el momento del bloqueo. El CAKE prestado se utiliza para el pago de cada sorteo semanal.&#x20;

Al final de las 10 semanas, cuando las recompensas del Syrup Pool se distribuyan, primero se reembolsará la tesorería de CAKE, luego el resto se devolverá a la bóveda para que los usuarios lo retiren junto con su depósito inicial en la serie.

![(Imagen solo con fines ilustrativos)](https://lh6.googleusercontent.com/NijUl8Qhz0iqXs3\_CYjRXVlRl4KtdemQPymzFNc-mO3bVCI8Ic-B1GVBc3WhqKElCku4eOzqpGsO974SxmrKz\_FsiRyEzV-GkOaA1TPSSP4wntHQNVeZERzGd0kwelGEIz3CW8LFoBw3hFMZBezU\_1gNDaXsrODV)

Por ejemplo, si la serie de Pottery el 1 de agosto de 2022 atrajo 100.000 depósitos de CAKE en total, el rendimiento estimado para 10 semanas de Stake bloqueado es de alrededor de 3674 CAKE. El contrato tomará prestado el 80%, o alrededor de 2940 CAKE, para el pozo de premios de 10 sorteos semanales, es decir, 294 CAKE en premios totales para cada sorteo semanal antes de las tarifas.&#x20;

Es importante tener en cuenta que las recompensas y el APY al final de la duración del depósito pueden cambiar durante la duración de 10 semanas en función de otros depósitos y sus períodos de bloqueo en el Pool de CAKE bloqueado. Puede haber una pequeña desviación de los porcentajes especificados (+/- 10%).&#x20;

Todas las recompensas de Stake netas de tarifas se devolverán a los depositantes a través de premios o recompensas. Si el APY real es más bajo que el APY estimado en el momento del bloqueo, significa que se distribuyen más recompensas a los depositantes durante los sorteos semanales y menos para la porción de recompensas de Stake. Si el APY real es más alto que el APY estimado en el momento del bloqueo, se distribuyen menos recompensas a través de los sorteos semanales y se reservan más para las recompensas de Stake disponibles para retiro. En última instancia, el valor resultante es el mismo.

## Cómo ganar: cálculo de probabilidades

Las probabilidades se calculan en función de la parte del monto del depósito en relación con el tamaño total del depósito de la serie. Simplemente, cuanto más CAKE hayas depositado, mayor será la posibilidad de ganar cada sorteo semanal. Por ejemplo, si has depositado 10.000 CAKE y el depósito total de la serie es 100.000 CAKE, hay un 10% de posibilidades de que ganes en cada sorteo semanal.&#x20;

Cada dirección puede ganar más de 1 de los 8 premios ganadores cada semana.&#x20;

En el caso extremo, si usted deposita todos los 100.000 CAKE de la serie, ganará todos los premios de cada sorteo semanal. Sin embargo, eso significa que el rendimiento final que obtendrá es el mismo que poner 100,000 CAKE en el Stake bloqueado durante 10 semanas, pero también pagará las tarifas de Pottery.

## Riesgos – ¡Importante!

Se le garantizará recuperar el 100% de lo que depositó en 10 semanas. Sin embargo, solo puede retirar su depósito de CAKE después de 10 semanas de bloqueo, sin ninguna otra forma de retiro anticipado.

&#x20;Al participar en Pottery, arriesgará las recompensas de Stake, junto con otras utilidades de CAKE bloqueadas como iCAKE y vCAKE. En caso de que no haya ganado nada de los 10 sorteos semanales, habría perdido el 80% de las recompensas de Stake que se suponía que obtendría si bloqueaba su CAKE en el Pool de Stake durante 10 semanas.&#x20;

Participe en función de su preferencia de riesgo. Una vez que se deposita CAKE, no hay nada que nadie pueda hacer para ayudarlo a retirar anticipadamente.

## FEES (Tarifas)

El ocho por ciento (8%) del premio acumulado que se distribuye cada semana se cobrará como tarifa de quema. Nuestro objetivo es revisar y ajustar la estructura de tarifas en consecuencia después de la etapa beta del producto.

## ¿Listo para participar?

Si tienes clara la estructura del producto, los riesgos y las tarifas, consulte esta página sobre cómo participar desde la interfaz de usuario web de PancakeSwap y otras preguntas frecuentes sobre Pottery.
