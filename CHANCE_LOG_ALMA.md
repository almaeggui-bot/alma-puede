# CHANCE LOG — MI REGALO PARA ALMA CON AMOR

> **Proyecto: "Mi regalo para Alma con amor"**
> Repo: `github.com/almaeggui-bot/alma-puede`
> Cuenta: `almaeggui@gmail.com`
> Deploy: `alma-puede.vercel.app`
>
> **Este proyecto NO pertenece a VAO Sistemas.**

Registro descriptivo de cada sesión de desarrollo.
Formato detallado en `CLAUDE_ALMA.md` → sección "CHANCE LOG".

Propósito:
- Permitir reconstruir funciones complejas desde cero.
- Documentar errores blindados (nunca más sufrir el mismo problema).
- Dejar contexto para futuras IAs y para mí mismo en 3 meses.

═══════════════════════════════════════════════════
CHANCE LOG — HISTORIAL PREVIO (05/09 a 12/09/2026)
═══════════════════════════════════════════════════

Registro reconstruido a partir del estado del repo al 12/09/2026.
Las sesiones previas no se documentaron con este formato en su momento.

## SESIÓN PREVIA 1 — APP DE MATEMÁTICAS (05-07/09/2026)

QUÉ: Se construyó `sumas-multiplicacion-alma.html` (sumas y multiplicaciones).

POR QUÉ: Ejercicios de matemáticas para Alma.

CÓMO: HTML/CSS/JS puro. Iteraciones sucesivas con formato de versión
viejo (`-v1.1` a `-v1.5`), luego corregido a formato correcto
(`_v7_backup`, `_v9_backup`).

DÓNDE: raíz del repo `alma-puede`.

PROBLEMA QUE EVITA O RESUELVE: práctica de matemáticas básicas.

SI SE ROMPE: restaurar desde `sumas-multiplicacion-alma_v9_backup.html`.

PENDIENTE:
- Limpiar los archivos `-v1.1` a `-v1.5` (historia muerta, formato viejo).
- Confirmar que `sumas-multiplicacion-alma.html` es la versión vigente.

───────────────────────────────────────────────────

## SESIÓN PREVIA 2 — APRENDE ARGENTINA v1 (09/09/2026)

QUÉ: Se construyó `aprende-argentina.html` con Río Negro como primera
provincia. Incluye mapa SVG interactivo (24 formas tocables), 5 modos
(Ubicar, Conocer, Jugar, Desafío, Mi progreso), 8 niveles progresivos,
33 preguntas, repetición espaciada real con localStorage, y una única
foto verificada (Centro Cívico de Bariloche, Wikimedia Commons, CC BY-SA).

POR QUÉ: Objetivo del proyecto: desarrollar cultura general argentina
en Alma usando memoria visual, asociación, descubrimiento, repetición
y recuperación activa.

CÓMO: HTML/CSS/JS puro. Sin backend. Sin build step. Fuente de contenido:
`rio-negro.md` (verificado contra Argentina.gob.ar y rionegro.gov.ar).

DÓNDE: raíz del repo.

PROBLEMA QUE EVITA O RESUELVE: arranca el proyecto de cultura general
con una provincia completa y un motor que sirve para las 24.

SI SE ROMPE: restaurar desde `aprende-argentina_v1_backup.html`.

PENDIENTE:
- Renombrar `aprende-argentina_v1_backup.html` a formato `_vNNN`.
- Cargar la segunda provincia.
- Reemplazar el mapa esquemático (grilla) por bordes geográficos reales.

───────────────────────────────────────────────────

## SESIÓN PREVIA 3 — PORTAL (07 y 12/09/2026)

QUÉ: Se crearon `index.html` (07/09, portal oficial que Vercel reconoce)
e `índice.html` (12/09, con backup `índice_v1_backup.html`).

POR QUÉ: Necesidad de una página de entrada al repo con múltiples apps.

CÓMO: HTML puro.

DÓNDE: raíz del repo.

PROBLEMA QUE EVITA O RESUELVE: punto de entrada único para las apps.

SI SE ROMPE: Vercel usa `index.html` automáticamente.

