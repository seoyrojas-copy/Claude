# VoC — Intento adicional: Quora, YouTube y alternativa (Hacker News)

> Tercera ronda de investigación sobre "la IA no escribe como un humano", tras dos Deep Research previas (GPT y Gemini) que no consiguieron nada verificable en Quora ni YouTube.
> **Resultado de esta ronda: Quora y YouTube siguen bloqueados, igual que antes.** Se amplió a Hacker News (vía API de Algolia + páginas individuales de `news.ycombinator.com`), que sí es accesible y dio hallazgos nuevos.
> Clasificación: **[NEGOCIO]** = uso laboral/negocio · **[PERSONAL]** = uso personal · **[INDETERMINADO]** = no se puede saber · **[BAJA CONFIANZA TÉCNICA]** = la voz suena a alguien con poca soltura técnica.
> Aviso importante sobre esta fuente: Hacker News es una comunidad de perfil muy técnico (desarrolladores, fundadores de startups). Por tanto casi ninguna cita aquí lleva **[BAJA CONFIANZA TÉCNICA]** — es el sesgo esperado de esta plataforma, útil como contraste pero no representativo del target final (35-60 años, no-técnicos). Se señala explícitamente en cada entrada cuando el autor revela perfil técnico.

---

## Bloque 0 — Qué se intentó y qué falló (reporte de bloqueo, sin fabricar nada)

### QUORA — BLOQUEADO (igual que las rondas anteriores)
- `WebSearch` con `site:quora.com` + variantes en inglés ("sounds like AI", "sounds robotic", "ChatGPT doesn't sound like me", "ashamed AI wrote this") **nunca devolvió una sola URL de quora.com** en los resultados; el propio motor de búsqueda reconoce explícitamente en varias respuestas que el operador `site:` no se aplicó.
- Variantes sin `site:` (p. ej. `quora "How do I make ChatGPT write like a human"`, `quora.com answer "sounds like ChatGPT" embarrassing`) tampoco devolvieron ninguna URL de Quora, solo blogs/SEO sobre el mismo tema.
- Intento de `WebFetch` directo sobre `https://www.quora.com/search?q=...`: **HTTP 403 Forbidden**. No se insistió más (según la instrucción de no repetir más de 2-3 veces).
- **Conclusión: Quora no dio ningún hallazgo verificable, ni por búsqueda ni por fetch directo. Mismo resultado que las dos investigaciones Deep Research previas.**

### YOUTUBE — BLOQUEADO (igual que las rondas anteriores)
- `WebSearch` con `site:youtube.com` + variantes ("make chatgpt sound human", "AI writing sounds robotic", tutoriales en español) **no devolvió ninguna URL de youtube.com/watch**; el motor confirma que el filtro `site:` no se aplicó y solo trae blogs/SEO.
- No se encontró ninguna URL de vídeo de YouTube concreta y verificable sobre la que intentar `WebFetch` para extraer comentarios (el método pedía intentarlo solo *si* aparecía una URL de vídeo relevante).
- **Conclusión: no se pudo ni siquiera llegar a la fase de pedir comentarios a un vídeo concreto, porque no se obtuvo ninguna URL de YouTube utilizable. Mismo bloqueo que las dos rondas anteriores — ningún comentario de YouTube en este documento, ninguno inventado.**

### HACKER NEWS — SÍ FUNCIONÓ (fuente alternativa)
- El operador `site:news.ycombinator.com` en `WebSearch` tampoco se aplicó de forma fiable (mismo problema que con Quora/YouTube), pero **la API pública de Algolia para HN (`hn.algolia.com/api/v1/search`) sí es accesible vía `WebFetch`** y devuelve resultados reales con `comment_id`/`story_id` verificables, y cada comentario se pudo confirmar visitando `news.ycombinator.com/item?id=...` directamente.
- Esto permitió encontrar varios hilos reales con quejas sobre texto que "suena a IA", detectores de IA que marcan texto humano, y frustración por escritura robótica.

---

## Bloque 1 — Hallazgos verificados en Hacker News

### Hacker News — comentario personal sobre su propia escritura marcada como IA por GPTZero — [PERSONAL] [BAJA CONFIANZA TÉCNICA: no aplica, es ingeniero, pero el detalle es muy humano/no-técnico]
> "My writing tends to be quite dry to the extent that GPTzero flagged it as written by AI" — el motivo que dio la herramienta fue "the lack of a creative use of grammar". En el mismo comentario admite que admira el estilo de Roger Ebert y le gustaría escribir así.
Fuente: https://news.ycombinator.com/item?id=46936833

### Hacker News — colegas de trabajo marcados en bloque como "100% IA" sin haber usado IA — [NEGOCIO]
> "Tools like GPTzero are incredibly unreliable." / "Me and plenty of my colleagues often get our writing flagged as 100% AI by these tools, when no AI was used."
Fuente: https://news.ycombinator.com/item?id=46184015

### Hacker News — detector marca como IA textos escritos antes de que la IA generativa existiera — [PERSONAL/INDETERMINADO]
> "I tried it on several texts & messages I wrote before 2019, and it flagged them as 80% AI-generated." (usado como prueba de que estos detectores producen más falsos positivos que aciertos)
Fuente: https://news.ycombinator.com/item?id=49155118

### Hacker News — le dijeron directamente que su estilo de escritura suena a IA generada — [NEGOCIO] (autor es desarrollador, reacciona construyendo una skill de IA)
> [PARÁFRASIS, no literal] Cuenta que alguien le comentó que su forma de escribir "sounds like AI generated text"; en vez de tomárselo solo como crítica, decidió que si la gente imita el estilo de la IA que lee, él podía invertir el proceso y creó una skill que transforma la salida del modelo a un estilo isabelino/Shakespeare, presentándolo medio en broma como "lifehack".
Fuente: https://news.ycombinator.com/item?id=49737133

