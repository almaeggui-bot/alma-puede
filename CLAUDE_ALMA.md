# CLAUDE_ALMA.md — MI REGALO PARA ALMA CON AMOR

> **Proyecto: "Mi regalo para Alma con amor"**
> Repo: `github.com/almaeggui-bot/alma-puede`
> Cuenta GitHub: `almaeggui-bot`
> Cuenta Vercel: `almaeggui-5646`
> URL producción: `alma-puede.vercel.app`
> Cuenta mail: `almaeggui@gmail.com`
> Portal: `index.html` (Vercel lo reconoce automáticamente)
>
> **Este proyecto NO pertenece a VAO Sistemas.**
> Cuentas, repo, numeración y reglas viven separados de VAO POS/SmartPOS.

---

## SOBRE ESTE PROYECTO

App educativa para Alma (16 años).
Objetivo: desarrollar cultura general argentina usando memoria visual,
asociación, descubrimiento, repetición y recuperación activa.

Arranca con Río Negro. Se extiende a las 24 jurisdicciones.
También conviven apps hermanas en el mismo repo (matemáticas).

**Este proyecto se trata con la misma seriedad y las mismas Reglas de Oro
que VAO POS/SmartPOS.** No es un experimento descartable.

---

## SOBRE MÍ (Víctor / VAO)

NO SOY PROGRAMADOR. Explicame simple, sin jerga.
Si no entendés mi pedido, preguntá antes de asumir.
Trabajo en criollo y espero respuestas en criollo.

---

## 🛑 REGLA CERO — ANTES DE TOCAR CÓDIGO

Antes de modificar cualquier archivo, declarar brevemente:

1. Qué archivo vas a modificar.
2. Qué sección exacta.
3. Qué NO vas a tocar.
4. Si detectás riesgo de romper una Regla de Oro.

Esperar mi OK. Después escribir.

---

## 🛑 REGLA MÁS IMPORTANTE

**NO ROMPER LO QUE YA FUNCIONA.**
PRIMERO PRESERVAR. DESPUÉS MODIFICAR.
NUNCA MODIFICAR POR MODIFICAR.

Una solicitud de cambio NO es autorización para modificar el resto.
Si dudás entre cambiar algo no pedido o conservarlo → CONSERVARLO.

Aplica especialmente a:
- Contenido educativo ya verificado (no se toca sin pedido explícito).
- Código del mapa, del quiz, de la repetición espaciada.
- Apps hermanas del repo (matemáticas).

---

## REGLAS DE ORO

1. `APP_VERSION` entero, +1 por entrega. Nunca `v1.2`, nunca `-v1.1`.
   Cada archivo del ecosistema tiene su PROPIO `APP_VERSION` independiente.

2. Entregar SIEMPRE 2 archivos idénticos:
   - `archivo.html` (producción, listo para subir)
   - `archivo_vNNN_backup.html` (historial)
   Ejemplo: `aprende-argentina.html` + `aprende-argentina_v3_backup.html`

3. Nunca salir de la página sin confirmación
   (history + popstate + botón atrás + swipe-back + links internos).

4. Ediciones del usuario → icono 💾 cuando hay cambios pendientes.

5. No volver a preguntar por estas reglas. Se aplican automáticamente.

6. Sin pull-to-refresh (`overscroll-behavior-y: contain`).

7. No recargar páginas que cargan datos por detalles de interfaz.
   Un solo botón de refrescar por pantalla.

8. Mensajes: centrado > abajo-izq > arriba-der. Nunca tapar info.

9. El usuario siempre debe poder desplazarse. Revisar overflow, height,
   max-height, fixed, absolute, overlays.

10. Verde = éxito. Rojo = error. Siempre.

11. El contenido principal (lista, mapa, pregunta) tiene prioridad de espacio.
    Lo secundario arranca colapsado.

12. Autoguardado en localStorage mientras se edita.
    💾 Guardar = almacenamiento definitivo.
    🛡️ localStorage = salvavidas automático de la edición.

13. Modularizar: núcleo liviano + páginas aparte. Nunca uno gigante.
    Antes de agregar feature: ¿es parte del flujo principal de la app,
    o es herramienta/página secundaria? Si es lo segundo, va aparte.
    Un índice/dashboard lista y enlaza las páginas independientes.

---

## REGLAS PROPIAS DE ESTE PROYECTO (ALMA)

