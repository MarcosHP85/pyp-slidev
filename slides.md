---
theme: apple-basic
layout: intro-image
image: ./images/background.png
---

<div class="transform top-1/2 -translate-y-1/2 absolute">
  <img src="images/atom.png" class="h-12">
  <h1 class="pt-8 !text-white">Titulo de<br>presentación</h1>
  <p class="pb-12 text-gray-600">subtitulo de presentación</p>
  <img src="images/banner.png" class="h-14">
</div>

<img src="images/unida.png" class="right-10 w-12 absolute">

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

<img src="images/atom-blue.png" class="h-12 top-14 right-14 absolute">

### Epígrafe

# Tareas diárias

## subtítulo

<p w="3/4">
Durante el proceso diario de planificación y programación es necesario contar con información, que actualmente se encuentra distribuida y clasificada de manera arbitraria.
</p>

- Resumen diario de novedades
- Ordenes de trabajo, Historial, Preventivos
- Planos, Flowsheet, Instrucciones internas
- Repuestos, Solicitudes de compra
- PQ de trabajos, Fotos, Manuales
- Puenteos, MI, MIT, Equipos indisponibles, etc...

<arrow v-click x1="355" y1="295" x2="718" y2="230" color="#ff595e" width="2.5" arrowSize="1" />
<arrow v-after x1="420" y1="330" x2="718" y2="290" color="#ff595e" width="2.5" arrowSize="1" />
<arrow v-after x1="420" y1="360" x2="718" y2="350" color="#ff595e" width="2.5" arrowSize="1" />
<arrow v-after x1="365" y1="395" x2="718" y2="415" color="#ff595e" width="2.5" arrowSize="1" />
<arrow v-after x1="350" y1="425" x2="718" y2="480" color="#ff595e" width="2.5" arrowSize="1" />

<div v-after class="right-24 bottom-4 w-max-38 absolute">
  <div class="flex items-center">
    <img src="images/informe-diario.png" class="m-1 w-18">
    <p class="text-sm ml-2">INTRANET operaciones</p>
  </div>
  <div class="flex items-center">
    <img src="images/ifs.png" class="m-1 w-18">
    <p class="text-sm ml-2">IFS</p>
  </div>
  <div class="flex items-center">
    <img src="images/documentacion.png" class="m-1 w-18">
    <p class="text-sm ml-2">Ingenieria Documentación</p>
  </div>
  <div class="flex items-center">
    <img src="images/sap.png" class="m-1 w-18">
    <p class="text-sm ml-2">SAP</p>
  </div>
  <div class="flex items-center">
    <img src="images/pq-trabajo.png" class="m-1 w-18">
    <p class="text-sm ml-2">Carpeta compartida</p>
  </div>
</div>


---

<img src="images/atom-blue.png" class="h-12 top-14 right-14 absolute">

### Epígrafe

# ¿Qué es un CMMS?

## subtítulo

CMMS, abreviatura en inglés de sistema computarizado de gestión de mantenimiento, es un software que ayuda a gestionar activos, programar mantenimiento y realizar seguimiento de las órdenes de trabajo.

Es un software que **centraliza** la información de mantenimiento y facilita los procesos de las operaciones de mantenimiento.

<br>
<br>

