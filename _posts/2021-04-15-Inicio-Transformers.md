---
keywords: fastai
title: De que van los siguientes post(s) #
nb_path: _notebooks/2021-04-15-Inicio-Transformers.ipynb
layout: notebook
---

<!--
#################################################
### THIS FILE WAS AUTOGENERATED! DO NOT EDIT! ###
#################################################
# file to edit: _notebooks/2021-04-15-Inicio-Transformers.ipynb
-->

<div class="container" id="notebook-container">
        
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Esta arquitectura tiene una ventaja sobre lo que era en su momento el estado del arte la RNN  y las LSTM
Una de las principales ventajas es que el cómputo de las secuencias se hace paralelizable, con los modelos anteriores se procesaba la secuencia en orden, "añadiendo" el conocimiento de los datos ya procesados de uno por uno, en los transformers este computo se ejecuta en paralelo, otra característica de la arquitectura de transformers es la implementación de la autoatención, si bien el mecanismo de atención era algo que ya se usaba en otros contextos y modelos, en este caso hay dos tipos de atención una, combate la longitud variable de las secuencias, la attention mask, esta permite añadir caracteres de padding para normalizar la longitud de las secuencias y le "indica" al modelo que esos caraceteres no son relevantes, por otro lado, tambien tenemos el ya mencionado mecanismo de autoatención cuya finalidad es de cierta forma determinar el parecido o la correspondencia entre palabras, por ejemplificar, la palabra "hola" tendria un alto parecido a la palabra "hello", pero bajo respecto a la palabra "Queue"</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p>Durante los siguientes post implementaré una versión sencilla de esta arquitectura, la idea es que pueda 
realizar una tarea de traducción relativamente sencilla, la cual será invertir un patrón de caracteres.
Por ejemplo: abcd -----&gt; dcba</p>

</div>
</div>
</div>
</div>
 

