
# 🧩 Skills de lu4t

Colección de skills para asistentes de inteligencia artificial que amplían sus capacidades mediante instrucciones especializadas.

Los skills de este repositorio siguen el estándar [Agent Skills](https://agentskills.io/) y pueden instalarse en clientes compatibles mediante [skills.sh](https://skills.sh/).

---

## 🔥 frieme

**Pon tus ideas a prueba antes de llevarlas a la práctica.**

`frieme` convierte a tu asistente de IA en un entrevistador crítico que cuestiona tus ideas, planes y decisiones para ayudarte a identificar errores, riesgos, contradicciones y alternativas que quizá no hayas considerado.

No se limita a darte la razón ni a hacerte preguntas genéricas: analiza tu propuesta, recomienda soluciones y también cuestiona sus propias recomendaciones.

Su objetivo no es hacerte más preguntas, sino **hacerte las preguntas que realmente importan**.

### ✨ Características principales

- 🧠 **Pensamiento crítico:** identifica suposiciones débiles, riesgos ocultos y contradicciones.
- 🌳 **Árbol de decisiones:** organiza las decisiones según sus dependencias y evita preguntas prematuras.
- 💬 **Entrevistas por rondas:** plantea un máximo de tres preguntas a la vez para facilitar la conversación.
- ⚖️ **Recomendaciones con contraargumentos:** propone soluciones razonadas y presenta sus posibles debilidades.
- 🔍 **Investigación autónoma:** comprueba hechos utilizando las herramientas disponibles, sin delegar innecesariamente ese trabajo en el usuario.
- 🔄 **Revisión de decisiones:** actualiza el análisis cuando aparecen nuevas respuestas o contradicciones.
- 🎯 **Priorización inteligente:** se concentra en las decisiones con mayor impacto.
- 🏁 **Conclusiones prácticas:** termina cuando existe suficiente claridad para avanzar, evitando entrevistas interminables.

### 📦 Instalación

Desde la raíz del proyecto donde quieras utilizarlo:

    npx skills add lu4t/skills --skill frieme

El instalador te permitirá seleccionar los agentes compatibles.

Por defecto, la instalación es local al proyecto. No necesitas instalarlo globalmente.

Para consultar los skills disponibles en el repositorio:

    npx skills add lu4t/skills --list

### 🚀 Cómo utilizarlo

Una vez instalado, puedes activar el skill con expresiones como:

- "Fríeme esta idea: quiero crear una aplicación para..."
- "Pon a prueba mi plan de negocio."
- "Cuestiona la arquitectura que he diseñado."
- "Hazme preguntas difíciles sobre esta decisión."
- "Busca los puntos débiles de mi estrategia."
- "Desmonta mi propuesta antes de implementarla."

**Ejemplo de uso:**

> **Usuario:** Fríeme esta idea: quiero construir una aplicación SaaS para pequeños restaurantes.

El asistente examinará aspectos importantes como el problema que resuelve el producto, el público objetivo, la viabilidad comercial, las alternativas y los principales riesgos.

En lugar de hacerte veinte preguntas de golpe, seleccionará las tres más relevantes, aportará sus recomendaciones y contraargumentos, y esperará tus respuestas antes de continuar.

### 💡 ¿En qué se diferencia de una conversación normal?

| Conversación habitual | Con frieme |
|---|---|
| Responde a tu propuesta | Cuestiona tus premisas |
| Puede asumir requisitos | Detecta decisiones pendientes |
| Tiende a explorar linealmente | Organiza dependencias |
| Puede hacer demasiadas preguntas | Máximo tres por ronda |
| Propone recomendaciones | También las pone en duda |
| Busca completar la tarea | Busca mejorar la decisión |

---

## 🌱 Origen e inspiración

`frieme` está inspirado en **[grill-me, de Matt Pocock](https://github.com/mattpocock/skills/tree/main/skills/productivity/grill-me)**.

El skill original propone someter las ideas y decisiones del usuario a un interrogatorio riguroso mediante un árbol de decisiones, avanzando por rondas según las dependencias entre preguntas.

`frieme` nace como una evolución de ese planteamiento, manteniendo sus principios fundamentales e incorporando mejoras orientadas a conseguir entrevistas más ágiles, críticas y útiles.

### ¿Qué aporta frieme respecto a grill-me?

**1. Menos preguntas, mejor seleccionadas**

En lugar de plantear todas las preguntas disponibles en cada ronda, `frieme` limita las entrevistas a un máximo de tres preguntas, priorizando las decisiones con mayor impacto.

**2. Priorización en lugar de exhaustividad**

No pretende explorar todas las ramas posibles del árbol. Se concentra en las decisiones que realmente pueden cambiar el resultado.

**3. Recomendaciones con contraargumentos**

El asistente no solo propone una respuesta: también identifica sus debilidades y presenta las alternativas más relevantes.

**4. Detección y resolución de contradicciones**

Cuando aparece información incompatible con decisiones anteriores, `frieme` identifica el conflicto y revisa las ramas afectadas.

**5. Profundidad adaptativa**

La intensidad del interrogatorio se ajusta a la complejidad del problema, la importancia de las decisiones y las preferencias del usuario.

**6. Finalización basada en la utilidad**

La entrevista termina cuando las decisiones importantes están suficientemente resueltas, los riesgos son conocidos y seguir preguntando aporta poco valor.

### Reconocimiento al trabajo original

La idea original y los conceptos de árbol de decisiones, frontera de preguntas y entrevistas por rondas proceden de `grill-me`, creado por **Matt Pocock**.

`frieme` es una adaptación y evolución independiente de ese enfoque, sin afiliación oficial con el proyecto original.

Agradecimiento a Matt Pocock por compartir públicamente su trabajo y servir de inspiración para esta versión.

**Proyecto original:** [mattpocock/skills — grill-me](https://github.com/mattpocock/skills/tree/main/skills/productivity/grill-me)

**Licencia del proyecto original:** [MIT License](https://github.com/mattpocock/skills/blob/main/LICENSE)

Copyright (c) 2026 Matt Pocock.

La licencia MIT del proyecto original permite su modificación y redistribución, siempre que se conserven los avisos de copyright y licencia aplicables.

---

## 🔒 Seguridad

`frieme` ha superado las auditorías automatizadas de seguridad de los tres proveedores integrados en skills.sh:

- ✅ **Gen Agent Trust Hub** — PASS
- ✅ **Socket** — PASS
- ✅ **Snyk** — PASS

Estas evaluaciones no garantizan la ausencia total de riesgos de seguridad.

Puedes consultar la ficha pública y los resultados actualizados de las auditorías aquí:

**[frieme en skills.sh](https://skills.sh/lu4t/skills/frieme)**

---

## 🖥️ Compatibilidad

Los skills de este repositorio están diseñados para clientes compatibles con el estándar Agent Skills.

Entre los clientes que pueden utilizarlos se encuentran:

- Cursor
- Claude Code
- Codex
- GitHub Copilot
- Gemini CLI
- OpenCode

La compatibilidad y el modo de activación pueden variar según el cliente y su versión.

---

## 📁 Estructura del repositorio

Cada skill dispone de su propia carpeta y un archivo `SKILL.md` con sus metadatos e instrucciones.

    skills/
    ├── README.md
    └── frieme/
        └── SKILL.md

Esta estructura permite incorporar nuevos skills en el futuro manteniendo una organización sencilla.

### Código fuente

[Consultar las instrucciones de frieme](./frieme/SKILL.md)

---

## 📚 Recursos

- [Agent Skills — Especificación](https://agentskills.io/)
- [skills.sh — Directorio e instalador](https://skills.sh/)
- [frieme — Ficha pública](https://skills.sh/lu4t/skills/frieme)
- [grill-me — Skill original de Matt Pocock](https://github.com/mattpocock/skills/tree/main/skills/productivity/grill-me)

---

**Un buen asistente no siempre debe darte la razón. A veces, su mayor valor es hacerte cambiar de opinión.**

🔥 **frieme — Menos preguntas. Más pensamiento crítico. Mejores decisiones.**


