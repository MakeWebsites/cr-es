---
ID: 1085
post_title: Simulación del lavado de nitratos
author: AUtset
post_excerpt: ""
layout: post
permalink: >
  http://cr-es/simulacion-del-lavado-de-nitratos/
published: true
post_date: 2018-08-19 09:03:03
---
Uno de los principales problemas ambientales en la agricultura es la contaminación de los acuíferos por nitratos. El <strong>lavado de nitratos</strong> es un proceso físico complejo, que depende de muchas variables. Sin embargo, actualmente podemos simular cómo se produce este proceso a través de <a href="https://es.climarisk.com/modelos-agricolas-impacto-climatico/">modelos agrícolas</a>.
<!--more-->
<div class="row">
<div class="col-sm-7">
<p class="framed-box">El lavado de nitratos desde el suelo puede deberse a un exceso de fertilización, un manejo de riego inadecuado o también simplemente a la <a href="https://es.climarisk.com/variabilidad-climatica/">variabilidad climática</a>.</p>

</div>
<div class="col-sm-5"><img class="rounded img-responsive float-right mb-1" title="Lavado de nitratos debido al exceso de fertilizantes" src="https://climarisk.com/wp-content/uploads/2018/08/nitratos_fertilización.jpg" alt="Lavado de nitratos debido al exceso de fertilizantes"></div>
</div>
Las simulaciones con modelos pueden reducir la contaminación por nitratos de los acuíferos, a la vez que recomiendan mejoras para el manejo agrícola general. Asimismo, las simulaciones permiten estimar los riesgos de contaminación debido a la variabilidad climática.
<p class="framed-box">En Europa, la <a href="https://ec.europa.eu/environment/water/water-nitrates/index_en.html" target="_blank" rel="noopener noreferrer">Directiva de Nitratos</a> de la UE pretende reducir el lavado de nitratos de fuentes agrícolas. La Directiva proteje las aguas de los países que forman la Unión, promoviendo las <strong>"buenas prácticas agrícolas"</strong>.</p>
Todos los estados miembros de la UE tienen que cumplir la Directiva de Nitratos. La Directiva obliga a los países de la UE a controlar periódicamente el contenido de nitratos de las aguas, mediante una red de monitoreo. Los estados miembros deben declarar "Zonas Vulnerables de Nitratos" (ZVN) aquellos lugares con riesgos de contaminación o contenidos altos de nitratos. La Directiva de Nitratos obliga a los países a desarrollar "Programas de Acción" y a elaborar "Códigos de Buenas Prácticas Agrícolas". La Comisión Europea revisa el cumplimiento de la Directiva cada cuatro años. Actualmente, el área de ZVN constituye cerca del 50% del total del área agrícola de la UE.
<div class="row">
<div class="col-md-7"><a href="https://ec.europa.eu/environment/water/water-nitrates/index_en.html" target="_blank" rel="noopener noreferrer"><img class="rounded img-responsive align-left" title="Directiva de Nitratos de la UE" src="https://eur-lex.europa.eu/resource.html?uri=comnat:SWD_2018_0246_FIN.ENG.xhtml.SWD_2018_0246_FIN_ENG_26004.jpg" alt="Directiva de Nitratos de la UE"></a></div>
<div class="col-md-5">

El "Código de Buenas Prácticas" es de obligatorio cumplimiento en las ZVN para recibir ayudas agrícolas, de acuerdo a la condicionalidad de la Política Agraria Común (PAC) de la UE.

También, entre las "medidas agroambientales" de los Programas de Desarrollo Rural se promueven prácticas que reduzcan la contaminación por nitratos.

</div>
</div>
Sin embargo, un <a href="https://www.eca.europa.eu/en/Pages/DocItem.aspx?did=44179" target="_blank" rel="noopener noreferrer">informe reciente</a> del Tribunal de Cuentas de la UE señala varias deficiencias de la PAC en relación a los objetivos medioambientales europeos.
<h3>Simulación del lavado de nitratos: Procedimientos</h3>
Las simulaciones que se muestran a continuación corresponden al proyecto LIFE <a href="https://www.life-nitratos.eu/index.php" target="_blank" rel="noopener noreferrer">NITRATOS</a>. Un enfoque similar se me empleó en el proyecto <a href="https://www.freewat.eu/" target="_blank" rel="noopener noreferrer">FREEWAT</a> del Horizonte 2020 de la UE. Ambos proyectos fueron ejecutados por <a href="https://www.amaltea.com" target="_blank" rel="noopener noreferrer">Zeta Amaltea</a>. El objetivo en ambos casos fue facilitar la implementación de la Directiva de Nitratos, simulando el lavado de nitratos desde las áreas agrícolas.
<p class="framed-box">El procedimiento combina simulaciones 1D y 3D. El lavado de nitratos desde la zona no saturada del suelo se simuló utilizando el modelo agro-hidrológico <a href="https://www.swap.alterra.nl/" target="_blank" rel="noopener noreferrer">SWAP</a>. Empleamos el modelo hidrológico <a href="https://water.usgs.gov/ogw/modflow/" target="_blank" rel="noopener noreferrer">MODFLOW</a> para simular el movimiento 3D del agua y los solutos en la zona saturada.</p>
<img class="rounded img-responsive" title="Procedimiento para simular el lavado de nitratos" src="https://es.climarisk.com/wp-content/uploads/2018/08/procedimiento-lavado-de-nitratos.png" alt="Procedimiento para simular el lavado de nitratos">

Este procedimiento combinado para simular el lavado de nitratos ha sido empleado con éxito en Holanda, Italia y China. Nuestra contribución más importante radica en utilizar la información de las parcelas de la PAC. Las simulaciones se basan en los datos de cada parcela, con un manejo de fertilización y riego únicos, que se corresponde además con el informe oficial de los agricultores a los registros de la PAC.

Utilizamos una función de pedotransferencia para estimar los parámetros de Van Genuchten de las propiedades hidráulicas del suelo, requeridas como entrada para las simulaciones con SWAP. Se consideró la información de más de 900 perfiles de suelo, así como muestras tomadas específicamente para el proyecto.

<img class="rounded img-responsive mt-1" title="Simulación de lavado de Nitratos: Muestreo de suelos" src="https://es.climarisk.com/wp-content/uploads/2018/08/procedimiento-simulaciones-con-SWAP.png" alt="Simulación de lavado de Nitratos: Muestreo de suelos">

El procedimiento fue automatizado en un script. El programa escribe los ficheros SWAP, leyendo de la base de datos, corre el modelo, escribe los resultados y los pasa a MODFLOW.
<h3>Simulación del lavado de nitratos: Validaciones</h3>
<div class="row">
<div class="col-md-8"><img class="rounded img-responsive mb-2" title="Simulación del lavado de nitratos: Validaciones" src="https://climarisk.com/wp-content/uploads/2018/08/simulating-nitrate-leaching-validation.jpg" alt="Simulación del lavado de nitratos: Validaciones"></div>
<div class="col-md-4">

En general, hay una buena correspondencia entre las simulaciones y las mediciones de la red de control, especialmente en cuanto a las variaciones.

</div>
</div>
<p class="framed-box">La simulación del lavado de nitratos debido a la actividad agrícola pueden ayudar a la toma de decisiones, mejorando la actividad agrícola y sus consecuencias medioambientales. Las simulaciones pueden ser especialmente útiles para la implementación de la Directiva de Nitratos.</p>