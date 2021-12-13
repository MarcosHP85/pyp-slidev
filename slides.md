---
theme: apple-basic
layout: intro-image
image: /background.png
---

<div class="transform top-1/2 -translate-y-1/2 absolute">
  <img src="/atom.png" class="h-12">
  <h1 class="pt-8 !text-white">Titulo de<br>presentación</h1>
  <p class="pb-12 text-gray-600">subtitulo de presentación</p>
  <img src="/banner.png" class="h-14">
</div>

<img src="/unida.png" class="right-10 w-12 absolute">

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

<img src="/atom-blue.png" class="h-12 top-14 right-14 absolute">

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
    <img src="/informe-diario.png" class="m-1 w-18">
    <p class="text-sm ml-2">INTRANET operaciones</p>
  </div>
  <div class="flex items-center">
    <img src="/ifs.png" class="m-1 w-18">
    <p class="text-sm ml-2">IFS</p>
  </div>
  <div class="flex items-center">
    <img src="/documentacion.png" class="m-1 w-18">
    <p class="text-sm ml-2">Ingenieria Documentación</p>
  </div>
  <div class="flex items-center">
    <img src="/sap.png" class="m-1 w-18">
    <p class="text-sm ml-2">SAP</p>
  </div>
  <div class="flex items-center">
    <img src="/pq-trabajo.png" class="m-1 w-18">
    <p class="text-sm ml-2">Carpeta compartida</p>
  </div>
</div>


---

<img src="/atom-blue.png" class="h-12 top-14 right-14 absolute">

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

<img src="/atom-blue.png" class="h-12 top-14 right-14 absolute">

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
  src="/webapp.png"
  class="top-75 left-85 w-24 absolute"
  v-motion
  :initial="{ y: -20, opacity: 0 }"
  :enter="{ y: 0, opacity: 1, transition: { delay: 1000, duration: 1000}}">

<div class="right-34 bottom-8 w-max-38 absolute">
  <div class="flex items-center">
    <img src="/informe-diario.png" class="m-1 w-18">
    <p class="text-sm ml-2">INTRANET operaciones</p>
  </div>
  <div class="flex items-center">
    <img src="/ifs.png" class="m-1 w-18">
    <p class="text-sm ml-2">IFS</p>
  </div>
  <div class="flex items-center">
    <img src="/documentacion.png" class="m-1 w-18">
    <p class="text-sm ml-2">Ingenieria Documentación</p>
  </div>
  <div class="flex items-center">
    <img src="/sap.png" class="m-1 w-18">
    <p class="text-sm ml-2">SAP</p>
  </div>
  <div class="flex items-center">
    <img src="/pq-trabajo.png" class="m-1 w-18">
    <p class="text-sm ml-2">Carpeta compartida</p>
  </div>
</div>


---

<img src="/atom-blue.png" class="h-12 top-14 right-14 absolute">

### ¿Cómo se compone?

# Aplicación web

## arquitectura básica

<div class="flex justify-center">
  <img src="/architecture.png" class="w-[55%]">
</div>


---
preload: false
clicks: 8
---

<img src="/atom-blue.png" class="h-12 top-14 right-14 absolute">

### ¿por qué un arquitectura basada en eventos?

# Arquitectura

## como integrar con IFS

