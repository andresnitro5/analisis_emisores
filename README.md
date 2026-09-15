# Servicios financieros — Bancos de primer piso · 1S2026

Informe interactivo del área de **Middle Office · Laboratorio Financiero UTP** sobre los
emisores del subsector bancario de primer piso, con corte a **30 de junio de 2026**.

Es una página web estática (un solo `index.html`) lista para publicarse con **GitHub Pages**.

## Estructura del repositorio

```
.
├── index.html        # El informe (página principal del sitio)
├── support.js        # Motor de render del documento (dc-runtime)
├── assets/           # Imágenes del informe (logos, portada, organigramas, mapa de calor)
├── source/           # Materiales de trabajo (NO se publican como parte del sitio)
│   ├── Consolidado.md
│   ├── Sector_Bancos_1er_piso_Jun_26.xlsx
│   ├── imagenes-originales/     # Imágenes con sus nombres originales (respaldo)
│   └── Servicios financieros bancos primer piso 1S2026.dc.html   # Versión previa (respaldo)
├── .nojekyll         # Evita que GitHub Pages procese el sitio con Jekyll
└── README.md
```

## Publicar con GitHub Pages

1. Crea un repositorio en GitHub y sube **todo** el contenido de esta carpeta
   (incluye `index.html`, `support.js`, la carpeta `assets/` y el archivo `.nojekyll`).
2. En GitHub: **Settings → Pages**.
3. En **Build and deployment → Source** elige **Deploy from a branch**.
4. En **Branch** selecciona `main` y carpeta `/ (root)`. Guarda.
5. En 1–2 minutos el sitio quedará disponible en
   `https://<tu-usuario>.github.io/<nombre-del-repo>/`.

> Requiere conexión a internet al abrir la página: `support.js` carga React y Babel
> desde el CDN público de unpkg para renderizar las secciones interactivas
> (pestañas de emisores, indicadores, calificación y los botones de Aspectos/Factores).
> Las gráficas de indicadores son SVG incrustados y no dependen de internet.

## Editar el informe

- Todo el contenido y los estilos están en `index.html`.
- Las imágenes van en `assets/` y se referencian con rutas relativas (p. ej.
  `./assets/logo-bancolombia.png`). Si agregas imágenes, usa nombres sin espacios ni
  tildes para evitar problemas de rutas en la web.

## Comité de Riesgos Financieros

Laboratorio Financiero UTP · Middle Office · corte 30 de junio de 2026.
