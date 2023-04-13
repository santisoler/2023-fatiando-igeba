<!-- .slide: class="center" -->

# Fatiando a Terra: software libre para geofísica

Santiago Soler

<!-- UBC, IGEBA, etc -->

---

<!-- .slide: data-visibility="hidden" -->

## Layout

- acerca de mi
    - lic fisica en unr
    - phd en unsj
    - postdoc en ubc (ahora)
- que es software libre/open-source?
- por que usar sl en ciencia?
    - ciencia abierta
    - reproducibilidad
    - accesibilidad/democratizacion de la ciencia
    - avances sobre desarrollos anteriores (no reinventar la rueda)
    - favorece la colaboracion
- que es fatiando?
    - historia
    - herramientas actuales
- ejemplos con verde
    - data decimation
    - detrend
    - gridding/interpolation
- ejemplos con harmonica
    - processing gravity data
- cerrando
    - como se desarrolla fatiando (comunidad, colaboracion)
    - quienes desarrollan fatiando
    - quienes lo usan?
    - join the conversation


## dont forget to mention

- doctorado en unsj, donde comencé a colaborar con fatiando
- otros software libres en geofisica (python stack, gmt, qgis, gplates)
- integracion con otros software: pyproj, pygmt, etc


---

# Acerca de

<div class="centered r-stretch">

<div class="d-flex flex-row">

<div>
<img src="images/santisoler.jpg" alt="" style="width: 80%; border-radius: 50%">
</div>

<div>

- Lic en Física (UNR)
- Doctor en Geofísica (UNSJ)
- Postdoc en UBC, Canada
- Investigaciones:
    - Procesamiento y modelado gravedad y magnetismo
    - Inversiones conjuntas
- Desarrollador de Fatiando a Terra

</div>

</div>
</div>

---

<!-- .slide: class="center"  -->

# ¿Qué es el software libre <br> o open-source?

---

## Libertades

<div class="centered r-stretch">

0. **Utilizar** el software con cualquier propósito
1. **Estudiar** el código y **modificarlo**
2. **Distribuir copias** del software
3. **Distribuir** versiones **modificadas**

</div>

---

<!-- .slide: class="center"  -->

# ¿Por qué utilizar software libre en Ciencia?

---

<!-- .slide: class="center"  -->

- Posibilita una **Ciencia Abierta**
- Aumenta a la **reproducibilidad**
- **Democratiza** la Ciencia
- Facilita **desarrollos futuros**
- Favorece la **colaboración**

---

# Fatiando a Terra

---

<!-- .slide: class="center" -->

## Un poco de historia

<div class="d-flex flex-row justify-space-between align-start">

<div style="flex: 4">

- Comenzó en 2010
- Parte del Doctorado de **Leonardo Uieda** en Brasil
- Librería de Python: `fatiando`
- Herramientas para:
    - Procesar datos espaciales
    - Modelado de gravedad y magnetismo
    - Inversiones geométricas
    - Problemas juguete para docencia

</div>

<div style="flex: 1">
<img src="images/leouieda.jpg" style="border-radius: 50%">
</div>

</div>

---

<!-- .slide: class="center" -->

## Modernizar nuestras herramientas

---

<!-- .slide: class="center" -->

## Librerías de Fatiando

---

<!-- .slide: class="center" data-background-color="#eeeeee" -->

<div class="r-stretch d-flex flex-column justify-space-evenly">

<!-- row 1 -->
<div class="fatiando-projects-row">

<!-- Harmonica -->
<div class="fatiando-project">
<a href="http://www.fatiando.org/harmonica">
<img class="project-logo center-block" src="images/logos/harmonica-logo.svg">
</a>

Procesamiento y modelado de **gravedad** y **magnetismo**

<i class="fab fa-github fa-fw" title="Github repository"></i>
<a href="https://github.com/fatiando/verde">fatiando/harmonica</a>
</div>
<!-- - -->

<!-- Verde -->
<div class="fatiando-project">
<a href="http://www.fatiando.org/verde">
<img class="project-logo center-block" src="images/logos/verde-logo.svg">
</a>

**Procesamiento** e **interpolación** de datos espaciales
con un toque de machine learning

<i class="fab fa-github fa-fw" title="Github repository"></i>
<a href="https://github.com/fatiando/verde">fatiando/verde</a>
</div>
<!-- - -->

</div>


<!-- row 2 -->
<div class="fatiando-projects-row">

