# CONTRASTES TV — Skills de periodismo digital

Kit de **skills para agentes de IA** (Claude Code, Codex y compatibles con el formato `SKILL.md`) pensado para que la redacción de **Contrastes TV** produzca más rápido, con rigor periodístico, y posicione la marca en redes sociales y buscadores.

> Una skill es un manual de procedimiento que el agente carga solo cuando la tarea lo necesita. Cada una vive en `.claude/skills/<nombre>/SKILL.md`.

## Qué incluye

| Área | Skill | Para qué sirve |
|---|---|---|
| Marca | [`voz-de-marca`](.claude/skills/voz-de-marca/SKILL.md) | Manual de estilo y tono de Contrastes TV. Base de todas las demás. |
| Marca | [`estrategia-de-marca`](.claude/skills/estrategia-de-marca/SKILL.md) | Plan de posicionamiento de 90 días en web y redes. |
| Rigor | [`verificacion-fact-checking`](.claude/skills/verificacion-fact-checking/SKILL.md) | Verificar datos, imágenes, videos y declaraciones antes de publicar. |
| Rigor | [`etica-y-derechos`](.claude/skills/etica-y-derechos/SKILL.md) | Ética, derechos de autor, privacidad, menores, rectificaciones. |
| Web | [`redaccion-seo-noticias`](.claude/skills/redaccion-seo-noticias/SKILL.md) | Notas optimizadas para Google, Google News y Discover. |
| Web | [`titulares-y-ganchos`](.claude/skills/titulares-y-ganchos/SKILL.md) | Titulares, copys y miniaturas que atraen sin clickbait. |
| Web | [`ultima-hora`](.claude/skills/ultima-hora/SKILL.md) | Protocolo de noticias de último momento (breaking news). |
| Web | [`cobertura-en-vivo`](.claude/skills/cobertura-en-vivo/SKILL.md) | Live blogs, transmisiones y coberturas especiales. |
| Video | [`guion-video-vertical`](.claude/skills/guion-video-vertical/SKILL.md) | Guiones para TikTok, Reels y YouTube Shorts. |
| Video | [`guion-noticiero-tv`](.claude/skills/guion-noticiero-tv/SKILL.md) | Escaleta y guion de noticiero y notas de TV. |
| Redes | [`adaptacion-multiplataforma`](.claude/skills/adaptacion-multiplataforma/SKILL.md) | Convertir una noticia en piezas para cada red. |
| Redes | [`comunidad-y-moderacion`](.claude/skills/comunidad-y-moderacion/SKILL.md) | Responder, moderar y gestionar crisis en comentarios. |
| Reportería | [`entrevista-y-reporteria`](.claude/skills/entrevista-y-reporteria/SKILL.md) | Preparar entrevistas, fuentes y pautas de reporteo. |
| Audiencia | [`newsletter-y-whatsapp`](.claude/skills/newsletter-y-whatsapp/SKILL.md) | Newsletter, canal de WhatsApp y Telegram. |
| Gestión | [`calendario-editorial`](.claude/skills/calendario-editorial/SKILL.md) | Planificación semanal y mensual de contenidos. |
| Gestión | [`analitica-y-kpis`](.claude/skills/analitica-y-kpis/SKILL.md) | Medir, interpretar métricas y decidir qué ajustar. |

## Cómo usarlo

1. **Completa la ficha de marca** en [`CLAUDE.md`](CLAUDE.md) (país, audiencia, redes, horarios). Los campos marcados `[COMPLETAR]` mejoran todos los resultados.
2. Abre la carpeta con Claude Code (`claude`) y pide tareas en lenguaje natural. Ejemplos:
   - «Tengo este comunicado del municipio, conviértelo en nota SEO y en un Reel».
   - «Verifica este video que circula en WhatsApp antes de publicarlo».
   - «Arma el calendario editorial de la próxima semana».
   - «Hay un sismo en este momento, activa el protocolo de última hora».
3. El agente elige la skill adecuada. También puedes nombrarla: «usa la skill `titulares-y-ganchos`».

### Con Codex u otros agentes

El archivo [`AGENTS.md`](AGENTS.md) indica a otros agentes dónde están las skills. Si tu herramienta usa otra carpeta, copia `.claude/skills/` a la ruta que corresponda.

## Flujo de trabajo recomendado

```
Información en bruto
   │
   ├─► verificacion-fact-checking ──► ¿se sostiene? ──no──► no se publica / se aclara
   │                                        │ sí
   ▼                                        ▼
redaccion-seo-noticias  +  titulares-y-ganchos   (pieza madre en la web)
   │
   ▼
adaptacion-multiplataforma ──► guion-video-vertical / X / IG / FB / WhatsApp
   │
   ▼
comunidad-y-moderacion  ──►  analitica-y-kpis  ──►  calendario-editorial (se ajusta)
```

**Regla de oro:** la web es la casa; las redes son la vitrina. Todo contenido de redes debe llevar a la marca y, cuando se pueda, al sitio.

## Estructura

```
contrastes-tv/
├── README.md          ← este archivo
├── CLAUDE.md          ← ficha de marca y reglas globales (léelo primero)
├── AGENTS.md          ← puntero para Codex y otros agentes
└── .claude/skills/    ← 16 skills de periodismo digital
```

## Licencia y uso

Material de trabajo interno de Contrastes TV. Las skills son guías editoriales: **la responsabilidad final de lo publicado siempre es de una persona editora**.
