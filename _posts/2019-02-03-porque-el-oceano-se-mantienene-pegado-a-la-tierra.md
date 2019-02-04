---
layout: posts
title:  Por qué el océano se mantiene pegado a la Tierra?
date:   2019-02-03
categories: [tierra] 
published: true
pinned: false
share: true
---

Por qué el océano se mantiene pegado a la Tierra a medida que ésta rota? Porque 1600 km/h NO es tan rápido como tú crees.


{% include toc %}

<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>


***
***

La velocidad de rotación de la Tierra en el ecuador es de aproximadamente 1600 kilómetros por hora. Esta velocidad suena muy alta, no? Pero alta respecto a qué? Sin duda es alta respecto a la velocidad a la que caminamos (1.4 metros por segundo o 5 kilómetros por hora). No suena *tan* alta comparada con la velocidad promedio de un avión comercial (un Boeing 777 alcanza velocidades crucero de 900 kilómetros por hora), y sin duda es baja comparada con la velocidad de un [Lockheed SR-71 Blackbird](https://en.wikipedia.org/wiki/Lockheed_SR-71_Blackbird), que alcanza velocidades de 3500  kilómetros por hora. 
Cuando uno habla de una velocidad "alta", esto sólo tiene sentido un términos relativos.

**Entonces ¿es 1600 km/h una velocidad alta?**

Un punto de referencia adecuado es la velocidad a la cual que la Tierra **podría potencialmente rotar**. 
La Tierra sólo puede rotar a una velocidad máxima; más rápido y se comienza a desarmar. En efecto, **a tales velocidades, los océanos serían puestos en órbita**. ¿Qué determina este máximo? 

Veamos a continuación...


Velocidad de escape y pozos de potencial
--------------------


Como lo explica de forma excelente [esta publicación de xkcd](https://www.explainxkcd.com/wiki/index.php/681:_Gravity_Wells), los planetas tienen un **pozo de potencial gravitacional**.  Mientras más profundo este pozo (es decir, mientras más masa tienen los planetas o más cerca estamos de ellos), más difícil es escapar de su gravedad. A mayor profundidad (o mayor energía gravitacional), uno necesita más energía de movimiento (energía cinética) para escapar de la atracción del planeta. Entonces, la ecuación de esta competencia es sencilla: **energía gravitacional versus energía cinética**. Los cohetes que son lanzados al espacio necesitan alcanzar cierto nivel de velocidad para poder competir con la atracción del planeta. Esta velocidad, llamada **velocidad de escape** es:
\\begin{align}
v_{\rm escape}=\sqrt{\frac{2GM_{\rm Tierra}}{R_{\rm Tierra}}}\approx 40000~ {\rm km/h}
\\end{align}
Lo que casi 30 veces mayor que la velocidad de rotación de la superficie terrestre.

Esta competencia entre el pozo de potencial y la energía de movimiento tiene una analogía con una juguera que funciona a varias velocidades. 


{% capture fig_img %}
![Foo]({{ "/images/behind_horizon.png" | relative_url }})
{% endcapture %}
<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption> Observación de un edificio ubicado por detrás del horizonte. Caso superior: el observador está ubicado con sus pies a cero elevación. Caso inferior: el observador aumenta su altura efectiva al estar parado sobre un relieve (figure credit D.J.Munoz). </figcaption>
</figure>



Velocidad de ruptura
--------------------

Cualquier objeto unido por la gravedad (la Tierra, otro planeta o una estrella) tiene un propiedad conocido como la "velocidad de ruptura". **Si el objeto rota más rápido que este límite, el éste se desarma**.
\\begin{align}
P_{\rm ruptura}=2\pi\sqrt{\frac{R^3}{GM}}
\\end{align}
En el caso de la Tierra, $$P_{\rm ruptura}\approx1.4~$$ horas, es decir, 17 veces más rápido que el período de rotación actual. 

Simplemente, **la Tierra rota demasiado lento como para poder lanzar sus océanos volando por el espacio**. Para poder lograr aquello, el día tendría que durar alrededor de una sola hora.


Estrellas que rotan rápido
--------------------

La física de deformación rotacional es aplicable a estrellas de todo tipo. De hecho, la geometría de una esfera de fluido deformada por la rotación **se puede calcular exactamente** (los detalles los dejamos para otro post). Un estrella deformada por su propia rotación adquiere la forma de un [**esferoide oblato**](https://en.wikipedia.org/wiki/Spheroid#Oblate_spheroids).


[Monnier et al (2007)](http://science.sciencemag.org/content/317/5836/342.full)

[!["hhi"](http://en.es-static.us/upl/2015/08/altair-800.jpg)](https://earthsky.org/brightest-stars/altair-the-bluish-jewel-of-the-eagle?utm_campaign=shareaholic)