<!-- Boule -->
<div class="fatiando-project">
<a href="http://www.fatiando.org/boule">
<img class="project-logo center-block" src="images/logos/boule-logo.svg">
</a>

**Elipsoides de referencia** y cálculo de **gravedad normal**

<i class="fab fa-github fa-fw" title="Github repository"></i>
<a href="https://github.com/fatiando/boule">fatiando/boule</a>
</div>
<!-- - -->

<!-- Pooch -->
<div class="fatiando-project">
<a href="http://www.fatiando.org/pooch">
<img class="project-logo center-block" src="images/logos/pooch-logo.svg">
</a>

**Descarga** y **almacena** datos de la web

<i class="fab fa-github fa-fw" title="Github repository"></i>
<a href="https://github.com/fatiando/pooch">fatiando/pooch</a>
</div>
<!-- - -->

<!-- Ensaio -->
<div class="fatiando-project">
<a href="http://www.fatiando.org/ensaio">
<img class="project-logo center-block" src="images/logos/ensaio-logo.svg">
</a>

Sets de **datos geofísicos** bajo **licencia abierta** para experimentar

<i class="fab fa-github fa-fw" title="Github repository"></i>
<a href="https://github.com/fatiando/ensaio">fatiando/ensaio</a>
</div>
<!-- - -->

</div>

</div>

---

<div class="container small">
<div class="col">

### ✨New Fatiando✨

Split into libraries

Better coding practices

Use modern tools

Supplement the ecosystem

</div>
<div class="col fragment">

<a href="http://www.fatiando.org/pooch">
<img class="project-logo center-block" src="assets/pooch-logo.svg">
</a>

Data <b>download & caching</b> (used by other libraries)

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/pooch">fatiando/pooch</a>
</li>
<li><i class="fa-li fas fa-bookmark fa-fw" title="Publication"></i>
   doi: <a href="https://doi.org/10.21105/joss.01943">10.21105/joss.01943</a>
</li>
<li><i class="fa-li fa fa-check fa-fw" style="color: green" title="Project status"></i>
   Stable and ready for use
</li>
</ul>

</div>
<div class="col fragment">

<a href="http://www.fatiando.org/verde">
<img class="project-logo center-block" src="assets/verde-logo.svg">
</a>

ML-based point data processing and <b>gridding</b>

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/verde">fatiando/verde</a>
</li>
<li><i class="fa-li fas fa-bookmark fa-fw" title="Publication"></i>
   doi: <a href="https://doi.org/10.21105/joss.00957">10.21105/joss.00957</a>
</li>
<li><i class="fa-li fa fa-check fa-fw" style="color: green" title="Project status"></i>
   Stable and ready for use
</li>
</ul>

</div>
</div>
<div class="container small" style="margin-top: 4%">
<div class="col fragment">

<a href="http://www.fatiando.org/harmonica">
<img class="project-logo center-block" src="assets/harmonica-logo.svg">
</a>

Processing and modeling <b>gravity & magnetic</b> data

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/harmonica">fatiando/harmonica</a>
</li>
<li><i class="fa-li fa fa-sync-alt fa-fw" style="color: green" title="Project status"></i>
   Ready for use but still changing
</li>
</ul>

</div>
<div class="col fragment">

<a href="http://www.fatiando.org/boule">
<img class="project-logo center-block" src="assets/boule-logo.svg">
</a>

Reference <b>ellipsoids</b> for <b>normal gravity</b>

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/boule">fatiando/boule</a>
</li>
<li><i class="fa-li fa fa-sync-alt fa-fw" style="color: green" title="Project status"></i>
   Ready for use but still changing
</li>
</ul>

</div>
<div class="col fragment">

<a href="http://www.fatiando.org/ensaio">
<img class="project-logo center-block" src="assets/ensaio-logo.svg">
</a>

**Practice datasets** to probe your code

<ul class="fa-ul project-icons">
<li><i class="fa-li fab fa-github fa-fw" title="Github repository"></i>
   <a href="https://github.com/fatiando/ensaio">fatiando/ensaio</a>
</li>
<li><i class="fa-li fa fa-flask fa-fw" style="color: green" title="Project status"></i>
    Functional but still evolving
</li>
</ul>

</div>
</div>

---

<!-- .slide: class="center" -->

## This is another slide

<div class="centered r-stretch">

- with
- items

</div>

---

1. enumerate
2. lists

---

<!-- .slide: class="center" -->

# Code

```python
import harmonica as hm

hm.prism_gravity(coordinates, prisms, density, field="g_z")
```
