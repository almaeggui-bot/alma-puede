═══════════════════════════════════════════════════
CHANCE LOG — 12/09/2026 (TARDE) — MARCO + TAREA MENSAJES
═══════════════════════════════════════════════════

## SESIÓN 1 — MARCO DEL PROYECTO CERRADO

**QUÉ:**
Se cerró el marco de trabajo del proyecto "Mi regalo para Alma con
amor". Los archivos `CLAUDE_ALMA.md` y `CHANCE_LOG_ALMA.md` quedaron
completos, en la raíz del repo `almaeggui-bot/alma-puede`, con:

- Las Reglas de Oro de VAO aplicadas enteras (sin recortes).
- Tres reglas propias del proyecto Alma: sentido crítico, nada de
  imágenes inventadas, contenido verificado contra fuente.
- Regla 18 nueva: mensajes de familia = contenido intacto + metadata
  separada.
- Estado actual del repo documentado (inventario de archivos,
  pendientes, formato viejo de versión detectado).
- Tarea 1 registrada (mensajes de mamá como premio).

**POR QUÉ:**
El proyecto venía creciendo sin marco escrito. Cada sesión con IA
reinventaba reglas, se perdía contexto, y había riesgo de mezclar
archivos de este proyecto con los de VAO Sistemas.

**CÓMO:**
- Se decidió que este proyecto se trata con la misma seriedad que
  VAO POS/SmartPOS: mismas Reglas de Oro, misma forma de trabajo,
  mismo formato de CHANCE LOG.
- Se separó identidad: repo propio (`almaeggui-bot/alma-puede`),
  cuentas propias (`almaeggui@gmail.com`), URL propia
  (`alma-puede.vercel.app`), numeración propia.
- Cada HTML del repo llevará cabecera identificadora:
  Proyecto + repo + cuenta + deploy + "NO pertenece a VAO Sistemas".

**DÓNDE:**
- `CLAUDE_ALMA.md` (raíz del repo).
- `CHANCE_LOG_ALMA.md` (raíz del repo).

**PROBLEMA QUE EVITA O RESUELVE:**
- Pérdida de reglas entre sesiones.
- IA inventando marcos distintos cada vez.
- Confusión con archivos de VAO Sistemas.
- No tener un lugar único para las decisiones del proyecto.

**SI SE ROMPE:**
Los archivos son texto plano. Están en GitHub + backup local.
Se pueden reconstruir desde este mismo CHANCE LOG.

**PENDIENTE:**
- Renombrar `aprende-argentina_v1_backup.html` a formato `_vNNN`.
- Decidir qué hacer con `índice.html` e `índice_v1_backup.html`.
- Limpiar versiones `-v1.x` de `sumas-multiplicacion-alma`.
- Cargar segunda provincia.
- Reemplazar mapa esquemático por bordes geográficos reales.
- Agregar imágenes verificadas a las maravillas que usan ícono.

───────────────────────────────────────────────────

## SESIÓN 2 — TAREA 1 REGISTRADA: MENSAJES DE MAMÁ COMO PREMIO

**QUÉ:**
Se diseñó y registró como tarea pendiente el sistema "Mensajes de
mamá como premio al esfuerzo". Consiste en un botón en el POS de
mamá (Naturaleza Ilustrada v449) que abre un Google Form en pestaña
nueva de Chrome. Mamá escribe lo que siente. El Form escribe directo
en la hoja `Notas` de la planilla "Alma progreso". La app de Alma
lee esa hoja y le muestra los mensajes como premio al esfuerzo.

**POR QUÉ:**
- Dar recompensa emocional real al esfuerzo de Alma. No puntos
  abstractos: palabras de su mamá.
- La espontaneidad es clave. Si mamá tiene que cambiar de contexto,
  loguearse o seguir un formato, se le pasa la idea.
- Alma tiene que saber que los mensajes son de mamá. Pero el texto
  queda 100% intacto, sin firma automática ni adornos del sistema.

**CÓMO:**
Se eligió **Opción B (Google Form)** sobre Opción A (integrar dentro
del POS vía GAS). Razones:
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

**DÓNDE:**
- Ficha completa: ver "TAREAS PENDIENTES DE EJECUCIÓN → Tarea 1".
- Regla aplicable: `CLAUDE_ALMA.md` → Regla 18.

**PROBLEMA QUE EVITA O RESUELVE:**
- Da sentido emocional al proyecto más allá del contenido educativo.
- Puente entre el trabajo de mamá (POS) y el proyecto de Alma
  (app educativa).
- No abre huecos de seguridad entre ecosistemas separados.

**SI SE ROMPE:**
El Form y la planilla son independientes de la app. Si algo falla
en la app, los mensajes quedan guardados igual.

**PENDIENTE:**
Ver ficha completa en Tareas Pendientes → Tarea 1.

═══════════════════════════════════════════════════
FIN DE LA SESIÓN — 12/09/2026 (tarde)
═══════════════════════════════════════════════════