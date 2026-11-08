---
name: verificacion-fact-checking
description: Protocolo de verificación de información, imágenes, videos, audios, cifras y declaraciones antes de publicar. Úsala cuando haya contenido viral, material enviado por la audiencia, capturas, cadenas de WhatsApp, cifras de terceros, o cuando pidan "verificar", "chequear", "¿es real?", "fact-check" o "desmentir".
---

# Verificación y fact-checking

**Principio:** es mejor llegar segundo con la verdad que primero con un error. Un error viral destruye en horas la credibilidad que la marca construye en años.

## Paso 1 — Clasificar la pieza

| Tipo | Riesgo típico |
|---|---|
| Declaración / cita | Sacada de contexto, inventada, mal atribuida |
| Cifra / estadística | Desactualizada, mal calculada, fuente sesgada |
| Imagen | Vieja, de otro lugar, editada o generada por IA |
| Video | Recortado, de otro evento, deepfake, audio cambiado |
| Audio / nota de voz | Voz clonada, sin origen identificable |
| Documento / captura | Falsificado, editado, parcial |
| Rumor / cadena | Sin fuente identificable |

## Paso 2 — Preguntas básicas (las 5 del verificador)

1. **Origen:** ¿quién lo creó o lo publicó primero? Buscar la publicación más antigua.
2. **Fuente:** ¿quién lo dice y qué interés tiene? ¿Es fuente primaria o secundaria?
3. **Fecha:** ¿cuándo se creó? ¿Coincide con el evento que dice mostrar?
4. **Lugar:** ¿dónde se capturó? ¿Los elementos visuales coinciden (carteles, clima, arquitectura, vehículos, idioma)?
5. **Motivación:** ¿por qué circula ahora? ¿A quién beneficia?

## Paso 3 — Técnicas por tipo

### Imágenes
- Búsqueda inversa en varias herramientas (Google Lens, TinEye, Bing Visual, Yandex).
- Revisar metadatos (EXIF) si se tiene el archivo original; recordar que las redes los borran.
- Buscar señales de edición o IA: manos, textos ilegibles, sombras incoherentes, reflejos, bordes.
- Geolocalizar con mapas y vista de calle comparando puntos de referencia.

### Videos
- Extraer fotogramas clave y hacer búsqueda inversa de cada uno.
- Contrastar con otros ángulos del mismo evento.
- Verificar clima y hora (sombras) con registros históricos.
- En audio, sospechar de sincronía labial imperfecta o tono plano (posible clonación).

### Cifras
- Ir siempre a la **fuente primaria** (organismo oficial, estudio original, base de datos).
- Comprobar año, unidad, base (¿porcentaje de qué?) y metodología.
- Recalcular variaciones porcentuales: `(nuevo − anterior) / anterior × 100`.
- Comparar con al menos otra fuente independiente.

### Declaraciones
- Buscar el video o audio completo, no solo el recorte.
- Confirmar con la persona o su equipo cuando sea posible.
- Ver la cita en su contexto anterior y posterior.

### Documentos
- Verificar formato, sellos, firmas y numeración con documentos auténticos del mismo emisor.
- Consultar directamente al emisor.

## Paso 4 — Dictamen

Asigna una de estas etiquetas y justifícala:

| Etiqueta | Criterio |
|---|---|
| ✅ **Verdadero** | Confirmado por fuente primaria o dos fuentes independientes fiables. |
| 🟡 **Engañoso** | Contiene algo real pero sacado de contexto, exagerado o incompleto. |
| ❌ **Falso** | Las pruebas lo contradicen. |
| ⚪ **Sin evidencia** | No se pudo confirmar ni desmentir. No se publica como hecho. |
| 🔄 **En desarrollo** | Hay indicios pero falta confirmación oficial. Se publica solo con advertencia explícita. |

## Paso 5 — Entregable

```
VERIFICACIÓN — [tema]
Pieza analizada: [descripción / enlace]
Dictamen: [etiqueta]
Evidencias:
  1. …
  2. …
Fuentes consultadas: …
Lo que aún no sabemos: …
Recomendación: publicar / publicar con advertencia / no publicar / publicar desmentido
```

## Si se publica un desmentido

- Titular con el dato correcto, no repitiendo el bulo: «El video del puente no es de este año: es de 2019», no «¿Se cayó el puente? Esto es lo que sabemos».
- Mostrar la imagen falsa solo con marca visible de **FALSO** superpuesta.
- Explicar cómo se verificó: genera confianza y educa a la audiencia (es contenido de marca muy valioso).

## Límites del agente

El agente **no puede** acceder por sí solo a herramientas de búsqueda inversa ni confirmar con fuentes humanas si no tiene esas herramientas conectadas. En ese caso, entrega el plan de verificación paso a paso y marca el dictamen como **pendiente**. Nunca declares algo «verificado» sin evidencia concreta.