<div class="flex w-full justify-center">
  <div
    v-if="$slidev.nav.clicks >= 5"
    class="flex pt-12 items-start relative"
  >
    <div class="flex items-center">
      <img src="/webapp.png" class="border-dashed border-r-4 border-indigo-200 py-8 px-4 w-24">
      <div class="top-9 left-3 text-indigo-400 absolute">frontend</div>
      <div class="w-18 relative self-center">
        <div
          class="flex px-4 inset-0 text-indigo-200 items-center absolute"
        >
          <carbon:arrow-right
            v-motion
            class="-top-1 relative"
            :initial="{ x: -40, scale: 0 }"
            :enter="{ opacity: 1, x: 35, scale: 1.2, transition: { duration: 800, repeat: 2, repeatDelay: 4000, repeatType: 'loop' }}" />
          <carbon:arrow-left
            v-motion
            class="top-1 relative"
            :initial="{ x: 40, scale: 0 }"
            :enter="{ opacity: 1, x: -35, scale: 1.2, transition: { delay: 3000, duration: 800, repeat: 2, repeatDelay: 4000, repeatType: 'loop' }}" />
        </div>
      </div>
    </div>
  </div>
  <div class="flex flex-col py-4 self-end relative">
    <div
      v-if="$slidev.nav.clicks >= 5"
      class="flex flex-col mb-12 self-start"
    >
      <div class="border-dashed rounded-md border-2 border-indigo-200 p-2 relative">
        <carbon:bare-metal-server-02 class="text-4xl text-indigo-400" />
        <div class="-top-6 -left-1 text-indigo-400 w-24 absolute">backend</div>
      </div>
      <div class="h-18 relative">
        <div
          class="flex flex-col inset-0 text-indigo-200 items-center absolute"
        >
          <carbon:arrow-down
            v-motion
            class="-left-1 w-12 relative"
            :initial="{ scale: 0, y: -20 }"
            :enter="{ scale: 1.2, y: 95, transition: { delay: 1000, duration: 800, repeat: 3, repeatDelay: 4000, repeatType: 'loop' }}" />
          <carbon:arrow-up
            v-motion
            class="left-1 relative"
            :initial="{ scale: 0, y: 95 }"
            :enter="{ scale: 1.2, y: -20, transition: { delay: 2000, duration: 800, repeat: 3, repeatDelay: 4000, repeatType: 'loop' }}" />
        </div>
      </div>
    </div>
    <div v-if="$slidev.nav.clicks >= 4" class="flex items-center">
      <div class="border-dashed rounded-md border-2 border-indigo-200 p-2 relative">
        <carbon:data-base class="text-4xl text-indigo-400" />
        <div class="top-16 -left-3 text-indigo-400 w-24 absolute">DB propia</div>
      </div>
      <div class="flex pr-6 text-indigo-200 w-12 items-center">
        <carbon:arrow-left
          v-motion
          :initial="{ scale: 0, x: 75 }"
          :enter="{ scale: 1.2, x: 0, transition: { delay: 900, duration: 700, repeat: 2, repeatDelay: 4000, repeatType: 'loop' }}"
        />
      </div>
      <div class="rounded-md border-2 border-indigo-200 p-2">
        <carbon:video class="transform text-indigo-400 rotate-180" />
      </div>
      <div class="flex pr-6 text-indigo-200 w-12 items-center">
        <carbon:arrow-left
          v-motion
          :initial="{ scale: 0, x: 75 }"
          :enter="{ scale: 1.2, x: 0, transition: { duration: 700, repeat: 2, repeatDelay: 4000, repeatType: 'loop' }}"
        />
      </div>
    </div>
    <div
      v-if="$slidev.nav.clicks >= 7"
      class="flex flex-col top-[40%] right-0 absolute"
    >
      <div
        v-motion
        :initial="{ opacity: 0 }"
        :enter="{ opacity: 1, transition: { delay: 1000, duration: 800}}"
        class="flex pb-2"
      >
        <div class="rounded-md border-2 border-indigo-200 p-2">
          <carbon:email-new class="text-indigo-400" />
        </div>
        <div class="flex pr-6 text-indigo-200 w-12 items-center">
          <carbon:arrow-left />
        </div>
      </div>
      <div
        v-motion
        :initial="{ opacity: 0 }"
        :enter="{ opacity: 1, transition: { duration: 800}}"
        class="flex"
      >
        <div class="rounded-md border-2 border-indigo-200 p-2">
          <carbon:notification-new class="text-indigo-400" />
        </div>
        <div class="flex pr-6 text-indigo-200 w-12 items-center">
          <carbon:arrow-left />
        </div>
      </div>
    </div>
  </div>
  <div v-if="$slidev.nav.clicks >= 3">
    <div
      v-motion
      :initial="{ opacity: 0 }"
      :enter="{ opacity: 1, transition: { duration: 500}}"
      class="rounded-full bg-indigo-200 border-2 border-indigo-400 h-78 w-5 relative"
    >
      <div class="w-full transform bottom-20 text-indigo-700 -rotate-90 absolute whitespace-nowrap">message broker</div>
    </div>
  </div>
  <div class="flex flex-col">
    <div class="flex self-start">
      <div
        v-if="$slidev.nav.clicks >= 2"
        class="flex self-center items-stretch"
      >
        <div class="flex pr-6 text-indigo-200 w-12 items-center">
          <carbon:arrow-left
            v-if="$slidev.nav.clicks >= 3"
            v-motion
            :initial="{ scale: 0, x: 75 }"
            :enter="{ scale: 1.2, x: 0, transition: { duration: 700, repeat: 2, repeatDelay: 4000, repeatType: 'loop' }}" />
        </div>
        <div class="rounded-md border-2 border-indigo-200 p-2">
          <carbon:update-now 
            v-motion
            class="text-indigo-400"
            :initial="{ opacity: 0, rotate: 0 }"
            :enter="{ opacity: 1, rotate: -360, transition: { duration: 1000 }}" />
        </div>
        <div class="w-18 relative">
          <div
            v-if="$slidev.nav.clicks >= 2"
            class="flex px-4 inset-0 text-indigo-200 items-center absolute"
          >
            <carbon:arrow-right
              v-motion
              class="-top-1 relative"
              :initial="{ x: -40, scale: 0 }"
              :enter="{ opacity: 1, x: 35, scale: 1.2, transition: { delay: 1000, duration: 700, repeat: 2, repeatDelay: 4000, repeatType: 'loop' }}" />
            <carbon:arrow-left
              v-motion
              class="top-1 relative"
              :initial="{ x: 40, scale: 0 }"
              :enter="{ opacity: 1, x: -35, scale: 1.2, transition: { delay: 1700, duration: 700, repeat: 2, repeatDelay: 4000, repeatType: 'loop' }}" />
          </div>
        </div>
      </div>
      <div class="flex items-center">
        <div class="rounded-md border-2">
          <div class="p-2">IFS</div>
          <div class="flex justify-end">
            <div 
                v-if="$slidev.nav.clicks >= 1"
                class="rounded-md border-2"
                v-motion
                :initial="{ opacity: 0 }"
                :enter="{ opacity: 1, transition: { duration: 500}}"
              >
              <div class="p-2">
                <carbon:data-base /> Oracle
              </div>
              <div class="p-2">
                <carbon:data-table class="text-pink-500" /><carbon:data-table /><carbon:data-table /><carbon:data-table />
              </div>
            </div>
            <div class="rounded-sm h-full bg-pink-200 border-pink-300 border-2 h-min-20 w-4"></div>
          </div>
        </div>
        <carbon:arrow-left class="mx-2 text-pink-400" />
        <flat-color-icons-reading-ebook class="text-5xl" />
      </div>
    </div>
    <div v-if="$slidev.nav.clicks >= 6">
      <div
        v-motion
        :initial="{ opacity: 0 }"
        :enter="{ opacity: 1, transition: { duration: 500}}"
        class="flex self-start"
      >
        <div class="flex self-center items-stretch">
          <div class="flex pr-6 text-indigo-200 w-12 items-center">
            <carbon:arrow-left class="transform scale-120" />
          </div>
          <div class="rounded-md border-2 border-indigo-200 p-2">
            <carbon:update-now class="text-indigo-400" />
          </div>
          <div class="w-18 relative">
            <div class="flex px-4 inset-0 text-indigo-200 items-center absolute"
            >
              <carbon:arrow-right class="transform -top-1 scale-120 relative" />
              <carbon:arrow-left class="transform top-1 scale-120 relative" />
            </div>
          </div>
        </div>
        <img src="/informe-diario.png" class="m-1 w-18">
      </div>
      <div
        v-motion
        :initial="{ opacity: 0 }"
        :enter="{ opacity: 1, transition: { delay: 1000, duration: 800}}"
        class="flex self-start"
      >
        <div class="flex self-center items-stretch">
          <div class="flex pr-6 text-indigo-200 w-12 items-center">
            <carbon:arrow-left class="transform scale-120" />
          </div>
          <div class="rounded-md border-2 border-indigo-200 p-2">
            <carbon:update-now class="text-indigo-400" />
          </div>
          <div class="w-18 relative">
            <div class="flex px-4 inset-0 text-indigo-200 items-center absolute"
            >
              <carbon:arrow-right class="transform -top-1 scale-120 relative" />
              <carbon:arrow-left class="transform top-1 scale-120 relative" />
            </div>
          </div>
        </div>
        <img src="/documentacion.png" class="m-1 w-18">
      </div>
      <div
        v-motion
        :initial="{ opacity: 0 }"
        :enter="{ opacity: 1, transition: { delay: 2000, duration: 800}}"
        class="flex self-start"
      >
        <div class="flex self-center items-stretch">
          <div class="flex pr-6 text-indigo-200 w-12 items-center">
            <carbon:arrow-left class="transform scale-120" />
          </div>
          <div class="rounded-md border-2 border-indigo-200 p-2">
            <carbon:update-now class="text-indigo-400" />
          </div>
          <div class="w-18 relative">
            <div class="flex px-4 inset-0 text-indigo-200 items-center absolute"
            >
              <carbon:arrow-right class="transform -top-1 scale-120 relative" />
              <carbon:arrow-left class="transform top-1 scale-120 relative" />
            </div>
          </div>
        </div>
        <img src="/pq-trabajo.png" class="m-1 w-18">
      </div>
    </div>
  </div>
</div>
<div class="flex w-full bottom-5 text-gray-500 absolute">
  <div v-if="$slidev.nav.clicks === 1">La tabla de Auditoría de Ordenes de Trabajo, registra todos los cambios que en estas se producen.</div>
  <div v-if="$slidev.nav.clicks === 2">Cada pocos segundos se verifica si existe un nuevo registro.</div>
  <div v-if="$slidev.nav.clicks === 3">Los cambios que se producen en IFS son publicados en un bróker como NATS, RabbitMQ o Kafka.</div>
  <div v-if="$slidev.nav.clicks === 4">Un subscriptor lee estos eventos y actualiza los datos necesarios en otra base de datos.</div>
  <div v-if="$slidev.nav.clicks === 5">Esta aplicación web nos permite aplicar nuestra propia lógica de negocio y una interface a medida.</div>
  <div v-if="$slidev.nav.clicks === 6">Es posible diseñar publicadores de eventos para otras fuentes.</div>
  <div v-if="$slidev.nav.clicks === 7">Y subscriptores que generen otras acciones como crear notificaciones o enviar email.</div>
</div>