14. **Sentido crítico ante todo.**
    Si dos fuentes serias no coinciden en un dato, NO se afirma un número
    cerrado. Se plantea como pregunta abierta que invite a investigar.
    Ejemplo real ya aplicado: "¿Cuántos MTV VMA ganó Nirvana? Wikipedia
    se contradice a sí misma — ¿vos qué encontrás?"
    Una "semilla de duda" vale tanto como un dato confirmado.

15. **Nada de imágenes inventadas.**
    Solo se usan fotos con autor + licencia verificados (Wikimedia Commons).
    Si no hay, se usa un ícono ilustrado. NUNCA una URL inventada,
    NUNCA una licencia supuesta.

16. **Contenido verificado contra fuente.**
    Cada dato del contenido (.md de cada provincia) tiene que poder
    rastrearse a una fuente. Si no se puede verificar, va marcado
    PENDIENTE — no se completa con invento.

17. **Hoja de configuración del sistema (`CONFIG_SISTEMA`).**
    Toda app de este proyecto debe tener un panel de configuración de tema
    accesible desde la interfaz, que permita elegir entre 4 variantes
    de color, de la más clara a la más oscura, incluyendo modo nocturno.

    Reglas de contraste obligatorias:
    - Fondo claro → letras oscuras.
    - Fondo oscuro → letras claras.
    - Mínimo WCAG AA 4.5:1.
    - Si una combinación falla el contraste, no se aplica.

    La preferencia del usuario se guarda en `localStorage` y persiste
    entre sesiones. Si no hay elección previa, arranca con la variante
    por defecto.

18. **Mensajes de familia: contenido intacto, metadata separada.**
    Los mensajes que familiares escriben para Alma (vía Google Form u
    cualquier otro canal) son contenido puro.

    El sistema NUNCA agrega palabras, firma, saludo, emoji ni formato
    dentro del texto del mensaje.

    Toda información agregada por el sistema (autor, fecha, tipo) va en
    un lugar visualmente separado, en letra chica, como metadata.
    El mensaje original se reproduce tal cual fue escrito, sin recortes,
    sin correcciones, sin adornos.

    Por qué: el sentimiento espontáneo es el corazón del mensaje.
    Si el sistema le agrega algo, deja de ser de mamá y pasa a ser de
    la app. Eso no se toca.

---

## NUNCA HAGAS ESTO

- Hardcodear datos sin fuente.
- Inventar URLs de imágenes o licencias.
- Tocar contenido educativo verificado sin pedido explícito.
- Refactorizar sin pedido explícito.
- "Aprovechar" un cambio para limpiar otra cosa.
- Modificar una app hermana del repo para arreglar otra.
- Subir credenciales, PINs o claves a GitHub.
- Cambiar nombres, estructuras o estilos sin necesidad.
- Agregar dependencias innecesarias.
- Reemplazar una solución funcional solo porque exista una más moderna.

---

## FORMA DE TRABAJO

1. Yo pido en criollo.
2. Vos declarás qué tocás y qué NO (REGLA CERO).
3. Yo confirmo.
4. Vos entregás código + backup `_vNNN_backup.html`.
5. Yo pruebo.
6. Si falla → volver atrás, no parchear encima.
7. Una cosa por vez, sin excepciones.

---

## PRIORIDAD ANTE CONFLICTO

1. Solicitud explícita del usuario.
2. Reglas de Oro.
3. Comportamiento funcional existente.
4. Sugerencias o mejoras técnicas de la IA.

Una "mejora técnica" nunca justifica romper una Regla de Oro
ni alterar una función existente que no fue solicitada.

---

## STACK

- Frontend: HTML/CSS/JS puro. Sin backend. Sin build step.
- Deploy: Vercel desde GitHub `almaeggui-bot/alma-puede`.
- Portal: `index.html`.
- Persistencia local: `localStorage`.
- Cuentas: `almaeggui@gmail.com` (GitHub y Vercel).

---

## IDENTIFICACIÓN DE ARCHIVOS

Cada HTML del repo lleva en su cabecera un comentario identificador:

```html
<!--
  Proyecto: Mi regalo para Alma con amor
  Repo: github.com/almaeggui-bot/alma-puede
  Cuenta: almaeggui@gmail.com
  Deploy: alma-puede.vercel.app
  Este archivo NO pertenece a VAO Sistemas.
-->
