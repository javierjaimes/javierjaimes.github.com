---
layout: post
title: "Hello LoRa!"
description: ""
category: 
tags: []
---
{% include JB/setup %}

Desde hace un tiempo he venido aprendiendo cosas nuevas y muchas de esas estan asociadas a lo que creo tendran un auge en el 2020 o menos, y son aquellas relacionadas con el *IoT*.

Unos meses atras conocí el concepto de LPWAN (Low Power Wide Area Networks) y al investigar un poco mas sobre el tema y cual era su rol en el mundo del internet de las cosas supuse que iba a ser interesante y decidi conocer un poco mas y esto es a lo que he llegado.

Antes de hablar de LPWAN quiero a manera de ejercicio hablar un poco de dos cosas RF y WIRELESSS. Ambas han estado con nosotros desde hace mas de un siglo, y su primer experimento fue dado por Guglielmo Marconi cuando a principios del siglo 20 decidio trasmitir codigo Morsa desde Comwall, Inglaterra hasta St Jhon's en Canada.

Por RF que tecnicamente viene a ser un sinonimo de Wireless nos referimos a ciertas ondas electromagneticas que existen entre los 3 Khz hasta 300 GHz, las cuales la mayoria de estas ondas en este espectro son usadas para comunicaciones o señales de radar.

Pero que es LoRa&copy;? bueno, basicamente es un formato de modulacion de señales electricas. Es propietario y fue creado por Cycleo una compañia que luego fue adquirida por Semtech&trade;, a pesar de ser cerrado el formato si tienes algo de dinero podrias adquirir una licencia, cosa que ya hecho Semtech con algunos otros fabricantes de semiconductores.

Para mas informacion sobre el formato de modulacion de LoRa&copy; [click aqui](https://www.link-labs.com/what-is-lora).

Ahora hablemos de las cosas, si de las cosas que necesitan ser conectadas a internet, y con esto me refiero por ejemplo a medidores de agua, energia y gas, tambien podria mencionar pequeños sensores de temperatura, todos ellos tienen algo en comun y es que sus requerimientos en temas de networking son limitados comparados a lo que necesita un smart phone, una tablet o un computador. y es aqui en donde vienen las LPWAN a salvarnos, y en esta ocasion hablaremos de LoRaWAN&trade;.

Que es LoRaWAN&trade; basicamente un protocolo de red, definido y mantenido por la LoRa Alliance&trade;.

De entre algunos beneficios tenemos:

* Usa espectros gratuitos (868 MHz en Europa y 915 MHz en USA).
* Rango: algunos pocos kilometros en areas densas urbanas y hasta 15-30 kilometros en areas rurales.
* Bateria: hasta mas de 10 años de vida.
* Costos: $2USD para un dispositivo y hasta $1USD por subscripcion a una red LoRaWAN&trade;.

Hablando un poco de la Arquitectura de una red LoRaWAN&trade; puedo mencionar cuatro grandes elementos:

* El mote/end-point-device: basicamente es tu cosa en si, es decir el sensor que mide la cantidad de ruido generado en un punto especifico de tu ciudad.
* El gateway/concentrator: quien esta a cargo de recibir los datos de los motes y enviarlos a algo que se llama el Network Server.
* El Network Server: quien esta ahi para recibir todos los datos y enrutarlos al Application Server adecuado con el fin de ser manipulados ó visualizados.
* El Application Server y Consumer Service: El uno sirve para administrar tus motes conectados a tu red y el otro quizas puede ser el elemento final a donde tus datos van a llegar y seran representados.


Para ser honestos LoRaWAN&trade; no es la unica opcion en lo que a LPWAN se refiere de hecho hay opciones para donde escoger como por ejemplo SigFox, NB-IoT ó LTE-Advanced Pro.

Pero a su favor podemos decir que varias ciudades del mundo hoy lo apuestan a LoRaWAN&trade; como una solucion muy viable a la hora de generar redes publicas que aporten al desarrollo de ciudades inteligentes ya que es mejor tener una red que use todos sus canales sincronizados a las mismas frecuencias y es mejor tener una sola red operando para evitar coliciones.

Terminaré con algunos sitios de referencia que sean de utilidad par todos:

* [Semtech Lora Website](http://www.semtech.com/wireless-rf/internet-of-things/)
* [LoRa Alliance](https://www.lora-alliance.org)
* [LoRaWAN Architecture](http://www.3glteinfo.com/lora/lora-architecture/)
* [LoRaWAN for Arduino, Raspberry PI & Waspmote](https://www.cooking-hacks.com/documentation/tutorials/lorawan-for-arduino-raspberry-pi-waspmote-868-900-915-433-mhz/)
* [A Comparison of LPWAN Technologies](http://www.digi.com/blog/iot/lpwan-technology-comparison/)