[IBM - ¿Qué es un CMMS?](https://www.ibm.com/ar-es/topics/what-is-a-cmms)


---
preload: false
---

<img src="images/atom-blue.png" class="h-12 top-14 right-14 absolute">

### Epígrafe

# Propuesta

## subtítulo

Aplicación web

<div
  v-if="$slidev.nav.clicks >= 0"
  class="top-78 left-50 absolute"
  v-motion
  :initial="{ x: 0 }"
  :enter="{ x: -80, transition: { delay: 1000, duration: 1000}}">
  <flat-color-icons-manager class="text-5xl" />
  <flat-color-icons-reading-ebook class="text-5xl" />
  <flat-color-icons-reading class="text-5xl" />
</div>

<arrow x1="400" y1="310" x2="680" y2="200" color="#ff595e" width="2.5" arrowSize="1" />
<arrow x1="400" y1="325" x2="680" y2="270" color="#ff595e" width="2.5" arrowSize="1" />
<arrow x1="400" y1="340" x2="680" y2="330" color="#ff595e" width="2.5" arrowSize="1" />
<arrow x1="400" y1="355" x2="680" y2="395" color="#ff595e" width="2.5" arrowSize="1" />
<arrow x1="400" y1="370" x2="680" y2="460" color="#ff595e" width="2.5" arrowSize="1" />

<img
  v-if="$slidev.nav.clicks >= 0"
  src="images/webapp.png"
  class="top-75 left-85 w-24 absolute"
  v-motion
  :initial="{ y: -20, opacity: 0 }"
  :enter="{ y: 0, opacity: 1, transition: { delay: 1000, duration: 1000}}">

<div class="right-34 bottom-8 w-max-38 absolute">
  <div class="flex items-center">
    <img src="images/informe-diario.png" class="m-1 w-18">
    <p class="text-sm ml-2">INTRANET operaciones</p>
  </div>
  <div class="flex items-center">
    <img src="images/ifs.png" class="m-1 w-18">
    <p class="text-sm ml-2">IFS</p>
  </div>
  <div class="flex items-center">
    <img src="images/documentacion.png" class="m-1 w-18">
    <p class="text-sm ml-2">Ingenieria Documentación</p>
  </div>
  <div class="flex items-center">
    <img src="images/sap.png" class="m-1 w-18">
    <p class="text-sm ml-2">SAP</p>
  </div>
  <div class="flex items-center">
    <img src="images/pq-trabajo.png" class="m-1 w-18">
    <p class="text-sm ml-2">Carpeta compartida</p>
  </div>
</div>


---
preload: false
---

<img src="images/atom-blue.png" class="h-12 top-14 right-14 absolute">

### Epígrafe

# Detalles

## subtítulo

<div class="flex">
  <div class="border-2 p-4 flex flex-col items-center">
    <div class="pb-2">webapp backend</div>
    <carbon:bare-metal-server-02 class="text-4xl" />
  </div>
  <div
    v-if="$slidev.nav.clicks >= 0"
    class="flex space-x-10 mx-10"
    v-motion
    :initial="{ opacity: 0 }"
    :enter="{ opacity: 1, transition: { delay: 1000, duration: 1000}}">
    <div class="border-2 w-4 mt-10 rounded-lg bg-blue-200 border-blue-300"></div>
    <carbon:update-now class="top-17 relative" />
  </div>
  <div class="border-2 p-2">
    <div class="pb-2">IFS</div>
    <div class="border-2 p-2">
      <div class="pb-2">
        <carbon:data-base /> Oracle
      </div>
      <div class="border-2 p-2">
        <carbon:data-table /><carbon:data-table /><carbon:data-table /><carbon:data-table />
      </div>
    </div>
  </div>
</div>


---
class: px-20
---

# Themes

Slidev comes with powerful theming support. Themes can provide styles, layouts, components, or even configurations for tools. Switching between themes by just **one edit** in your frontmatter:

<div grid="~ gap-2 cols-2" m="-t-2">

```yaml
---
theme: default
---
```

```yaml
---
theme: seriph
---
```

<img border="rounded" src="https://github.com/slidevjs/themes/blob/main/screenshots/theme-default/01.png?raw=true">

<img border="rounded" src="https://github.com/slidevjs/themes/blob/main/screenshots/theme-seriph/01.png?raw=true">

</div>

Read more about [How to use a theme](https://sli.dev/themes/use.html) and
check out the [Awesome Themes Gallery](https://sli.dev/themes/gallery.html).

---
preload: false
---

# Animations

Animations are powered by [@vueuse/motion](https://motion.vueuse.org/).

```html
<div
  v-motion
  :initial="{ x: -80 }"
  :enter="{ x: 0 }">
  Slidev
</div>
```

<div class="mt-6 w-60 relative">
  <div class="h-40 w-40 relative">
    <img
      v-motion
      :initial="{ x: 800, y: -100, scale: 1.5, rotate: -50 }"
      :enter="final"
      class="top-0 right-0 bottom-0 left-0 absolute"
      src="https://sli.dev/logo-square.png"
    />
    <img
      v-motion
      :initial="{ y: 500, x: -100, scale: 2 }"
      :enter="final"
      class="top-0 right-0 bottom-0 left-0 absolute"
      src="https://sli.dev/logo-circle.png"
    />
    <img
      v-motion
      :initial="{ x: 600, y: 400, scale: 2, rotate: 100 }"
      :enter="final"
      class="top-0 right-0 bottom-0 left-0 absolute"
      src="https://sli.dev/logo-triangle.png"
    />
  </div>

  <div 
    class="top-14 left-40 text-5xl text-[#2B90B6] -z-1 absolute"
    v-motion
    :initial="{ x: -80, opacity: 0}"
    :enter="{ x: 0, opacity: 1, transition: { delay: 2000, duration: 1000 } }">
    Slidev
  </div>
</div>

<!-- vue script setup scripts can be directly used in markdown, and will only affects current page -->
<script setup lang="ts">
const final = {
  x: 0,
  y: 0,
  rotate: 0,
  scale: 1,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
</script>

<div
  v-motion
  :initial="{ x:35, y: 40, opacity: 0}"
  :enter="{ y: 0, opacity: 1, transition: { delay: 3500 } }">

[Learn More](https://sli.dev/guide/animations.html#motion)

</div>

---

# LaTeX

LaTeX is supported out-of-box powered by [KaTeX](https://katex.org/).

<br>

Inline $\sqrt{3x-1}+(1+x)^2$

Block
$$
\begin{array}{c}

\nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t} &
= \frac{4\pi}{c}\vec{\mathbf{j}}    \nabla \cdot \vec{\mathbf{E}} & = 4 \pi \rho \\

\nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t} & = \vec{\mathbf{0}} \\

\nabla \cdot \vec{\mathbf{B}} & = 0

\end{array}
$$

<br>

[Learn more](https://sli.dev/guide/syntax#latex)

---

# Diagrams

You can create diagrams / graphs from textual descriptions, directly in your Markdown.

<div class="-mb-6 grid pt-4 gap-10 grid-cols-2">

```mermaid {scale: 0.9}
sequenceDiagram
    Alice->John: Hello John, how are you?
    Note over Alice,John: A typical interaction
```

```mermaid {theme: 'neutral', scale: 0.8}
graph TD
B[Text] --> C{Decision}
C -->|One| D[Result 1]
C -->|Two| E[Result 2]
```

</div>

[Learn More](https://sli.dev/guide/syntax.html#diagrams)


---
layout: center
class: text-center
---

# Learn More

[Documentations](https://sli.dev) · [GitHub](https://github.com/slidevjs/slidev) · [Showcases](https://sli.dev/showcases.html)