### Hacker News — hija le dice a su padre que toda su escritura "suena a IA" desde hace 30 años — [PERSONAL]
> "My daughter feels all my writing naturally sounds like AI." / "Maybe author has similar issue?"
> [contexto, paráfrasis] Explica que su hija incluye en esa acusación incluso sus trabajos universitarios de hace 30 años, es decir, textos escritos mucho antes de que existiera la IA generativa.
Fuente: https://news.ycombinator.com/item?id=45600383 (hilo: "I almost got hacked by a 'job interview'")

### Hacker News — respuesta a la anterior: a él también le dicen que suena a IA por ser "demasiado entusiasta" — [PERSONAL]
> [PARÁFRASIS, no literal] johnisgood responde que a él también le han dicho que suena a IA por ser demasiado serio, entusiasta o friki con ciertos temas, y reconoce que muchos de sus comentarios son de "bajo esfuerzo".
Fuente: https://news.ycombinator.com/item?id=45600383

### Hacker News — queja viva sobre el tono de ChatGPT en sí mismo, no solo de textos generados — [PERSONAL/INDETERMINADO]
> "The single biggest issue for me with ChatGPT right now is how absolutely awful it sounds in every answer." (menciona muletillas recurrentes como "Why it matters" y "the big picture", y se pregunta si ese estilo es intencionado para poder identificar contenido de ChatGPT en la web)
Fuente: https://brianlovin.com/hn/47236169 [BAJA CONFIANZA TÉCNICA: no aplica — comunidad técnica, pero la queja en sí (el tono le "parece horrible") es emocional y no técnica]

### Hacker News — "esto es basura de IA" dicho directamente sobre un artículo — [INDETERMINADO]
> "This is AI slop."
Fuente: https://news.ycombinator.com/item?id=50177364

### Hacker News — queja sobre redacción confusa que "suena a IA incoherente" — [INDETERMINADO]
> "sounds like incoherent AI writing" (se queja de que la redacción de un artículo es confusa y atribuye esa confusión a estar escrita por IA)
Fuente: https://news.ycombinator.com/item?id=50180887

### Hacker News — frustración al escribir copy de landing page que "suena a vómito de robot" — [NEGOCIO]
> "Sunday: Writing landing page copy that sounds like robot vomit." (parte de un relato de varios días de frustración intentando crear materiales de marketing, antes de construir su propia herramienta de IA para resolverlo)
Fuente: https://news.ycombinator.com/item?id=44733188

### Hacker News — defensa de que escribir "como se nota que es IA" sigue siendo mala escritura, venga de donde venga — [INDETERMINADO]
> "If you wrote it 100% by hand and it still sounds like AI, it's still bad writing"
Fuente: https://news.ycombinator.com/item?id=47006013

### Hacker News — acusación directa y cruda a otro usuario sobre su forma de escribir — [INDETERMINADO]
> "Your writing sounds like fuckin' AI, so I wouldn't complain if I were you."
Fuente: https://news.ycombinator.com/item?id=46385779

### Hacker News — sospecha de que un artículo sobre la Stasi usó un LLM, por el lenguaje "de relleno" — [INDETERMINADO]
> [PARÁFRASIS, no literal] Dice que la introducción le suena a texto redactado con ayuda de un LLM, citando la frase "a city where every street corner whispers secrets of a divided past" como ejemplo de lenguaje hueco; añade "Adjective-heavy fluff like this screams 'ChatGPT'/LLM to me", aclarando que no pretende desacreditar al autor.
Fuente: https://news.ycombinator.com/item?id=43820477

### Hacker News — extensión de Chrome creada porque "la mitad de mi feed de LinkedIn suena a la misma persona" — [NEGOCIO]
> "half my LinkedIn feed sounds like the same person" (motivación para crear una extensión que detecta posts de LinkedIn generados por IA)
Fuente: comment_id 47213560, story_id 47213559 (news.ycombinator.com/item?id=47213559)

### Hacker News — "no suena como un robot" como requisito explícito al buscar un generador de LinkedIn — [NEGOCIO]
> "does not make me sound like a robot." (buscaba específicamente un generador de posts de LinkedIn que evitara ese problema)
Fuente: comment_id 43245621 (news.ycombinator.com/item?id=43245621)

---

## Resumen de resultados por fuente

| Fuente | Resultado | Citas obtenidas |
|---|---|---|
| Quora | **BLOQUEADO** — sin una sola URL verificable, ni por búsqueda ni por fetch directo (403) | 0 |
| YouTube | **BLOQUEADO** — sin una sola URL de vídeo verificable sobre la que intentar extraer comentarios | 0 |
| Hacker News (vía Algolia API + item pages) | **Funcionó** | 14 citas verificadas con URL directa |
| Otras (ninguna añadida) | No se exploraron foros adicionales más allá de HN, por haber encontrado ya material suficiente y de calidad en esa fuente | 0 |

**Honestidad del resultado:** Quora y YouTube siguen exactamente igual de bloqueados que en las dos investigaciones Deep Research anteriores — no se consiguió ni una cita verificable de ninguna de las dos plataformas en esta tercera ronda, con varios enfoques de búsqueda distintos. La única vía que funcionó fue la alternativa explícitamente sugerida en el encargo (Hacker News), usando su API pública de Algolia en lugar de depender del buscador general. Dicho esto, el perfil de Hacker News es mucho más técnico que el del target del infoproducto (35-60 años, no-programadores); estas citas sirven como contraste y validación cruzada del problema ("sonar a IA" preocupa incluso a gente técnica), no como voz directa del comprador final.
