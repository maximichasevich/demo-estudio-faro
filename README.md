# Estudio Faro · Estudio de arquitectura

> **Proyecto de demostración.** Estudio Faro es un negocio ficticio. Hice este sitio
> como ejemplo de mi trabajo de diseño y desarrollo web. Conocé más en
> [michasevich.com](https://michasevich.com).

Sitio completo pensado para propietarios de alto nivel, desarrolladores inmobiliarios y clientes comerciales. Funciona como una página real: se puede
navegar, armar pedidos y guardar datos, pero no cobra nada ni envía
información a ningún servidor.

**Versión publicada:** [estudiofaro.michasevich.com](https://estudiofaro.michasevich.com)

## Tecnologías

- [Next.js 16](https://nextjs.org) con App Router
- React 19 y TypeScript
- Tailwind CSS 4 y componentes de Radix
- Efectos 3D hechos con CSS, sin librerías pesadas
- `localStorage` para guardar el carrito, los datos y los pedidos en el navegador del visitante
- Publicado en [Netlify](https://www.netlify.com)

## Estilo

Editorial de lujo monocromo: hueso, carbón y un único acento latón. Fuentes Cormorant Garamond, DM Mono y Hanken Grotesk. Fotografía a pantalla completa y menú de pantalla completa.

## Funcionalidades principales

- **Maqueta axonométrica 3D** con vistas, capas, separación de niveles y estudio solar.
- **Corte de una casa** con el recorrido del sol por estación y comparador croquis y obra.
- **Obras** con filtros, parallax y ficha con memoria, planta, materiales y visor.
- **Mapa de obras** y estimador orientativo de costo en dólares.
- **Área de clientes** de demostración con seguimiento de obra.
- **Agenda de reuniones** en 5 pasos.
- **Diario**, búsquedas laborales, dossier en PDF y newsletter.

## Cómo correrlo en local

Necesitás [Node.js](https://nodejs.org) 20.9 o más nuevo. Recomiendo la versión 22.

```bash
git clone https://github.com/maximichasevich/demo-estudio-faro.git
cd demo-estudio-faro
npm install
npm run dev        # http://localhost:3000
```

No hace falta configurar nada. Otros comandos:

```bash
npm run build && npm start   # versión optimizada
npm run lint                 # revisión de código
npm run typecheck            # revisión de tipos
```

## Configuración

`config/sitio.ts` tiene el nombre del negocio, la dirección de esta demo, la
del portfolio y el WhatsApp del botón "¿Querés una página así?". Las
direcciones también se pueden definir con las variables de `.env.example`.

## Estructura

```
app/layout.tsx          Base del sitio: fuentes, estilos globales y botón de WhatsApp
app/(sitio)/            Diseño, estilos y páginas de la demo
components/demos/       Secciones, componentes, aviso "Demo" y créditos de fotos
config/                 Nombre y direcciones
public/demos/           Fotos
```

## Créditos

Las fotos son de [Wikimedia Commons](https://commons.wikimedia.org) con
licencias libres. Cada foto muestra su autor y licencia dentro del sitio.

## Autor

Diseñado y desarrollado por Maximiliano Michasevich.
[michasevich.com](https://michasevich.com) · contacto@michasevich.com

---

## English

**Estudio Faro is a demo project for a fictional business.** An editorial, high-end website for an architecture studio. It was built by
Maximiliano Michasevich, a web designer and developer based in Montevideo,
Uruguay, as a portfolio sample. See more at [michasevich.com](https://michasevich.com).

- **Live demo:** [estudiofaro.michasevich.com](https://estudiofaro.michasevich.com)
- **Stack:** Next.js 16, React 19, TypeScript, Tailwind CSS 4, Netlify.
- **Highlights:** interactive 3D axonometric model with sun study, project pages with technical sheets, cost estimator, client area and a 5-step meeting scheduler.
- **Run locally:** `npm install`, then `npm run dev`.
