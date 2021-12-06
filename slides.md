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

<p w="1/2">
Durante el proceso diario de planificación y programación es necesario contar con información, que actualmente se encuentra distribuida y clasificada de manera arbitraria. <carbon-user-multiple />
</p>

<div class="absolute top-24 right-30">
  <div class="flex items-center">
    <img src="images/informe-diario.png" class="w-18 m-2">
    <ul class="text-sm !list-none !mt-0">
      <li>Resumen diario de novedades</li>
    </ul>
  </div>
  <div class="flex items-center">
    <img src="images/ifs.png" class="w-18 m-2">
    <ul class="text-sm !list-none !mt-0">
      <li>Ordenes de trabajo</li>
      <li>Historial</li>
      <li>Preventivos</li>
    </ul>
  </div>
  <div class="flex items-center">
    <img src="images/documentacion.png" class="w-18 m-2">
    <ul class="text-sm !list-none !mt-0">
      <li>Planos</li>
      <li>Flowsheet</li>
      <li>Instrucciones internas, etc...</li>
    </ul>
  </div>
  <div class="flex items-center">
    <img src="images/sap.png" class="w-18 m-2">
    <ul class="text-sm !list-none !mt-0">
      <li>Repuestos</li>
      <li>Solicitudes de compra</li>
    </ul>
  </div>
  <div class="flex items-center">
    <img src="images/pq-trabajo.png" class="w-18 m-2">
    <ul class="text-sm !list-none !mt-0">
      <li>PQ de trabajo</li>
      <li>Fotos</li>
      <li>Manuales</li>
    </ul>
  </div>
  <div class="text-sm mt-2">Puenteos, modificación a la instalación <br> Equipos indisponibles</div>
</div>


---

# Navigation

Hover on the bottom-left corner to see the navigation's controls panel, [learn more](https://sli.dev/guide/navigation.html)

### Keyboard Shortcuts

|     |     |
| --- | --- |
| <kbd>right</kbd> / <kbd>space</kbd>| next animation or slide |
| <kbd>left</kbd>  / <kbd>shift</kbd><kbd>space</kbd> | previous animation or slide |
| <kbd>up</kbd> | previous slide |
| <kbd>down</kbd> | next slide |

<!-- https://sli.dev/guide/animations.html#click-animations -->
<img
  v-click
  class="opacity-50 -bottom-9 -left-7 w-80 absolute"
  src="https://sli.dev/assets/arrow-bottom-left.svg"
/>
<p v-after class="opacity-30 transform bottom-23 left-45 -rotate-10 absolute">Here!</p>

---
layout: image-right
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# Code

Use code snippets and get the highlighting directly![^1]

```ts {all|2|1-6|9|all}
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function updateUser(id: number, update: User) {
  const user = getUser(id)
  const newUser = {...user, ...update}  
  saveUser(id, newUser)
}
```

<arrow v-click="3" x1="400" y1="420" x2="230" y2="330" color="#564" width="3" arrowSize="1" />

[^1]: [Learn More](https://sli.dev/guide/syntax.html#line-highlighting)

<style>
.footnotes-sep {
  @apply mt-20 opacity-10;
}
.footnotes {
  @apply text-sm opacity-75;
}
.footnote-backref {
  display: none;
}
</style>

---

# Components

<div grid="~ gap-4 cols-2">
<div>

You can use Vue components directly inside your slides.

We have provided a few built-in components like `<Tweet/>` and `<Youtube/>` that you can use directly. And adding your custom components is also super easy.

```html
<Counter :count="10" />
```

<!-- ./components/Counter.vue -->
<Counter :count="10" m="t-4" />

Check out [the guides](https://sli.dev/builtin/components.html) for more.

</div>
<div>

```html
<Tweet id="1390115482657726468" />
```

<Tweet id="1390115482657726468" scale="0.65" />

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
