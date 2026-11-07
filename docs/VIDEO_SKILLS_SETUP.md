# Instalación de skills audiovisuales — Claude Code y Codex

Este documento prepara la instalación, pero **no instala software en tu computadora**. Revisa el código y los permisos de cada repositorio antes de ejecutar comandos.

## Requisitos
Node.js 20+, npm/npx, Git y, para renderizar, FFmpeg. Algunas skills necesitan Chrome/Chromium, APIs o dependencias adicionales.

## Instalación de colecciones confirmadas

Desde una terminal local, en la carpeta de este proyecto:

```bash
npx skills add remotion-dev/skills -a claude-code -a codex
npx skills add adamperlis/video-skills -a claude-code -a codex
npx skills add Melvynx/video-agent-skills -a claude-code
```

Las instalaciones son interactivas para que puedas revisar qué se incorporará. No utilices opciones que omitan confirmaciones sin auditar el código.

## Colecciones adicionales a revisar

Estas se mencionaron en la conversación, pero **no están auditadas ni verificadas aquí como compatibles con ambos agentes**:

- https://github.com/sfgdfgd/-skill (Video Shotcraft)
- https://github.com/OpenClip-App/agent-skills (OpenClip)
- https://github.com/soumatheusgomes/editonny (Editonny)

Si contienen archivos SKILL.md compatibles, instala selectivamente:

```bash
npx skills add https://github.com/sfgdfgd/-skill
npx skills add https://github.com/OpenClip-App/agent-skills
npx skills add https://github.com/soumatheusgomes/editonny
```

Comprueba primero la legitimidad, requisitos y permisos de cada repositorio. No pegues claves API en GitHub; utiliza variables de entorno y .gitignore.

## Verificación
```bash
npx skills list
```

Reinicia Claude Code o Codex y comprueba que detectan las habilidades. Instalar una skill no instala necesariamente Remotion ni renderiza videos.

## Flujo sugerido
1. Crear composición vertical 1080x1920 con Remotion.
2. Generar animaciones de datos y transiciones.
3. Editar material propio, revisar subtítulos y audio.
4. Renderizar MP4 y revisar calidad antes de publicar.
