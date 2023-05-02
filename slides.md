<!-- .slide: class="slide-title" data-background-image="images/fatiando-background.png" -->

<div class="title-authors r-stretch">
<h1 class="title"> Fatiando a Terra: <br> software libre para geofísica </h1>
<h2 class="authors"><a href="https://www.santisoler.com">Santiago Soler</a></h2>
</div>

<p class="location">
IGeBA  |  Abril 2023
</p>

<div class="d-flex flex-row align-center justify-around">
<img
class="institutional-logo"
src="images/logos/fatiando-light.png"
alt="Fatiando a Terra"
>
<img
class="institutional-logo"
src="images/logos/ubc-narrow.png"
alt="University of British Columbia"
>
<img
class="institutional-logo"
src="images/logos/igeba.jpg"
alt="IGeBA"
>
</div>

<p class="footer">
<i class="fa-solid fa-earth-americas"></i>
<a href="https://www.fatiando.org">fatiando.org</a>
|
<i class="fab fa-creative-commons"></i><i class="fab fa-creative-commons-by"></i>
Creative Commons Attribution 4.0
</p>

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
- awesome open geoscience: https://github.com/softwareunderground/awesome-open-geoscience


---

<div class="d-flex flex-row justify-between align-center">

# Acerca de

<div>
<img src="images/logos/unr.png" alt="" style="height: 2.5em; margin: 0">
<img src="images/logos/unsj.png" alt="" style="height: 2.5em; margin: 0">
<img src="images/logos/igsv.png" alt="" style="height: 2.5em; margin: 0">
<img src="images/logos/ubc.png" alt="" style="height: 2.5em; margin: 0">
</div>

</div>

<div class="centered r-stretch">

<div class="d-flex flex-row">

<div>
<img src="images/santisoler.jpg" alt="" style="width: 80%; border-radius: 50%">
</div>

<div>

<ul class="fa-ul">
    <li><i class="fa-li fa-sharp fa-solid fa-building-columns"></i>
        Lic en Física (UNR)
    </li>
    <li><i class="fa-li fa-sharp fa-solid fa-building-columns"></i>
        Doctor en Geofísica (UNSJ)
    </li>
    <li><i class="fa-li fa-sharp fa-solid fa-building-columns"></i>
        Postdoc en UBC, Canada
    </li>
    <li><i class="fa-li fas fa-flask"></i>
        Investigaciones:
    </li>
        <ul class="margin-left-0">
            <li class="text-medium">Procesamiento y modelado gravedad y magnetismo</li>
            <li class="text-medium">Inversiones conjuntas</li>
        </ul>
    <li><i class="fa-li fas fa-code"></i>
        Desarrollador de Fatiando a Terra 🌎
    </li>
</ul>

</div>

</div>
</div>

---

<!-- .slide: class="center"  -->

# ¿Qué es el software libre <br> u open-source?

---

<!-- .slide: class="center"  -->

## Libertades

0. <b class="green">Utilizar</b> el software con cualquier propósito
1. <b class="green">Estudiar</b> el código y <b class="green">modificarlo</b>
2. <b class="green">Distribuir copias</b> del software
3. <b class="green">Distribuir</b> versiones <b class="green">modificadas</b>

---

<!-- .slide: class="center" data-background-color="#eee" -->

## Ejemplos

<div class="d-flex flex-row justify-around align-center flex-wrap">

<div class="d-flex flex-column align-center justify-center">
<img src="images/logos/gmt.png" style="height: 5em; width: auto;">
Licencia: LGPLv3
</div>

<div class="d-flex flex-column align-center justify-center">
<img src="images/logos/qgis.png" style="height: 5em; width: auto;">
Licencia: GPLv2
</div>

</div>

<div class="d-flex flex-column align-center justify-center">
<img src="images/logos/fatiando-logo.png" style="height: 5em; width: auto;">
Licencia: BSD-Clause3
</div>


---

<!-- .slide: class="center"  -->

# ¿Por qué utilizar software libre en Ciencia?

---

<div class="r-stretch centered">

<img src="images/reproducibility-crisis.jpg"
alt="Infografia con resultados de investigación sobre la reproducibilidad de la ciencia, mostrando que un 52% de les entrevistades consideran que hay una crisis de reproducibilidad en la ciencia."
style="height: 100vh; width: auto;">

</div>

<div class="footnote">

