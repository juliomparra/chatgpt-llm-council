# Inspección y decisiones de adaptación

Este documento conserva el registro de inspección y las decisiones de la edición 0.1. Para el diseño vigente de Consejo de Decisión, edición 0.2, consulta [METODOLOGIA.md](METODOLOGIA.md). La consulta del origen es parte de la historia de este proyecto; no se oculta ni se presenta la reescritura como un desarrollo sin antecedentes.

Se inspeccionaron README.md y SKILL.md del commit `55ee36e89e0f3f780099ac50332fbb3ec8d14738` mediante el conector de GitHub. El intento de clonar por Git falló por conectividad; no se ejecutó código del repositorio. La carpeta raíz listada por GitHub solo contiene esos dos archivos: no hay aplicación, dependencias, scripts ni pruebas automatizadas.

El README presenta una skill para Claude Code y Claude Cowork. SKILL.md propone recopilar contexto local, convocar cinco asesores mediante subagentes, etiquetar y reordenar respuestas para cinco revisores nuevos y producir una síntesis. Es una adaptación con diferentes enfoques dentro de Claude, no el sistema multimodelo al que alude como inspiración.

| Aspecto | Decisión para esta adaptación |
| --- | --- |
| Cinco enfoques | Conservar crítica, primeros principios, oportunidades, mirada externa y ejecución. |
| Subagentes obligatorios | Modo simulado por defecto; modo real solo con herramientas y autorización vigentes. |
| Contexto local automático | Utilizar fuentes realmente accesibles y pertinentes, sin presumir acceso al equipo. |
| Independencia y anonimización | Declarar las limitaciones de una simulación y de los contextos compartidos. |
| Revisión y síntesis | Mantener ambas rondas y conservar los desacuerdos sustanciales. |
| Certeza por consenso | Vincular confianza a evidencia y reconocer sesgos correlacionados. |
| Entrega | Elegir chat como salida principal. El original prohíbe HTML en un paso, pero vuelve a pedirlo en sus notas finales. |
| Persistencia | Guardar solo a petición en el destino autorizado. |
| Instalación | Ofrecer instrucciones copiables para ChatGPT sin modificar configuración global. |
| Créditos | Mantener la cadena de atribución y registrar la ausencia de licencia. |

La guía de uso con proyectos se contrastó con la [documentación oficial de OpenAI](https://learn.chatgpt.com/docs/projects), consultada el 2026-09-23. No se presupone un plan, un modelo concreto ni acceso a herramientas específicas.

Véanse los enlaces permanentes del código de origen en [ATTRIBUTION.md](../ATTRIBUTION.md).
