# Guía Interactiva - Investigación de Operaciones

Un entorno de estudio tipo "Dashboard" desarrollado para visualizar, repasar y comprender los algoritmos de redes y modelos de optimización (Programación Lineal) de la asignatura de Investigación de Operaciones. 

El proyecto destaca por sus **simuladores visuales interactivos** construidos de forma nativa, permitiendo ejecutar algoritmos matemáticos paso a paso sobre grafos y matrices sin recargar la página.

## Características Principales

El temario está dividido en 4 módulos interactivos:

1. **Modelo de Transporte:** Formulación de PL y simulador visual del algoritmo de la **Esquina Noroeste** (agotamiento de oferta/demanda).
2. **Problema de Asignación:** Simulador paso a paso del **Método Húngaro**, incluyendo visualización del trazado de líneas y el ajuste de la constante $k$ para casos excepcionales.
3. **Árbol de Mínima Expansión:** Grafo SVG interactivo que muestra la conexión de nodos acíclicos iteración por iteración.
4. **La Ruta Más Corta:** Resolución gráfica del algoritmo de **Dijkstra**, mostrando la transición de etiquetas temporales a permanentes y la actualización de distancias.

## Stack Tecnológico

Este proyecto fue diseñado priorizando el rendimiento y la escalabilidad, utilizando un enfoque *Zero-JS-Framework* (sin React, Vue o Svelte) para el cliente:

- **Framework:** [Astro](https://astro.build/) (v6+)
- **Estilos:** [Tailwind CSS](https://tailwindcss.com/) (v3.4)
- **Tipado Estricto:** TypeScript
- **Interactividad:** Vanilla JavaScript + SVG Nativo
- **Diseño UI:** Estética Dark Tech / Dashboard Académico

## Estructura del Proyecto

```text
/
├── public/                 # Assets estáticos (favicon, etc.)
├── src/
│   ├── components/         # Componentes aislados
│   │   ├── Navbar.astro
│   │   ├── GrafoDijkstraInteractivo.astro
│   │   ├── GrafoInteractivo.astro
│   │   ├── MatrizHungaroInteractiva.astro
│   │   └── MatrizTransporteInteractiva.astro
│   ├── layouts/            # Plantilla base (Fondo, fuentes, head)
│   │   └── Layout.astro
│   └── pages/              # Enrutamiento automático
│       ├── index.astro
│       ├── transporte.astro
│       ├── asignacion.astro
│       ├── arbol-expansion.astro
│       └── ruta-corta.astro
├── astro.config.mjs        # Configuración de integraciones
├── tailwind.config.mjs     # Configuración de diseño JIT
└── tsconfig.json           # Reglas estrictas de TypeScript
```
👨‍💻 Autor
Desarrollado por Nelson Avello

AveLogic Chile