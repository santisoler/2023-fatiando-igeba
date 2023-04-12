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

<!-- .slide: class="center" -->

## Acerca de

<div class="d-flex flex-column">

<div>
<img src="images/santisoler.jpg" alt="">
</div>

<div>

- Lic en Física (UNR)
- Doctor en Geofísica (UNSJ)
- Actualmente: Postdoc en University of British Columbia

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