PENDIENTE:
- Decidir qué hacer con `índice.html` y `índice_v1_backup.html`:
  ¿se borran, se renombran, o quedan como página interna?
- Confirmar que `index.html` es el portal oficial y que lista
  todas las apps vigentes del repo.

═══════════════════════════════════════════════════
CHANCE LOG — 12/09/2026 (MAÑANA) — MARCO DEL PROYECTO
═══════════════════════════════════════════════════

## SESIÓN 1 — MARCO DEL PROYECTO CERRADO

QUÉ: Se crearon `CLAUDE_ALMA.md` y `CHANCE_LOG_ALMA.md` en la raíz
del repo. Se fijó el nombre del proyecto: "Mi regalo para Alma con amor".
Se declaró explícitamente que este proyecto NO pertenece a VAO Sistemas.

POR QUÉ: Se decidió darle a este proyecto la misma seriedad y las mismas
Reglas de Oro que a VAO POS/SmartPOS. Sin un marco escrito, cada sesión
con IA reinventaba reglas y se perdía contexto.

CÓMO: Se adaptaron las Reglas de Oro del `PROMPT_MAESTRO.md` de VAO
(corren enteras, sin recortes) y se agregaron reglas propias del
proyecto Alma: sentido crítico, nada de imágenes inventadas, contenido
verificado contra fuente, hoja de configuración del sistema, mensajes
de familia con contenido intacto.

DÓNDE:
- `CLAUDE_ALMA.md` (raíz del repo)
- `CHANCE_LOG_ALMA.md` (raíz del repo)

PROBLEMA QUE EVITA O RESUELVE:
- Pérdida de reglas entre sesiones.
- IA inventando cosas distintas cada vez.
- Confusión con archivos de VAO Sistemas.
- No tener un "lugar único" para las decisiones del proyecto.

SI SE ROMPE: los archivos son texto. Están en GitHub + backup local.

PENDIENTE:
- Renombrar `aprende-argentina_v1_backup.html` a formato `_vNNN`.
- Decidir qué hacer con `índice.html` e `índice_v1_backup.html`.
- Cargar la segunda provincia en `aprende-argentina.html`.
- Reemplazar el mapa esquemático por bordes geográficos reales.
- Agregar imágenes verificadas a las maravillas que hoy usan ícono.

───────────────────────────────────────────────────

## PROBLEMAS ABIERTOS AL CIERRE DE LA MAÑANA (12/09/2026)

1. **Formato viejo de versión en `aprende-argentina_v1_backup.html`.**
   Debería ser `_vNNN_backup` correcto.

2. **Doble portal (`index.html` + `índice.html`).**
   Definir cuál manda y qué pasa con el otro.

3. **Versiones viejas de matemáticas (`-v1.1` a `-v1.5`).**
   Formato prohibido por Regla 1. No se tocan, pero conviene limpiar.

4. **Mapa esquemático (grilla).**
   Funciona, pero no tiene bordes geográficos reales. Reemplazable
   sin tocar el motor.

5. **Imágenes pendientes.**
   Solo una foto verificada (Centro Cívico de Bariloche). El resto
   de maravillas usan ícono.

6. **Segunda provincia.**
   Aún no cargada. `rio-negro.md` es la única fuente base.

═══════════════════════════════════════════════════
CHANCE LOG — 12/09/2026 (TARDE) — MARCO + TAREA MENSAJES
═══════════════════════════════════════════════════

## SESIÓN 1 — MARCO DEL PROYECTO CERRADO (confirmación)

QUÉ: Se confirmó el cierre del marco de trabajo del proyecto. Los
archivos `CLAUDE_ALMA.md` y `CHANCE_LOG_ALMA.md` quedaron completos,
en la raíz del repo, con:

- Las Reglas de Oro de VAO aplicadas enteras (sin recortes).
- Reglas propias del proyecto Alma: sentido crítico, nada de
  imágenes inventadas, contenido verificado contra fuente, hoja de
  configuración del sistema (Regla 17), mensajes de familia con
  contenido intacto (Regla 18).
- Estado actual del repo documentado.
- Tarea 1 registrada (mensajes de mamá como premio).

POR QUÉ: El proyecto venía creciendo sin marco escrito. Cada sesión
con IA reinventaba reglas, se perdía contexto, y había riesgo de
mezclar archivos de este proyecto con los de VAO Sistemas.

