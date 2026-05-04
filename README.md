# Introduccion
En este repositorio se explorara el diseño de un primer circuito con logica digital, desde la creacion de las tablas de verdad hsata la implementacion en una sistema de codificacion FPGA
# Mi primer diseño

<h3>Situacion problema</h3>
<!--Usted tiene un familiar que vive en el campo, tiene una finca y posibilidades de adaptar fuentes de energía para el consumo-->
<!--energético de su casa. En el lugar cuenta con la red eléctrica del comercializador de la zona rural y una excelente radiación-->
<!--solar. él sabe que usted está estudiando una ingeniería relacionada a la electricidad y le indica que está aburrido de los-->
<!--cortes de energía eléctrica en su zona. Usted por ocurrencia le sugiere tener un banco de baterías y un sistema fotovoltaíco para-->
<!--poder suplir de energía a su hogar cuando tenga fallos en la red eléctrica. A su familiar le suena la idea y como dicen coloquialmente-->
<!--¡lo embala!, llama a los demás familiares y empieza a expresar que usted se ha comprometido a desarrollar y diseñar-->
<!--ese sistema. usted por lo tanto siente que debe hacer lo mejor para que en Navidad sus familiares le feliciten porque está aplicando-->
<!--los conocimientos que ha estado desarrollando en su carrera.-->
<!---->
<!--Después de realizar las mediciones pertinentes de la carga eléctrica del hogar usted adquiere un sistema foltovoltáico, banco de baterías e iversores-->
<!--para acodicionar la red eléctrica de la casa y tiene los siguientes materiales:-->
<!---->
<!--* Un relé para conmutar la red del inversor y la red eléctrica del comercializador de la zona.-->
<!--* Un relé para energizar o desenergizar la red interna de la casa, en el caso de requerir realizar algún mantenimiento-->
<!--* Un sensor de medición de carga de la bateria, el cual sensa cuando la batería está cargada y cuando está descargada, tiene contactos tanto normalmente abiertos como normalmente cerrados.-->
<!--* Un sensor de luz que puede ser usado para detectar cuando hay radiación solar, tiene contactos tanto abiertos como cerrados-->
<!--* Un sensor detector de energía de red, el cual indica cuando hay electricidad en la red y cuando no la hay, tiene contactos abiertos y cerrados-->
<!--* Un tablero de mando en el cual usted puede poner diferentes indicadores, como pueden ser, paro de emergencia, batería descargada, detector de red electrica, casa energizada, etc.-->
<!--* Un botón de paro de emergencia o  demantenimiento, el cual, como fue mencionado, puede desenergizar su casa y para realizar otros mantenimientos.-->
<!---->
<!--El sistema que usted diseña minimo debe ser capaz de:-->
<!---->
<!--* Conmutar las fuentes de energía, ya sea de las baterías (el inversor) o de la red eléctrica.-->
<!--* Indicar cuando están las baterías descargadas-->
<!--* Indicar si se encuentra energizada la casa-->
<!--* Indicar si se detecta la red eléctrica de la casa-->
<!--* Indicar si hay suficiente radiación solar-->
<!--* Desde el tablero de mando poder detener el sistema desenergizado la casa.-->
<!---->
<!--Podrá realizar las combinaciones que usted crea convenientes, recuerde que ante su familia, usted es el que sabe, buena suerte!-->

Tienes un familiar que vive en el campo, en una finca, y tiene la posibilidad
de adaptar fuentes de energía para suplir el consumo eléctrico de su hogar. En
la zona donde vive, cuenta con la red eléctrica del comercializador local, pero
también dispone de una excelente radiación solar. Este familiar, sabiendo que
estás estudiando una ingeniería relacionada con la electricidad, te comenta que
está cansado de los constantes cortes de energía.

Con base en esto, se te ocurre sugerirle que implemente un sistema de energía
renovable que consta de un banco de baterías, el cual se recarga por energía
solar, así, garantizar el suministro de energía cuando haya fallos en la red
eléctrica. A tu familiar le entusiasma la idea (¡te embala, como se dice
coloquialmente!) y no tarda en contárselo al resto de la familia, expresando
que te has comprometido a diseñar y desarrollar dicho sistema. Ante esta
situación, decides tomar el reto en serio, pensando que sería genial recibir
felicitaciones de todos en Navidad por aplicar los conocimientos adquiridos en
tu carrera.

