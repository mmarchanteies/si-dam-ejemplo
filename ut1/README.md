# Apuntes UT1 · Herramientas y documentación del técnico

Fuentes de los apuntes de la UT1 de Sistemas Informáticos (DAM virtual, IES Juan Bosco, curso 2026-2027).

## Estructura

- `src/` — capítulos en Markdown (`00-presentacion.md` lleva los metadatos de portada).
- `img/` — diagramas propios (SVG) e imágenes con licencia libre (créditos en el Anexo D).
- `fonts/` — tipografías Inter y JetBrains Mono (licencia SIL OFL).
- `build/` — filtro Lua, plantillas HTML, hojas de estilo y `build.sh`.
- `plantillas/` — plantilla `README-tarea.md` y `.gitignore` para el alumnado.

## Generar el HTML y el PDF

Requisitos: `pandoc` 3.x y `weasyprint` (`pip install weasyprint`).

```bash
./build/build.sh
```

Se generan en `salida/`.

## Bloques destacados

Se escriben como citas que empiezan por una etiqueta, por ejemplo:

```markdown
> [!CASO] Título del caso
> Texto del caso.
```

Etiquetas: `CASO`, `NOTA`, `CONSEJO`, `AVISO`, `IMPORTANTE`, `SABERMAS`, `AUTOEVAL`, `CAPTURA`.

## Capturas pendientes

Buscar `[!CAPTURA]` en `src/`. Para sustituir un hueco por la captura real, guarda la imagen en `img/`
con el nombre sugerido y cambia el bloque completo por:

```markdown
![Descripción de la captura](img/nombre-sugerido.png)
```

## Licencia

CC BY-NC-SA 4.0, salvo las imágenes de terceros (Anexo D).
