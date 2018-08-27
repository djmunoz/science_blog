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


Ha medida que el radio de curvatura $$R$$ crece (es decir, el tamaño de la esfera sobre la que estamos parados aumenta), el ángulo $$\theta$$ se reduce. Cuando el radio $$R$$ is infinito -- lo que equivale a decir que la superficie sobre la que estamos parados **es plana** -- entonces $$\theta=0^\circ$$.


El Cálculo
----------------

Ahora que tenemos los principios básicos a la mano, calculemos la magnitud de la diferencia entre el punto de fuga, y el horizonte debido a la curvatura. Es una diferencia apreciable a simple vista?

Veamos. Ya sabemos que el infinito está a un ángulo de cero grados ($$0^\circ$$) por debajo de la línea de visión horizontal. A cuántos grados por debajo de la línea de visión está el horizonte?

Si el radio de la Tierra is de aproximadamente 6400 km y tu mides 1.75 metros, entonces,
por trigonometría básica (ver siguiente figura), el horizonte se encuentra a 


{% capture fig_img %}
![Foo]({{ "/images/horizon_angle.png" | relative_url }})
{% endcapture %}

<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption> Perspectiva de calles de Ciudad México, dibujadas usando la técnica del punto de fuga  (figure credit D.J.Munoz). </figcaption>
</figure>


De trigonometría básica sabemos que el tamaño angular $$\alpha$$ de un objeto
de ancho $$A$$ a una distancia $$D$$ obedece la relación

statement:\$$ \tan\alpha = \frac{A}{D} $$

\\begin{align}
\Delta \Sigma \dot{t} &= ((r^2+a^2)^2-\Delta a^2\sin^2\theta)E - 2Mr a L_z \\\
\Sigma^2 \dot{r}^2 &= E^2 r^4 + (a^2E^2-L_z^2-\mathcal{Q})r^2 + 2M[(aE-L_z)^2+\mathcal{Q}]r - a^2 \mathcal{Q} \\\
\Sigma^2\dot{\theta}^2 &= \mathcal{Q} - \left( \frac{L_z^2}{\sin^2\theta}-E^2a^2 \right)\cos^2\theta \\\
\Delta\Sigma\dot{\phi} &= 2MraE + (\Sigma-2Mr)\frac{L_z}{\sin^2\theta}
\\end{align}




El Experimento
----------------

Sin instrumentos, apreciar la diferenca
El experimento en este caso es simple.