Después de realizar las mediciones pertinentes del consumo eléctrico de la
casa, adquieres un sistema fotovoltaico, un banco de baterías e inversores para
acondicionar la red eléctrica del hogar. Además, cuentas con los siguientes
materiales:

1. **Un relé o contactor** para conmutar entre la red del inversor y la red eléctrica del
   comercializador.
2. **Un relé o contactor** para energizar o desenergizar la red interna de la casa en caso de
   requerir mantenimiento.
3. **Un sensor de carga de batería**, que detecta cuando la batería está cargada o
   descargada; incluye contactos normalmente abiertos y cerrados.
4. **Un sensor de luz**, que detecta la radiación solar; incluye contactos
   normalmente abiertos y cerrados.
5. **Un sensor detector de red eléctrica**, que indica si hay o no suministro en la
   red eléctrica; incluye contactos abiertos y cerrados.
6. **Un tablero de mando**, donde puedes instalar diversos indicadores, como: paro
   de emergencia, batería descargada, detector de red eléctrica, casa
energizada, entre otros.
7. **Un botón de paro de emergencia o mantenimiento**, que permite desenergizar la
   casa para realizar intervenciones de forma segura.

El sistema que diseñes debe ser, como mínimo, capaz de:

1. Conmutar entre las fuentes de energía: el banco de baterías (inversor) y la
   red eléctrica.
2. Permitir detener el sistema y desenergizar la casa desde el tablero de
   mando.

Se sugiere que tengas en cuenta estas posibilidades en su comportamiento:

* Indicar cuando las baterías están descargadas.
* Indicar si la casa está energizada.
* Indicar si la red eléctrica está disponible.
* Indicar si hay suficiente radiación solar.

Puedes combinar los elementos disponibles de la manera que consideres más
adecuada para cumplir con los requisitos. Recuerda que, ante tu familia, tú
eres quien sabe. ¡Buena suerte!


<h3>1).Dominio copmartimental</h3>
<h4>Sistema de caja negra</h4>

<h4>Tabla de verdad</h4>
A continuacion se presenta la tabla de verdad
<img src="https://github.com/JOUNAL/Mi-primer-dise-o-Lab-2-de-digital-/blob/main/Imagenes/Tabla_verdad.png" width=50% height=50%>

<h4>Diagrama de flujo</h4>


<h3>2).Dominio fisico</h3>
<h4>Circuito electrico del sistema de control</h4>
A continuacion se plantea el circuito a ejecutar para el montaje logico
<img src="https://github.com/JOUNAL/Mi-primer-dise-o-Lab-2-de-digital-/blob/main/Imagenes/Diagrama%20de%20flujo%20SVD.png" width=50% height=50%>

<h3>3).Dominio estructural</h3>
<h4>Diagrama de compuertas logicas</h4>
Se muestra a continuacion el diagrama logico del circuito con compuertas logicas
<img src="https://github.com/JOUNAL/Mi-primer-dise-o-Lab-2-de-digital-/blob/main/Imagenes/CIrcuito_logico.png" width=50% height=50%>

<h3>4).Descripcion en lenguaje HDL</h3>
<h4>Codigo en verilog</h4>
A continuacion se expone el codigo obtenido por el programa de Digital en Verilog
```
   module Lab_2_Circuito_logico (
     input E1,
     input E2,
     input E3,
     input E4,
     input E5,
     output S1,
     output S2,
     output S3,
     output S4,
     output S5,
     output S6,
     output S7
   );
     wire s0;
     wire s8;
     wire s9;
     assign s0 = ~ E1;
     assign s8 = ~ E4;
     assign s9 = ~ E5;
     assign S1 = ((s0 & E3 & s8) | (s0 & E2));
     assign S2 = ((s0 & E2 & E3) | (E1 & s8) | (E2 & E3 & s9) | (E2 & s8) | (E3 & s8) | (s8 & s9));
     assign S6 = (E1 | E2 | E3 | s9);
     assign S7 = ((E1 & s8) | (E2 & s8 & E5) | (E3 & s8 & E5));
     assign S3 = E1;
     assign S4 = E3;
     assign S5 = E2;
   endmodule
```
```
Aquí va tu código
```
<h4>Puertos y nombre de modulo</h4>
<h4>Operadores logicos</h4>


<h3>5).Sintesis en FPGA</h3>
<h4>Codigo para la FPGA</h4>
<h4>Video de muestra</h4>
