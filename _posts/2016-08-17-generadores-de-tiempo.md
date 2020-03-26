---
ID: 130
post_title: >
  Generadores de tiempo y análisis de
  impacto climático
author: ANGEL UTSET
post_excerpt: ""
layout: post
permalink: >
  https://es.climarisk.com/generadores-de-tiempo/
published: true
post_date: 2016-08-17 06:30:54
---
Los generadores de tiempo ofrecen valores diarios de las variables meteorológicas, estadísticamente equivalentes a las series históricas del lugar.
<div class="row">
<div class="col-md-5">
<img class="img-responsive img-rounded" src="https://es.climarisk.com/wp-content/uploads/2016/08/weather-generators-300x156.gif" alt="Generadores de tiempo"></div>
<div class="col-md-7">

Han sido especialmente muy utilizados para <a href="https://www.ipcc-data.org/guidelines/pages/weather_generators.html" target="_blank" rel="noopener noreferrer">analizar el efecto del Cambio Climático</a>.
<!--more-->
El procedimiento consiste en combinar el generador de tiempo con salidas de los <a title="Modelos Generales de Circulación" href="https://es.climarisk.com/2016/08/12/proyecciones-del-cambio-climatico/">GCM</a>.

</div>
</div>
<p class="framed-box">Los generadores de tiempo generalmente reproducen de una manera correcta las medias mensuales de las variables meteorológicas. No obstante subestiman su variabilidad.</p>

<h4>En todo caso, los generadores de tiempo reproducen la estadística de la serie histórica.</h4>
Existen varios generadores de tiempo, pero el norteamericano <a href="https://www.goldsim.com/Library/Models/Applications/Hydrology/WGENWeatherGenerationModel/" target="_blank" rel="noopener noreferrer">WGEN</a> y el inglés <a href="https://www.rothamsted.ac.uk/mas-models/larswg" target="_blank" rel="noopener noreferrer">LARS-WG</a> están entre los más comúnmente empleados. LARS-WG no asume distribuciones estadísticas a priori, lo cual es un enfoque diferente a generadores como WGEN y otros basados en series de Markov.
<div class="framed-box">Los generadores pueden ser “perturbados” añadiendo condiciones climáticas determinadas al proceso de generación. Un aumento mensual de temperatura, disminución de precipitaciones, etc. De esa forma las series generadas reflejan estadísticamente la variabilidad climática del lugar, pero consideran también estas alteraciones.</div>
Algunos generadores permiten incluso considerar un aumento en la variabilidad de las temperaturas. Para ello se perturba el proceso de generación indicando una desviación de la media mensual mayor a la histórica.
<h4>Los generadores de tiempo no pueden utilizarse directamente como pronósticos o similares. No obstante, ofrecen una vía para obtener información climática, estadísticamente equivalente a la del sitio bajo estudio, pero correspondiente al riesgo climático considerado.</h4>
Por ejemplo, <a href="https://journals.cambridge.org/action/displayAbstract?fromPage=online&amp;aid=8025029" target="_blank" rel="noopener noreferrer">Utset y Del Rio (2011)</a> emplearon un generador de tiempo, "perturbado" según <a href="https://es.climarisk.com/proyecciones-del-cambio-climatico/">proyecciones de Cambio Climático</a>. El objetivo fue estimar el riesgo de que la futura demanda de agua en el mes de Julio, de cultivos típicos de Valladolid, fuera mayor que la capacidad de suministro de riego.

<a href="https://www.sciencedirect.com/science/article/pii/S0378377406001004" target="_blank" rel="noopener noreferrer"><img class="size-medium wp-image-148 alignright" title="Simulating the effects of extreme dry and wet years on the water use of flooding-irrigated maize in a Mediterranean landplane. Agric. Water Manag. 85:77-84 (2006)" src="https://es.climarisk.com/wp-content/uploads/2016/08/ejemplo-uso-generador-de-tiempo-206x300.png" alt="Ejemplo de uso de generador de tiempo"></a>Por otra parte, a partir de las realizaciones obtenidas con los generadores de tiempo pueden seleccionarse al azar años que cumplen determinadas condiciones. <a title="Simulating the effects of extreme dry and wet years on the water use of flooding-irrigated maize in a Mediterranean landplane. Agric. Water Manag. 85:77-84 (2006)" href="https://www.sciencedirect.com/science/article/pii/S0378377406001004" target="_blank" rel="noopener noreferrer">Utset et al. (2006)</a> utilizaron LARS-WG para generar más de 300 series anuales en Zaragoza, para el período 1960-2000.

Posteriormente seleccionaron dos muestras de 30 años en las que las precipitaciones fueron muy bajas o muy altas respecto a la media histórica, durante el período vegetativo del maíz. Esa información climática se utilizó como entrada en el modelo agrohidrológico SWAP. Las simulaciones permitieron evaluar los efectos de diferentes estrategias de riego deficitario, considerando también la variabilidad climática.
<div class="framed-box">La metodología general para este tipo de estudios de impacto consiste en obtener muchas realizaciones de las variables meteorológicas. Todas estas series de años son  estadísticamente equivalentes a la serie histórica del lugar. Luego se procede a escoger, de forma aleatoria, aquellas series que cumplen las condiciones marcadas por una proyección del Cambio Climático o por un pronóstico estacional.</div>
Al combinar esta información meteorológica con un modelo de simulación se obtendrán estimaciones del impacto de las condiciones climáticas consideradas.