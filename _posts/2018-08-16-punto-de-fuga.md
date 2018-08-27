---
layout: posts
title:  Punto de Fuga
date:   2018-08-16 
categories: [tierra] 
published: true
pinned: false
---

La línea del horizonte se encuentra a una distancia enorme ("infinita")? O simplemente a sólo algunos kilómetros de distancia? Cuál es la relación entre el horizonte y el punto de fuga?


{% include toc %}

<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>


***
***


Todos sabemos que a medida que un objeto se aleja, se ve más pequeño. El objeto no ha cambiado en sí. Es el **tamaño angular** que éste cubre en nuestro campo de visión el se reduce con la distancia (ver siguiente figura ilustrando este efecto). Uno puede extrapolar este hecho y afirmar que, a medida que el objeto se va "hacia el infinito", su tamaño angular se reducirá a cero. Cuando el objeto **se reduce a un punto**, la ubicación de éste es conocida como [**el punto de fuga**](https://es.wikipedia.org/wiki/Punto_de_fuga).


{% capture fig_img %}
![Foo]({{ "/images/vanishing_point.png" | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption> El "punto de fuga", es la proyección hacia el infinito del tamaño angular de un objecto, percibido por un observador a medida que el objeto se aleja de éste (figure credit D.J.Munoz). </figcaption>
</figure>


La geometría básica detrás del concepto de punto de fuga sirve como herramienta esencial en la ilustración de perspectiva tridimensional. Esta técnica es de conocimiento común para diseñadores, artistas y arquitectos. Para **representar la perspectiva del observador** en el papel, uno utiliza el infinito, posicionándolo en algún punto del cuadro, generando líneas rectas (paralelas en el mundo 3D, pero convergentes en la proyección 2D) a partir de ese punto de origen.

Como ejemplo, he usado una foto que tomé en Noviembre de 2017 en ciudad de México, cerca del Zócalo (ver figura). Primero, uno identifica la ubicación del punto de fuga en la imagen, y luego traza líneas rectas a partir de ese punto (segundo panel). Uno puede incluir trazos adicionales que representan las líneas que son verticales en el espacio 3D real (tercer panel), para finalmente asignar colores que separen las distintas estructuras (cuarto panel).

{% capture fig_img %}
![Foo]({{ "/images/mexico_vanishing_point.png" | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption> Perspectiva de calles de Ciudad México, dibujadas usando la técnica del punto de fuga  (figure credit D.J.Munoz). </figcaption>
</figure>


El Horizonte y el Infinito
----------------

Cuál es la relación entre estos conceptos y la línea del horizonte?
Es la desaparición de barcos en el horizonte un efecto de la curvatura de la Tierra, o una consecuencia de la distancia, similar a la de punto de fuga?

Pues bien, la diferencia entre mirar al infinito y mirar al **verdadero horizonte** es muy clara cuando el observador se encuentra sobre superficies de radio de curvatura pequeño (es decir, sobre una esfera pequeña). La siguiente figura ilustra esta diferencia.
 

{% capture fig_img %}
![Foo]({{ "/images/horizon_simple.png" | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption> Perspectiva de calles de Ciudad México, dibujadas usando la técnica del punto de fuga  (figure credit D.J.Munoz). </figcaption>
</figure>


A medida que el radio de curvatura $$R$$ crece (es decir, el tamaño de la esfera sobre la que estamos parados aumenta), el ángulo $$\theta$$ se reduce. Cuando el radio $$R$$ is infinito -- lo que equivale a decir que la superficie sobre la que estamos parados **es plana** -- entonces $$\theta=0^\circ$$. Es decir, si uno **viviera sobre un plano infinito** (o el radio de curvatura $$R$$ is infinito), el **el horizonte siempre estaría a nivel de los ojos**, como se ilustra en la siguiente figura.


El Cálculo
----------------

Ahora que tenemos los principios básicos a la mano, calculemos la magnitud de la diferencia entre el punto de fuga, y el horizonte debido a la curvatura. Es una diferencia apreciable a simple vista?

Veamos. Ya sabemos que el infinito está a un ángulo de cero grados ($$0^\circ$$) por debajo de la línea de visión horizontal. A cuántos grados por debajo de la línea de visión está el horizonte?

Si el radio de la Tierra is de aproximadamente 6400 km y tu mides 1.75 metros, entonces,
por trigonometría básica (ver siguiente figura), el horizonte se encuentra a 
una distancia $$d$$

{% capture fig_img %}
![Foo]({{ "/images/horizon_angle.png" | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption> Trigonometría básica detrás del cálculo de la distancia $$d$$ a la que se encuentra el horizonte  (figure credit D.J.Munoz). </figcaption>
</figure>

Usando el [teorema de Pitágoras](https://es.wikipedia.org/wiki/Teorema_de_Pitágoras),
podemos concluir que $$d$$ satisface la fórmula 


\\begin{align}
d^2 &= (R + h)^2 - R^2 = 2Rh + h^2 \\\
{\rm o sea}\\\
d &= \sqrt{2\times6400000\times1.75 + 1.75^2}~{\rm metros} = 4732~{\rm metros}
\\end{align}

Es decir, **el horizonte se encuentra sólo 5 kilómetros de distancia**!! 
Por supuesto, esto es asumiendo la ausencia de obstáculos (montañas, árboles, edificios), por lo que representa la realidad en lugares con muy poco relieve o en el mar.

Ahora, lo que nos interesa es ese ángulo $$\theta$$. De nuevo, usando el triángulo
rectángulo en la figura anterior, sabemos que existe una relación entre los lados
del triángulo y una propiedad de $$\theta$$ conocida como el coseno: 
statement:\$$ \cos\theta = \frac{R}{R+h} $$

Usando, como antes, $$R=6400$$ km y $$h=1.75$$ m, tenemos que el ángulo es 
\$$ \theta = 0.04^\circ  $$


Es decir, la diferencia entre mirar directo al infinito (a la altura de los ojos)
y mirar el horizonte en el mar, es de sólo 0.04 grados. Apreciar la este diferencia a simple vista (sin instrumentos) no es fácil. La resolución angular promedio del ojo humano es cerca de [0.02 grados](https://es.wikipedia.org/wiki/Simple_vista) por lo que somos apenas capaces de **físicamente** de notar esta diferencia. Para que el horizonte baje, digamos, un grado completo, por debajo de la línea horizontal, tendríamos que ir mucho más alto. Reemplazando $$\theta=1^\circ$$ en la ecuación anterior, encontramos que la altura necesaria es de $$h=975$$~metros! Lo que supera la altura del 
[edificio más alto del mundo](https://es.wikipedia.org/wiki/Burj_Khalifa). Esta dificultad puede ser superada por el experimento que descrito a continuación.


El Experimento
----------------

Sin instrumentos, apreciar la diferencia de xx grados a simple vista 
no es fácil. Sin embargo XX grados no es poco. Como referencia, el **tamaño angular**
de La Luna y el Sol es aproximadamente el mismo y corresponde a más o menos medio
grado. 

El experimento en este caso es simple. En lugar de intentar medir 