CÓMO:
- Se decidió que este proyecto se trata con la misma seriedad que
  VAO POS/SmartPOS: mismas Reglas de Oro, misma forma de trabajo,
  mismo formato de CHANCE LOG.
- Se separó identidad: repo propio (`almaeggui-bot/alma-puede`),
  cuentas propias (`almaeggui@gmail.com`), URL propia
  (`alma-puede.vercel.app`), numeración propia.
- Cada HTML del repo lleva cabecera identificadora:
  Proyecto + repo + cuenta + deploy + "NO pertenece a VAO Sistemas".

DÓNDE:
- `CLAUDE_ALMA.md` (raíz del repo).
- `CHANCE_LOG_ALMA.md` (raíz del repo).

PROBLEMA QUE EVITA O RESUELVE:
- Pérdida de reglas entre sesiones.
- IA inventando marcos distintos cada vez.
- Confusión con archivos de VAO Sistemas.
- No tener un lugar único para las decisiones del proyecto.

SI SE ROMPE: los archivos son texto plano. Están en GitHub + backup
local. Se pueden reconstruir desde este mismo CHANCE LOG.

PENDIENTE:
- Renombrar `aprende-argentina_v1_backup.html` a formato `_vNNN`.
- Decidir qué hacer con `índice.html` e `índice_v1_backup.html`.
- Limpiar versiones `-v1.x` de `sumas-multiplicacion-alma`.
- Cargar segunda provincia.
- Reemplazar mapa esquemático por bordes geográficos reales.
- Agregar imágenes verificadas a las maravillas que usan ícono.

───────────────────────────────────────────────────

## SESIÓN 2 — TAREA 1 REGISTRADA: MENSAJES DE MAMÁ COMO PREMIO

QUÉ: Se diseñó y registró como tarea pendiente el sistema "Mensajes de
mamá como premio al esfuerzo". Consiste en un botón en el POS de mamá
(Naturaleza Ilustrada v449) que abre un Google Form en pestaña nueva
de Chrome. Mamá escribe lo que siente. El Form escribe directo en la
hoja `Notas` de la planilla "Alma progreso". La app de Alma lee esa
hoja y le muestra los mensajes como premio al esfuerzo.

POR QUÉ:
- Dar recompensa emocional real al esfuerzo de Alma. No puntos
  abstractos: palabras de su mamá.
- La espontaneidad es clave. Si mamá tiene que cambiar de contexto,
  loguearse o seguir un formato, se le pasa la idea.
- Alma tiene que saber que los mensajes son de mamá. Pero el texto
  queda 100% intacto, sin firma automática ni adornos del sistema.

CÓMO:
Se eligió Opción B (Google Form) sobre Opción A (integrar dentro del
POS vía GAS). Razones:
- Cero riesgo de seguridad.
- Cero compartir planillas entre ecosistemas.
- Cero código backend nuevo.
- Funciona desde cualquier dispositivo (celular de mamá incluido).
- Respeta las Reglas de Oro sin excepciones.

Mecanismo de rotación de mensajes:
- Cada mensaje arranca con 0 veces mostrado.
- Primero salen los que están en 0 (nunca vistos).
- Después por prioridad (menos veces mostrados primero).
- Azar solo como desempate entre igualados en cantidad de veces.
- Al mostrarse, contador +1.

Metadata separada:
- El texto del mensaje es 100% de mamá.
- El sistema muestra aparte, en letra chica, "De: mamá — fecha".
- El mensaje original nunca se modifica.

DÓNDE:
- Ficha completa: ver "TAREAS PENDIENTES DE EJECUCIÓN → Tarea 1".
- Regla aplicable: `CLAUDE_ALMA.md` → Regla 18.

PROBLEMA QUE EVITA O RESUELVE:
- Da sentido emocional al proyecto más allá del contenido educativo.
- Puente entre el trabajo de mamá (POS) y el proyecto de Alma
  (app educativa).
- No abre huecos de seguridad entre ecosistemas separados.

SI SE ROMPE: El Form y la planilla son independientes de la app.
Si algo falla en la app, los mensajes quedan guardados igual.

