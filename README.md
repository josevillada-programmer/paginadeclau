# Página para Claudia

Página interactiva de Año Nuevo creada con Three.js.

Cómo abrir
- Abrir `index.html` en un navegador moderno (Chrome, Edge, Firefox).
- No requiere servidor, pero para evitar políticas de CORS en algunos navegadores puedes ejecutar un servidor local sencillo (por ejemplo con Python):

```
cd "c:\Users\joseb\Desktop\pagina para claudia"
python -m http.server 8000
```

Qué se cambió (optimización y mejoras)
- Corazones agrandados para una mejor visibilidad.
- Fondo animado sutil: overlay con gradiente y "twinkle" en las estrellas.
- Reducción del número de estrellas (600) para más fluidez.
- Se redujo la resolución geométrica de los planetas (más bajo recuento de polígonos).
- Se limitó el `devicePixelRatio` del renderer a `Math.min(window.devicePixelRatio, 2)` para evitar render muy pesado en pantallas HiDPI.
- ExtrudeGeometry para corazones con menos profundidad y sin bevel para reducir coste geométrico.

Notas y sugerencias
- Si la animación sigue lenta en equipos antiguos, reduce `STAR_COUNT` en `index.html`.
- Para pruebas locales, usa un servidor (ver ejemplo de Python arriba) para evitar discrepancias entre navegadores.

Contacto
- Si quieres más mejoras (música, más animaciones, o adaptarlo a móvil) dímelo y lo implemento.
