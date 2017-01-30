---
layout: post
title: "Hello LoRa!"
description: ""
category: 
tags: []
---
{% include JB/setup %}

Desde hace un tiempo he venido aprendiendo cosas nuevas y muchas de esas están asociadas a lo que creo tendrán un auge en el 2020 o antes, y son aquellas cosas relacionadas con el **IoT**.

Unos meses atrás conocí el concepto de LPWAN (Low Power Wide Area Networks) y al investigar un poco mas sobre el tema y cual era su rol en el mundo del internet de las cosas supuse que iba a ser interesante y decidí sumergirme de lleno en el tema.

Antes de hablar de LPWAN quiero a manera de ejercicio hablar un poco de dos cosas **RF** y **WIRELESSS**. Ambas han estado con nosotros desde hace mas de un siglo, y su primer experimento fue dado por Guglielmo Marconi cuando a principios del siglo 20 decidió trasmitir código Morsa desde Comwall, Inglaterra hasta St Jhon's en Canada.

Por RF que técnicamente viene a ser un sinónimo de Wireless nos referimos a ciertas ondas electromagnéticas que existen entre los 3 KHz hasta 300 GHz, de las cuales, la mayoría en el espectro, son usadas para comunicaciones o señales de radar.

Pero que es LoRa&copy;? bueno, básicamente es un formato de modulación de señales eléctricas. Es propietario y fue creado por Cycleo una compañía que luego fue adquirida por Semtech&trade;, a pesar de ser cerrado el formato, si tienes algo de dinero podrías adquirir una licencia, cosa que ya hecho Semtech con algunos otros fabricantes de semiconductores.

*Para mas información sobre el formato de modulacion de LoRa&copy; [click aqui](https://www.link-labs.com/what-is-lora).*

Ahora hablemos de las cosas, si de las cosas que necesitan o que eventualmente serán conectadas a internet, y con esto me refiero por ejemplo a medidores de agua, energía ó gas, también podría mencionar pequeños sensores de temperatura, pero todos ellos tienen algo en común y es que sus requerimientos en temas de networking y energia son limitados, comparados a lo que necesita un smart phone, una tablet o un computador. y es aquí en donde vienen las LPWAN a salvarnos, y en esta ocasión hablaremos de LoRaWAN&trade;.

Que es LoRaWAN&trade; es un protocolo de red, definido y mantenido por la LoRa Alliance&trade;.

De entre algunos beneficios tenemos:

* Usa espectros gratuitos (868 MHz en Europa y 915 MHz en USA).
* Rango: algunos pocos kilómetros en áreas densas urbanas y hasta 15-30 kilómetros en áreas rurales.
* Batería: hasta mas de 10 años de vida.
* Costos: $2USD para un dispositivo y hasta $1USD por subscripción a una red LoRaWAN&trade;.

Pero pasemos a los aspectos técnicos y hablemos un poco de la Arquitectura de una red LoRaWAN&trade; en donde puedo mencionar cuatro grandes componentes:

* Mote ó End-point Device: En pocas palabras es “la cosa” en si, es decir el sensor que mide la cantidad de ruido generado en un punto especifico de tu ciudad y que cierta cantidad de tiempo te envía información para ser recolectada y analizada.
* El Gateway ó Concentrator: quien esta a cargo de recibir los datos de los motes y enviarlos a algo que se llama el Network Server.
* El Network Server: quien esta ahí para recibir todos los datos y enviarlos al Application Server adecuado con el fin de ser manipulados ó visualizados.
* El Application Server y Consumer Service: El uno sirve para administrar tus motes conectados a tu red y el otro quizás puede ser el elemento final a donde tus datos van a llegar y serán representados.


Para ser honestos LoRaWAN&trade; no es la única opcion en lo que a LPWAN se refiere de hecho hay opciones para donde escoger como por ejemplo SigFox, NB-IoT ó LTE-Advanced Pro; Pero a su favor podemos decir que varias ciudades del mundo hoy lo apuestan a LoRaWAN&trade; como una solución muy viable a la hora de generar redes publicas que aporten al desarrollo de ciudades inteligentes ya que es mejor tener una red que use todos sus canales sincronizados sobre la misma frecuencias y tener una sola red operando para evitar colisiones.

Esperemos ver pronto algunas implementaciones de LoRaWAN en Colombia. Terminaré con algunos sitios de referencia que sean de utilidad par todos:

* [Semtech Lora Website](http://www.semtech.com/wireless-rf/internet-of-things/)
* [LoRa Alliance](https://www.lora-alliance.org)
* [LoRaWAN Architecture](http://www.3glteinfo.com/lora/lora-architecture/)
* [LoRaWAN for Arduino, Raspberry PI & Waspmote](https://www.cooking-hacks.com/documentation/tutorials/lorawan-for-arduino-raspberry-pi-waspmote-868-900-915-433-mhz/)
* [A Comparison of LPWAN Technologies](http://www.digi.com/blog/iot/lpwan-technology-comparison/)