PENDIENTE: Ver ficha completa en Tareas Pendientes → Tarea 1.

═══════════════════════════════════════════════════
FIN DE LAS SESIONES — 12/09/2026
═══════════════════════════════════════════════════

═══════════════════════════════════════════════════
TAREAS PENDIENTES DE EJECUCIÓN
═══════════════════════════════════════════════════

## TAREA 1 — MENSAJES DE MAMÁ COMO PREMIO AL ESFUERZO

**Estado:** Pendiente de ejecución.

### QUÉ

Un botón "Mensaje a Alma" en el POS de mamá
(Naturaleza Ilustrada · naturaleza-ilustrada-pos.vercel.app) que abre
un Google Form en pestaña nueva de Chrome. Mamá escribe una palabra
motivadora, anécdota o lo que sienta. El Form escribe directo en la
hoja `Notas` de la planilla "Alma progreso" (cuenta
`almaeggui@gmail.com`).

La app de Alma lee esa hoja y muestra los mensajes como premio al
esfuerzo, no como chat.

### POR QUÉ

Espontaneidad. Si mamá tiene que cambiar de contexto, loguearse en
otro lado o seguir un formato, se le pasa la idea. Un botón, una
pestaña, escribir, enviar.

### CÓMO SE DECIDIÓ

- Opción B (Google Form) elegida sobre Opción A (integrar GAS
  dentro del POS): cero riesgo de seguridad, cero compartir
  planillas, cero código backend nuevo, funciona desde cualquier
  dispositivo.

### CÓMO (diseño de la función)

**Entrada (lado mamá):**
- Botón en su POS → abre Form en pestaña nueva de Chrome.
- Campos del Form:
  - Mensaje (texto, obligatorio).
  - Quién lo manda (opción múltiple: Mamá / Papá / Otro).
  - Tipo (opcional: Motivadora / Anécdota / Chiste).
  - Fecha (automática, la agrega Google Forms).
- Mamá escribe lo que quiere. El texto queda 100% intacto.

**Salida (lado Alma):**
- La app lee la hoja `Notas`.
- Cada mensaje arranca con 0 veces mostrado.
- Orden de aparición:
  1. Primero los que están en 0 (nunca vistos).
  2. Después por prioridad (menos veces mostrados primero).
  3. Azar solo como desempate entre igualados en cantidad de veces.
- Al mostrarse, contador +1.

**Cuándo salta el mensaje:**
- Al superar un desafío (ej: 10 respuestas correctas seguidas).
- Al volver a la app después de X días sin entrar.

**Metadata separada (NO hardcodeada en el texto):**
- El texto del mensaje es 100% de mamá. Sin firma automática.
- El sistema muestra aparte, en letra chica, "De: mamá — 12/09/2026".
- Es un dato, no una firma. El mensaje de adentro queda intacto.

### DÓNDE

- Form: cuenta `almaeggui@gmail.com` (a crear).
- Planilla destino: "Alma progreso" → hoja `Notas` (ya existe).
- App destino: `aprende-argentina.html` (o `index.html` del repo).
- Botón origen: POS Naturaleza Ilustrada v449 (mamá).

### PROBLEMA QUE EVITA O RESUELVE

- Da recompensa emocional real al esfuerzo de Alma (no puntos
  abstractos: palabras de su mamá).
- No rompe la espontaneidad del mensaje.
- No requiere backend nuevo, ni compartir planillas, ni tocar GAS.

### SI SE ROMPE

El Form y la planilla son independientes. Si algo falla en la app,
los mensajes ya quedaron guardados igual.

### PENDIENTE

- Crear el Form.
- Agregar campos "Quién lo manda" y "Tipo" a la hoja `Notas`
  (hoy tiene solo una columna de texto).
- Agregar columna "veces_mostrado" a la hoja `Notas`.
- Crear el botón en el POS de Naturaleza Ilustrada.
- Agregar la lógica de lectura + rotación en la app de Alma.
- Decidir exactamente en qué momentos salta (desafío / días sin
  entrar / los dos).

═══════════════════════════════════════════════════
FIN DE TAREAS PENDIENTES — 12/09/2026
═══════════════════════════════════════════════════