Baker, M. (2016). doi: [10.1038/533452a](https://doi.org/10.1038/533452a)

</div>

---

<div class="r-stretch centered">

<img src="images/code-from-scratch.gif" alt="" style="width: 80vw;">

</div>

<div class="footnote">

[PhDComics (2014-03-14)](https://phdcomics.com/comics/archive.php?comicid=1689)

</div>

---

<!-- .slide: class="center"  -->

## El software libre:

- Posibilita una **Ciencia Abierta**
- Aumenta a la **reproducibilidad**
- **Democratiza** la Ciencia
- Facilita **desarrollos futuros**
- Favorece la **colaboración**

---

<!-- .slide: data-background-image="images/fatiando-banner.png" data-background-size="contain" data-background-color="#060629" -->

---

<!-- .slide: class="center" data-background-image="images/fatiando-background.png" -->

## Un poco de historia

<div class="d-flex flex-row justify-between align-start">

<div style="flex: 4">

- Comenzó en 2010
- Parte del Doctorado de **Leonardo Uieda** en Brasil
- Librería de Python: `fatiando`
- Herramientas para:
    - Procesar datos espaciales
    - Modelado de gravedad y magnetismo
    - Inversiones geométricas
    - Problemas juguete para docencia
- Circa 2015: primeras colaboraciones de Santiago

</div>

<div style="flex: 1">
<img src="images/leouieda.jpg" style="border-radius: 50%">
</div>

</div>

---

<!-- .slide: class="center" data-background-image="images/fatiando-background.png" -->

## Modernizar nuestras herramientas

<div class="d-flex flex-row justify-around align-between">
<img src="images/logos/python-3.png" style="width: auto; height: 100%;">
<p>+</p>
<p>Ecosistema científico <br> en Python</p>
</div>

<div style="background-color: #eee">
<img src="images/geoscientific-stack.png" style="width: 100%; height: auto;">
</div>

---

<!-- .slide: class="center" data-background-image="images/fatiando-background.png" -->

## ✨🌎 Librerías de Fatiando 🌎✨

---

<!-- .slide: class="center" data-background-color="#eeeeee" -->

<div class="r-stretch d-flex flex-column justify-evenly">

<!-- row 1 -->
<div class="fatiando-projects-row">

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

<!-- Harmonica -->
<div class="fatiando-project fragment">
<a href="http://www.fatiando.org/harmonica">
<img class="project-logo center-block" src="images/logos/harmonica-logo.svg">
</a>

Procesamiento y modelado de **gravedad** y **magnetismo**

<i class="fab fa-github fa-fw" title="Github repository"></i>
<a href="https://github.com/fatiando/harmonica">fatiando/harmonica</a>
</div>
<!-- - -->

</div>


<!-- row 2 -->
<div class="fatiando-projects-row">

<!-- Boule -->
<div class="fatiando-project fragment">
<a href="http://www.fatiando.org/boule">
<img class="project-logo center-block" src="images/logos/boule-logo.svg">
</a>

**Elipsoides de referencia** y cálculo de **gravedad normal**

<i class="fab fa-github fa-fw" title="Github repository"></i>
<a href="https://github.com/fatiando/boule">fatiando/boule</a>
</div>
<!-- - -->

<!-- Pooch -->
<div class="fatiando-project fragment">
<a href="http://www.fatiando.org/pooch">
<img class="project-logo center-block" src="images/logos/pooch-logo.svg">
</a>

**Descarga** y **almacena** datos de la web

<i class="fab fa-github fa-fw" title="Github repository"></i>
<a href="https://github.com/fatiando/pooch">fatiando/pooch</a>
</div>
<!-- - -->

<!-- Ensaio -->
<div class="fatiando-project fragment">
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

<!-- .slide: class="center" data-background-image="images/demo-time.gif" -->

<h1 style="text-shadow: 3px 3px 5px black;" >
Demos!
</h1>

---

<!-- .slide: class="center"  -->

## Descargá los Notebooks

<i class="fa fab fa-github" style="margin-top: 1em;"></i>
<a href="https://github.com/santisoler/2023-fatiando-igeba">
github.com/santisoler/2023-fatiando-igeba
</a>


---

<!-- .slide: class="center" data-background-image="images/fatiando-background.png" -->

# ¿Quién utiliza Fatiando?

---

<!-- .slide: data-background-image="images/fatiando-papers.png" data-background-size="contain" -->

---

<!-- .slide: class="center" data-background-image="images/fatiando-background.png" -->

# ¿Quién desarrolla Fatiando?

---

<!-- .slide: class="center slide-steering-council" data-background-image="images/fatiando-background.png" -->

## Steering council

<div class="d-flex flex-wrap flex-row align-start justify-evenly">

<div class="council-member">
<img src="https://www.github.com/aguspesce.png" >
<span>
<i class="fab fa-github fa-fw"></i>
<a href="https://github.com/aguspesce">aguspesce</a>
</span>
</div>

<div class="council-member">
<img src="https://www.github.com/leouieda.png" >
<span>
<i class="fab fa-github fa-fw"></i>
<a href="https://github.com/leouieda">leouieda</a>
</span>
</div>

<div class="council-member">
<img src="images/luli.jpg" >
<span>
<i class="fab fa-github fa-fw"></i>
<a href="https://github.com/ll-geo">LL-Geo</a>
</span>
</div>

<div class="council-member">
<img src="https://www.github.com/MGomezN.png" >
<span>
<i class="fab fa-github fa-fw"></i>
<a href="https://github.com/mgomezn">MGomezN</a>
</span>
</div>

<div class="council-member">
<img src="https://www.github.com/santisoler.png" >
<span>
<i class="fab fa-github fa-fw"></i>
<a href="https://github.com/santisoler">santisoler</a>
</span>
</div>

</div>

---

<!-- .slide: class="center slide-contributors" data-background-image="images/fatiando-background.png" -->

## Contribuidores

<div class="contributors">
<img src="https://www.github.com/mdtanker.png">
<img src="https://www.github.com/birocoles.png">
<img src="https://www.github.com/nshea3.png">
<img src="https://www.github.com/Esteban82.png">
<img src="https://www.github.com/djhoese.png">
<img src="https://www.github.com/lheagy.png">
<img src="https://www.github.com/jessepisel.png">
<img src="https://www.github.com/SAskevold.png">
<img src="https://www.github.com/andersy005.png">
<img src="https://www.github.com/GenevieveBuckley.png">
<img src="https://www.github.com/lukegre.png">
<img src="https://www.github.com/mathause.png">
<img src="https://www.github.com/hmaarrfk.png">
<img src="https://www.github.com/horta.png">
<img src="https://www.github.com/hugovk.png">
<img src="https://www.github.com/dokempf.png">
<img src="https://www.github.com/Xarthisius.png">
<img src="https://www.github.com/jrleeman.png">
<img src="https://www.github.com/drammock.png">
<img src="https://www.github.com/remram44.png">
<img src="https://www.github.com/neutrinoceros.png">
<img src="https://www.github.com/danshapero.png">
<img src="https://www.github.com/matthewturk.png">
<img src="https://www.github.com/avalentino.png">
<img src="https://www.github.com/dabiged.png">
<img src="https://github.com/BjoernLudwigPTB.png">
</div>

---

<!-- .slide: class="center slide-community" data-background-image="images/fatiando-background.png" -->

# ¡Participa en la comunidad!

<div class="signs">

<div class="sign">
<i class="fas fa-book"></i>
Aprende a usar las herramientas
<a href="https://www.fatiando.org/learn">fatiando.org/learn</a>
</div>


<div class="sign">
<i class="fas fa-comments"></i>
Contactate con el resto de la comunidad
<a href="https://www.fatiando.org/contact">fatiando.org/contact</a>
</div>

</div>

---

<!-- .slide: class="center" -->

# ¡Gracias!

---

<!-- .slide: class="center" -->

<div class="d-flex flex-row justify-between align-center">

<div>

## Contacto

<ul class="fa-ul">
<li>
<i class="fa-li fas fa-globe"></i>
<a href="https://www.fatiando.org">fatiando.org/contact</a>
</li>
<li>
<i class="fa-li fas fa-globe"></i>
<a href="https://www.santisoler.com">santisoler.com</a>
</li>
<li>
<i class="fa-li fab fa-mastodon"></i>
<a href="https://scicomm.xyz/@santisoler">@santisoler@scicomm.xyz</a>
</li>
<li>
<i class="fa-li fab fa-github"></i>
<a href="https://www.github.com/santisoler">santisoler</a>
</li>
</ul>

</div>

<div>

Diapositivas disponibles en
[santisoler.com/2023-fatiando-igeba](https://www.santisoler.com/2023-fatiando-igeba)

<img src="images/slides-qr.png" alt="" style="height: 7em;">

<p class="text-small">
<i class="fab fa-creative-commons"></i><i class="fab fa-creative-commons-by"></i>
Creative Commons Attribution 4.0
</p>

</div>

</div>
