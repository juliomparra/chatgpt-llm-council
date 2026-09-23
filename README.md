# Consejo de Decisión
### Versión en español para GPT

Una skill para convertir una decisión difícil en una elección argumentada, una prueba pequeña y una regla para revisar el resultado.

**Nombre del repositorio:** `chatgpt-llm-council` · **Edición:** 0.2 · **Estado:** experimental.

Esta versión conserva la idea de un consejo de perspectivas y revisión cruzada, con redacción, enfoques y procedimiento propios. Está inspirada en [aiwithremy/claude-skills-llm-council](https://github.com/aiwithremy/claude-skills-llm-council), cuyo README acredita a [Ole Lehmann](https://x.com/itsolelehmann) y a la metodología [LLM Council de Andrej Karpathy](https://github.com/karpathy/llm-council). Las fuentes de inspiración no son responsables de esta edición.

## Qué aporta esta versión

- Una ficha con objetivos, restricciones, alternativas y datos faltantes.
- Cinco enfoques: evidencia, valor, impacto humano, viabilidad y reversibilidad.
- Revisión circular: cada enfoque cuestiona un informe de otro enfoque.
- Comparación con criterios comunes, sin puntuaciones inventadas.
- Un acta con decisión provisional, objeción pendiente, prueba mínima y regla de revisión.

La finalidad es hacer explícito qué justifica una decisión y qué podría cambiarla. Coincidir entre perspectivas no demuestra que la conclusión sea correcta.

## Usarlo en ChatGPT

1. Abre [SKILL.md](SKILL.md).
2. Copia desde el título «Consejo de Decisión», omitiendo el encabezado YAML entre `---`.
3. Pega el contenido en un chat y añade tu decisión, alternativas y restricciones.

Ejemplo de entrada:

> Usa el Consejo de Decisión. Nuestro equipo de cuatro personas pierde tiempo buscando acuerdos. Tenemos seis horas esta semana para mejorar el proceso. ¿Cambiamos de herramienta o probamos una plantilla de decisiones en la actual? Queremos reducir búsquedas sin añadir otra suscripción. No tenemos mediciones todavía.

Para reutilizar las instrucciones puedes incluirlas en un proyecto de ChatGPT junto con sus fuentes pertinentes. Un proyecto de ChatGPT no proporciona por sí mismo acceso a esta carpeta local. Consulta la [guía oficial de proyectos](https://learn.chatgpt.com/docs/projects).

También puedes adjuntar SKILL.md y pedir que se lea y aplique; adjuntarlo no garantiza su instalación ni su activación. En un entorno compatible con skills, el identificador sigue siendo `chatgpt-llm-council`. Esta carpeta contiene la skill portable; no instala configuración global ni constituye todavía un plugin empaquetado.

## Cómo se presenta el resultado

El acta muestra una decisión provisional, una tabla comparativa, la objeción principal aún abierta y una prueba con una condición para revisar la decisión. Puedes solicitar los cinco informes y sus revisiones para ver el detalle.

El modo habitual es **simulado: un mismo asistente representa cinco enfoques**. El modo con agentes reales solo se usa si existen herramientas y autorización para delegar. No se prometen cinco modelos distintos ni revisión ciega.

## Contenido

| Archivo | Uso |
| --- | --- |
| [SKILL.md](SKILL.md) | Instrucciones completas, en español por defecto. |
| [docs/METODOLOGIA.md](docs/METODOLOGIA.md) | Diseño de esta versión y diferencias respecto de la inspiración. |
| [examples/decisiones.md](examples/decisiones.md) | Ejemplo desarrollado y entradas de prueba. |
| [docs/VALIDACION.md](docs/VALIDACION.md) | Comprobaciones realizadas y evaluación pendiente. |
| [docs/INSPECCION.md](docs/INSPECCION.md) | Registro de inspección del origen. |
| [ATTRIBUTION.md](ATTRIBUTION.md) | Créditos, procedencia y estado de licencia. |
| [CHANGELOG.md](CHANGELOG.md) | Cambios entre ediciones. |

## Autoría y procedencia

La redacción y las decisiones de diseño de esta edición se desarrollaron para este proyecto con asistencia de Codex. Se conservan las fuentes de inspiración y no se presenta como una creación sin antecedentes, traducción oficial o producto avalado por OpenAI.

El repositorio de origen inspeccionado no incluía licencia expresa. Esta edición no declara una licencia sobre contenido de terceros; su rediseño no certifica por sí solo la situación de derechos. Véase [ATTRIBUTION.md](ATTRIBUTION.md). Su distribución como repositorio no implica instalación ni disponibilidad en el directorio de plugins.
