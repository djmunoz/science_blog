---
layout: posts
title:  ¿Por qué los eclipses solares van de Oeste a Este?
date:   2020-12-07
categories: [tierra] 
published: true
pinned: false
share: true
---

 ¿Por qué los eclipses solares van de Oeste a Este? Respuesta corta: porque la Luna se mueve de Oeste a Este.


{% include toc %}

<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>


***
***

La Tierra demora 24 horas en completar una rotación, mientras que la Luna aproximadamente 28 días en completar una órbita alrededor de la Tierra. Entonces, a veces la gente concluye (erróneamente) que la Luna se desplaza más lento que la superficie de la Tierra. Esto llevaría a la siguiente (nuevamente errónea) conclusión: la sombra de la Luna en la superficie terrestre debería desplazarse de Este a Oeste, determinada principalmente por la rotación de la Tierra con la Luna aproximadamente fija. Como muestra la siguiente Figura

{% capture fig_img %}
![image]({{ "/images/earth_moon-1.pdf" | relative_url }})
{% endcapture %}
<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption> Eclipses con una Luna fija (figure credit D.J.Munoz). </figcaption>
</figure>




El error se encuentra en asumir que la Luna se encuentra fija. En realidad, la Luna se mueve más rápido que la superficie de la Tierra, y por lo tanto, la sombra de la Luna se sobrepone a la rotación terrestre. 


Para entender esta diferencia de velocidades, lo primero que hay que notar es la escala espacial. Usualmente, la escala del sistema Tierra-Luna se expresa como en la primera figura, cuando en realidad es así:

Es decir, la velocidad linea de la luna es
\\begin{align}
v_{\rm L}= 2\pi\frac{384,400 {\rm km}}{28 {\rm d}}\approx 3600 {\rm km/h}
\\end{align}

lo que es más de 2 veces más rápido que la velocidad de rotación terrestre en el ecuador
\\begin{align}
v_{\oplus,{\rm eq}}= 2\pi\frac{6,371 {\rm km}}{1 {\rm d}}\approx 1700 {\rm km/h}
\\end{align}



Mientras que la extensión longitudinal de Estados Unidos es de más 4500 km, la distancia en línea recta entre Temuco (Chile) y Viedma (Argentina) es de sólo 850 km, lo que implica que el eclipse, de comienzo en Chile a fin en Argentina, durará menos de una hora.

<iframe src="https://arc-anglerfish-washpost-prod-washpost.s3.amazonaws.com/public/QHMXAK2NTZECBK4TKVUPPQWOF4.png" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>



