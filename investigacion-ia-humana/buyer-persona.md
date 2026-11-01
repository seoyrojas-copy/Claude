# Buyer Persona — Infoproducto de escritura humana con IA

> **Fecha del análisis:** 1 de noviembre de 2026.
> **Alcance del research usado:** un único corpus, `voc-textos-ia.md`, con 189 entradas de voz pública (147 de Reddit, 34 de Trustpilot, 7 de LinkedIn y 1 de YouTube). Lo recopilaron dos investigaciones Deep Research independientes (GPT y Gemini), que después se fusionaron sin solapamiento. Todo el material está en **inglés** y procede de comunidades mayoritariamente anglófonas. **No hay ni una sola voz en español** y no hay entrevistas, encuestas ni datos de comportamiento propios. Quora, YouTube (salvo un short) y Facebook no dieron resultado, como explican las notas metodológicas del propio corpus.
> **Uso exclusivo:** copywriting interno. No se comparte con el prospecto.
> **Segmento que desarrolla este documento:** el principal según el research. Es el adulto que usa ChatGPT/Claude en modo chat para escribir cosas que firma con su nombre y que leen **personas** (jefe, cliente, compañeros), y que teme que se note que lo ha escrito una máquina. La justificación y la recomendación sobre un segundo segmento están en el bloque «Segmentación por motivaciones».

---

## 0. Auditoría previa — Protocolo de procedencia y calidad del dato

### 0.1. Inventario del corpus (conteo bruto)

| Dimensión | Recuento | % sobre 189 |
|---|---|---|
| Reddit | 147 | 78 % |
| Trustpilot | 34 | 18 % |
| LinkedIn | 7 | 4 % |
| YouTube | 1 | 0,5 % |
| Tag [NEGOCIO] | 70 | 37 % |
| Tag [PERSONAL] | 43 | 23 % |
| Tag [INDETERMINADO] | 79 | 42 % |
| Tag adicional [BAJA CONFIANZA TÉCNICA] | 26 | 14 % |
| Marcadas [PARÁFRASIS, no literal] | 64 | 34 % |

(Los tags suman más de 189 porque alguna entrada lleva dos etiquetas de uso.)

Distribución por bloques temáticos del corpus:

| Bloque | Entradas | Composición dominante |
|---|---|---|
| A. Fricción con el tono robótico | 36 | 16 NEGOCIO / 19 INDET. / 4 PERSONAL · 7 BCT |
| B. Ser descubierto o acusado | 23 | 23 PERSONAL (≈17 académicas o de admisiones) · 6 BCT |
| C. Trabajo, clientes, relaciones | 28 | 24 NEGOCIO · 1 BCT |
| D. Humanizadores y detectores | 42 | 37 INDET. · 4 BCT |
| E. Lexicografía de IA | 53 | 22 NEGOCIO / 22 INDET. / 9 PERSONAL · 8 BCT |
| F. LinkedIn | 7 | 7 NEGOCIO |

**Convención de códigos.** Cada cita se referencia como letra de bloque + posición dentro del bloque en el archivo `voc-textos-ia.md` (por ejemplo, A20 es la vigésima entrada del bloque A: «15 minutos atascado con una frase»). Así cualquier afirmación de este documento se puede auditar contra la fuente.

### 0.2. Sistema de etiquetas de este documento

- **[LIT]**: cita literal del corpus. Como todo el corpus está en inglés, la versión en español es traducción mía. Doy el original cuando es corto, para que el copywriter vea el registro real.
- **[PAR]**: paráfrasis hecha por los investigadores originales, no literal. Pesa menos que una LIT.
- **[ANCL]**: frase construida por mí y anclada en una o varias entradas concretas del corpus (cito los códigos). No es una cita: es una adaptación al español con base documental.
- **[HIP]**: hipótesis sin base directa en el corpus. Sale de mercados similares, del conocimiento del comportamiento de los LLM en español o de la adaptación cultural al mercado hispanohablante. Hay que validarla.
- **[FUENTE ÚNICA]**: patrón sostenido por una sola entrada, un solo canal o un solo tipo de voz.
- **[DATO INSUFICIENTE]**: el corpus no permite responder con alta confianza. Siempre va seguido de una hipótesis etiquetada y de la investigación que lo resolvería.
- **[DATO INSUFICIENTE: falta granularidad]**: frase en primera persona sin anclaje temporal, sensorial ni situacional suficiente en los datos.

**Advertencia de partida sobre las frases en primera persona en español.** Ninguna frase en español de este documento es literal del comprador objetivo, porque el corpus no contiene voces en español. Las mejores frases posibles son [ANCL]: adaptaciones fieles de lo que escribieron angloparlantes. El vocabulario nativo hispano («se nota a la legua», «currar», «quedar fatal», «el email de turno») es [HIP] de registro. Es razonable, pero no está observado.

### 0.3. Tipo de fuente por insight

Todo el corpus es **dato observacional puro**: posts, comentarios y reseñas escritos para que otros los lean. A nadie se le preguntó nada. Eso tiene tres consecuencias:

1. **Lo escrito es real; el motivo, el contexto previo y lo que sentía a solas se deducen.** Cuando este documento afirma, por ejemplo, que «el prospecto siente vergüenza delante de su jefe», distingo entre lo que escribió (A5: «I hateee it!!», porque su jefe le repite que sus emails «suenan a ChatGPT») y lo que deduzco (que se queda pensando en ello después de la reunión). Lo segundo es inferencia.
2. **Reddit y Trustpilot premian el relato del incidente.** La gente escribe cuando algo le ha pasado: una acusación, un cargo inesperado, un cero. Eso sobrerrepresenta el pico emocional y deja fuera el malestar crónico y silencioso del día a día (el «lo reescribo y ya está»). El dolor medio del mercado probablemente es **más tibio y más crónico** de lo que sugiere el corpus.
3. **Trustpilot está sesgado hacia la queja.** Las 34 reseñas sobre humanizadores son casi todas negativas. Es un dato fuerte sobre la reputación de la categoría, pero no permite medir la proporción real de usuarios satisfechos.

### 0.4. Ponderación de voces — quién está hablando

He clasificado manualmente las 189 entradas en dos ejes: el **tipo de participante** que pide el protocolo y el **rol del hablante frente al problema**, que resulta decisivo en este mercado.

**Eje 1: rol frente al problema (clasificación propia, entrada por entrada)**

| Rol | Qué es | Entradas | % |
|---|---|---|---|
| **Emisor ante personas** | Usa IA para escribir algo que leerá una persona (jefe, cliente, compañero, público) y le preocupa que suene a IA. **Es la voz del comprador objetivo.** | ≈ 42 | 22 % |
| **Emisor ante detector** | Usa IA o humanizadores para que un algoritmo (Turnitin, GPTZero, ZeroGPT, Pangram) no lo marque. Casi todo el bloque D y parte del B. | ≈ 43 | 23 % |
| **Juez / receptor** | Recibe textos de IA de otros y los detecta, los desprecia o se ofende (managers, VP, amigos, clientes). No compra, pero es **la amenaza social** del comprador. | ≈ 37 | 20 % |
| **Acusado sin culpa** | No usa IA, o solo para la gramática, y le acusan de sonar a IA. | ≈ 34 | 18 % |
| **Víctima de la IA ajena** | Su trabajo humano lo pasan por IA terceros (el jefe, RR. HH., ejecutivos). | ≈ 10 | 5 % |
| **Comentarista / meta** | Opina sobre el fenómeno, debate el «delve», cita estudios. | ≈ 19 | 10 % |
| **Mensajería de competidor o con agenda** | Ver 0.8. | 3 seguras + 4 sospechosas | 2-4 % |
| Fuera de tema | E52 (OpenAI y los chatbots de compañía) | 1 | 0,5 % |

**Hallazgo crítico de procedencia:** solo **uno de cada cinco** testimonios del corpus es la voz directa del comprador objetivo (el emisor ante personas). El bloque más emocional, el B (acusaciones, ceros, el Dean, «freaking out»), lo protagonizan sobre todo **estudiantes falsamente acusados o que intentan pasar un detector**. No son el target. Si el copy se construye sobre esa intensidad, hablará a un universitario de 19 años con miedo a Turnitin y no a una administrativa de 48 que escribe a un cliente. Tampoco el juez es comprador. Pero es enormemente útil, porque ofrece **las frases exactas que el comprador teme oír** («Did ChatGPT write this?», «It sounds like ChatGPT», «feels like talking to a robot»).

**Eje 2: tipo de participante (protocolo)**

| Tipo | Señales en el corpus | Peso estimado | Ejemplos |
|---|---|---|---|
| **Recién llegado** | Pregunta básica, admite no saber, lenguaje no especializado, subreddits de ayuda (r/IWantToLearn, r/smallbusiness «uneducated new small business person me», usuario «nuevo» de Claude) | ≈ 14-16 % (las 26 BCT más 2 o 3 sin tag) | A20, A21, A27, A35, A36, E46, E12, E33 |
| **Ocasional** | Cuenta un incidente puntual sin identidad de comunidad: r/mildlyinfuriating, r/managers, r/antiwork, r/AITAH, casi todo Trustpilot | ≈ 45-50 % | A1, A5, C11, C27, D7-D42 |
| **Devoto / insider** | Domina la jerga (prompts, skills, «tells», Pangram), usa la IA «maniacally for over a year», escribe en r/ChatGPT, r/ClaudeAI, r/claudeskills, r/PromptEngineering, r/WritingWithAI, r/BypassAiDetect, r/copywriting, LinkedIn de creadores | ≈ 35-40 % | A19, A29, A30, A33, E1-E11, E38, F2, F6 |

**Aviso de ponderación, obligatorio por el protocolo:** el lenguaje más visible del corpus, el de la «lexicografía de IA», el debate sobre *delve* y *tapestry*, las listas de patrones o los «AI tells», viene del **devoto/insider**. El comprador objetivo, un adulto de 35 a 60 años con poca confianza técnica que solo usa el chat, es el **recién llegado**, y esa voz está claramente **infrarrepresentada** (≈ 15 %). Si el persona suena a forero de r/ChatGPT que discute sobre em dashes, estará mal ponderado. Por eso las 26 citas [BAJA CONFIANZA TÉCNICA] reciben **peso especial** en el Prisma, en la Mass Desire, en el Disparador situacional y en el lenguaje de los pilares.

**Las 26 voces de baja confianza técnica, desglosadas (las de más peso para este persona):**

- **Emisores ante personas, en contexto laboral (8):** A20 (15 minutos con una frase de un email importante a un cliente → lo pega en ChatGPT para que «suene más natural»), A21 (el ciclo de cambiar de pestaña, copiar, pegar y volver a corregir le rompe el ritmo), A27 («terribly AI» tras dar ejemplos e instrucciones, 6-8 prompts, le da *cringe*), A28 («defeats the purpose»: se le acaba el límite de uso intentando corregir el tono), C21 (bajo revisión interna de seguridad por mandar resultados de ChatGPT al correo corporativo), E22 («para cuando he conseguido explicarle lo que quiero, ya podría haberlo escrito yo»), E33 («It's so embarrassing 😭😭😭… triple check before sending next time»), A26 (probó instrucciones de personalización y sigue saliendo «ridículo»).
- **Recién llegados abrumados por la herramienta (3):** A35 (sigue confuso con el tono pese a dedicarle mucho tiempo), A36 (se define como poco técnico; todo va más rápido de lo que puede asimilar), E6 (un año usándola: los mismos clichés ya dan vergüenza).
- **Recién llegados con trucos caseros (3):** E12 («por el amor de Dios, no le digas que "no suene a IA"; usó todos sus clichés»), E24 («añade "tono conversacional, menos jerga corporativa"»), E25 («digo que el inglés es mi segunda lengua»).
- **Acusado sin culpa, adulto (1):** E46 («puede que suene a que tengo 1.000 años, pero ni siquiera sé usar la IA… me molesta que la gente despache mi esfuerzo como IA»). Es la única voz del corpus con una **señal de edad que encaja con el target**.
- **Estudiantes ante el detector (6):** B12, B13, B14, B17, B19 y B22. Fuera del segmento principal.
- **Víctimas de humanizadores (4):** D3 (BypassGPT, «totally fraudulent»), D13 (la prueba gratuita vuelve a detectar IA), D14 (cobro total cuando el anuncio decía «al mes»), D25 (StealthGPT: «creía que lo había cancelado… no reconocí el nombre del cargo hasta que lo busqué»). Son importantísimos para el prisma de riesgo, porque **el miedo del recién llegado no es solo que no funcione: es que le cobren sin entender por qué**.
- **Configuración permanente (1):** E53, un short de YouTube con el «rulebook once». Ojo: es mensajería de creador, no voz de cliente (ver 0.8).

### 0.5. Aviso específico de sesgo de voz: idioma, nacionalidad, edad y soltura técnica

1. **Idioma.** El 100 % del corpus está en inglés y el producto se vende en español. Los «tells» léxicos del corpus (*delve*, *tapestry*, *journey*, *spearheaded*, *I hope this message finds you well*, *don't hesitate to reach out*) son **del inglés**. Sus equivalentes en español («Espero que este mensaje te encuentre bien», «En el vertiginoso mundo de…», «Es importante destacar que…», «sumergirse», «adentrarse», «no solo… sino también…», «En resumen,») son **[HIP]**. Se basan en el comportamiento conocido de los LLM en español, no en voces observadas. Ningún dato del corpus confirma qué tics detecta el lector hispanohablante medio.
2. **Nacionalidad y cultura.** Predominan EE. UU., Canadá, Reino Unido y Australia (r/auscorp, ca.reddit.com, uk.trustpilot.com). Las dinámicas laborales (Slack, Teams, «WFH engagement emails», cold email B2B) son anglosajonas. En España y Latinoamérica pesan canales que el corpus no cubre (WhatsApp profesional, el correo con el gestor, la comunidad de vecinos, el grupo del colegio, LinkedIn en español, Facebook) **[DATO INSUFICIENTE]**.
3. **Edad.** El corpus no declara edades. Las señales son indirectas. El bloque B es mayoritariamente universitario o preuniversitario (UCAS, admisiones a Medicina y Odontología, Turnitin), así que es joven. Hay señales de madurez profesional (una periodista con 12 años de experiencia, una relación comercial de más de 20 años, VPs, managers, una directora de RR. HH., un abogado senior), pero casi siempre en el rol de **juez**, no de emisor. La franja de 35 a 60 años como **emisora** casi no aparece de forma explícita **[DATO INSUFICIENTE]**.
4. **Soltura técnica.** Reddit, y en particular r/ChatGPT, r/ClaudeAI y r/PromptEngineering, sobrerrepresenta a usuarios avanzados. El rasgo que define al target («siento que la tecnología me ha superado») aparece de forma explícita en **solo 4-5 entradas** (A35, A36, E46, E22 y, en parte, A21): es un patrón **minoritario-residual**. Por eso es la pieza más débil del persona y la que más research en español necesita.
5. **Consecuencia operativa.** Este persona está bien fundamentado en el **qué** (el problema, las frases del juez, el fracaso de los humanizadores, el fracaso de los prompts sueltos) y mal fundamentado en el **quién** (edad, idioma, canales y vocabulario nativo del hispanohablante de 35 a 60 años con poca confianza técnica). Todo lo que toca al quién va etiquetado.

### 0.6. Triangulación mínima

| Patrón | Canales donde aparece | Tipos de voz | Estado |
|---|---|---|---|
| Reescribir una y otra vez porque «sigue sonando a IA» | Reddit (varios subs), LinkedIn, Trustpilot (edición extra tras el humanizador) | Recién llegado, ocasional, insider | **Triangulado** |
| Comentario de una persona: «suena a ChatGPT» / «¿lo escribió ChatGPT?» | Reddit (trabajo y personal), LinkedIn | Emisor, acusado, juez | **Triangulado** |
| Los humanizadores no funcionan, destrozan el texto y cobran de forma opaca | Trustpilot (9 marcas) y Reddit (r/BypassAiDetect, r/WritingWithAI, r/PromptEngineering, r/studytips) | Ocasional, recién llegado | **Triangulado** (dos plataformas, nueve marcas) |
| Las instrucciones o prompts sueltos no arreglan el tono o se degradan | Solo Reddit (r/OpenAI, r/ChatGPT, r/ClaudeAI, r/claudeskills, r/AIWritingLounge) | Insider y recién llegado | Parcial: un solo canal, varias comunidades |
| Configurar la IA una vez en lugar de pelearse cada vez | Solo YouTube (E53) | Creador de contenido | **[FUENTE ÚNICA]** y además mensajería de creador |
| «Siento que la tecnología me ha superado» | Solo Reddit (A35, A36, E46) | Recién llegado | **[FUENTE ÚNICA]** de canal, frecuencia residual |
| Coste comercial directo (descuento, cliente perdido, 50 horas rechazadas) | Reddit y LinkedIn (E19, C11, C17, F7, C1) | Ocasional, juez | Triangulado, pero de frecuencia minoritaria |
| Vergüenza por dejar pegada la frase del asistente | Reddit (B22, E33, C18, C20, E29) | Emisor y juez | Triangulado, minoritario |

**Implicación importante:** el núcleo de la promesa del producto, «configúralo una vez y deja de pelearte», tiene **una sola mención directa** en todo el corpus, y viene de un creador que vende algo parecido. El **dolor** que resuelve sí está saturado (reescribir cada vez, el ciclo de copiar y pegar, el límite de uso que se va en correcciones). Pero el **deseo explícito** de la solución concreta no lo está. Es una oportunidad (nadie lo está diciendo en voz alta, así que hay espacio para «nombrarlo») y también un riesgo (no sabemos si el target lo cree posible).

### 0.7. Umbral de saturación: señal frente a anécdota

- **Saturado (señal fiable):** suena a IA, se nota, genérico, sin alma; reescritura; humanizadores que fallan; acusación o comentario de terceros; vocabulario delator en inglés. Recorrer más entradas de estos bloques ya no añade temas nuevos, solo variantes.
- **Frecuente pero no saturado:** las instrucciones fallan o se degradan (≈ 9-10); el coste en tiempo cuantificado (≈ 10); la «imperfección deliberada» como estrategia (≈ 6).
- **Anécdota (1-3 entradas, no puede presidir el copy):** dimitir por la IA (C6); revisión de seguridad corporativa (C21); clientes que piden descuento si saben que se usa IA (E19, [FUENTE ÚNICA], aunque es potentísima para el segmento autónomo); terapeuta con emails de IA (A10); tirar el MacBook al río (C7); el estudio de que los managers que usan IA parecen menos sinceros (E16, citado en Reddit, no verificado).
- **Regla aplicada:** el cliente que pide descuento (E19) o la dimisión (C6) son emocionalmente atractivos, pero no pueden ser el ángulo principal. Son material de body copy o de prueba lateral.

### 0.8. Filtro anti-contaminación de competidores

Las entradas siguientes **no se tratan como voz de cliente**. Las separo en la categoría «mensajería de competidor o con agenda comercial»:

| Código | Motivo de sospecha | Tratamiento |
|---|---|---|
| D2 | «Tools like Walter Writes AI help because they shift rhythm and pacing, not just reword sentences.» Tiene la estructura típica de comentario plantado: nombra la marca y repite su argumento de venta («ritmo, no solo palabras»). Además contrasta con siete reseñas de Trustpilot sobre Walter Writes, todas devastadoras (D30-D35). | **Excluida** del conteo de voz. Útil solo como muestra del argumentario de la competencia: **«cambiamos el ritmo, no solo las palabras»**. Ojo, porque es casi el mismo argumento que tendría este producto (la cadencia uniforme). Habrá que diferenciarlo. |
| D5 (2.ª frase) | «Tried grubby and it aint perfect». Mención de otra marca en un hilo que critica a un competidor: es el patrón clásico de *seeding*. | La primera mitad («Undetectable legit doesn't work») se conserva. La mención a la marca se excluye. |
| D24 | Es un resumen automático de reseñas generado por Trustpilot, no una voz. | Excluida como voz. Se conserva como dato agregado. |
| E53 | Short de YouTube de un creador que vende o promociona un «rulebook». Es el único texto del corpus que formula la promesa central de este producto. | **Mensajería de creador.** No es prueba de demanda. Indica que **ya existe** contenido gratuito con el mismo mecanismo, lo que afecta a la sofisticación (ver Schwartz). |
| F1 y F3 | Autor con hashtags `#ai-writing #buildinpublic`: probablemente un fundador que construye una herramienta de escritura con IA. Los relatos pueden ser reales, pero tienen agenda. | **Ponderación reducida** y etiquetada como «voz con agenda». |
| F6 | Cuenta de «content mentor»: vende formación sobre contenido. | Ponderación reducida. |
| Subreddits de marca (r/stealthgpt, r/bestaihumanizers) | Comunidades probablemente sembradas o moderadas por los propios humanizadores. | B14 y D28 se conservan, porque son quejas y una queja en territorio de marca es más creíble, pero se tiene en cuenta el entorno. |

**Argumentario de la competencia que NO debe colarse como voz del prospecto:** «100 % humano», «indetectable», «pasa todos los detectores», «bypass», «undetectability level», «modelo actualizado para superar a Pangram», «cambia el ritmo, no solo las palabras». Si alguna de estas expresiones acaba en el copy como si fuera la voz del cliente, el copy clonará a los humanizadores.

### 0.9. Limitaciones declaradas por el propio research

- **Quora:** no dio hilos indexados con detalle suficiente. Es una laguna relevante, porque Quora concentra preguntas de recién llegados de más edad («¿Cómo hago que ChatGPT…?»).
- **YouTube:** no expuso comentarios individuales verificables, y solo entra un short (E53). Es otra laguna relevante: los comentarios de YouTube en español («no me sale», «dónde se pone eso») serían probablemente **la mejor fuente del recién llegado de 45-60 años**.
- **Facebook:** bloqueado por login. Es la laguna **más grave para el target**, porque los grupos de Facebook en español sobre ChatGPT para autónomos, pymes, docentes e inmobiliarias concentran precisamente al usuario de 35 a 60 años con poca soltura técnica.
- **No invento nada para rellenar esas lagunas.** Donde hacen falta, aparece [DATO INSUFICIENTE] y se propone la investigación concreta que lo resolvería.

**Research adicional recomendado, por orden de impacto:**
1. Grupos de Facebook en español («ChatGPT en español», «IA para autónomos», «ChatGPT para inmobiliarias», «IA para docentes»): minar preguntas literales de recién llegados.
2. Comentarios de YouTube en español bajo vídeos del tipo «cómo hacer que ChatGPT escriba como un humano» o «instrucciones personalizadas ChatGPT»: buscar los «no me funciona» y los «¿dónde se pone esto?».
3. Entre 8 y 12 entrevistas de 30 minutos con usuarios de 35 a 60 años que usan ChatGPT para escribir en el trabajo. Preguntar por **la última vez** que alguien les dijo o insinuó que un texto suyo sonaba a máquina, y qué hicieron después.
4. Encuesta corta en la base de contactos del creador del producto (si existe), con una pregunta abierta: «¿Qué es lo que más te molesta de cómo escribe ChatGPT por ti?».

---

## Protocolo de honestidad sobre los datos — declaración de calidad global

| Área | Confianza | Motivo |
|---|---|---|
| Síntomas del problema (suena a IA, genérico, reescritura) | **Alta** | Saturado, triangulado y con varios tipos de voz |
| Reacción social (lo que dicen jefes, clientes y amigos) | **Alta** | Muchísimas voces de juez, frases literales |
| Reputación de los humanizadores | **Alta** | 42 entradas en dos plataformas y nueve marcas |
| Fracaso de prompts e instrucciones sueltas | **Media-alta** | ≈ 10 entradas, un solo canal |
| Motivación social del emisor (miedo a jefe y cliente) | **Media** | Directa en ≈ 15 entradas e inferida en el resto |
| Demografía (edad, ingresos, situación) | **Baja** | No hay datos demográficos en el corpus |
| Vocabulario nativo en español | **Baja** | Cero voces en español |
| Sensación de «la tecnología me ha superado» | **Baja** | Residual (4-5 entradas) |
| Canales y dieta informativa del target en español | **Baja** | Las fuentes del target no dieron resultado |
| Deseo explícito de «configurar una vez» | **Baja** | Fuente única de creador |
| Disposición a pagar 29 € | **Baja** | Solo hay anclas indirectas (humanizadores de 20, 60, 180 y 200 $) |

---

## 1. INFORMACIÓN SOBRE EL PRODUCTO

- **Nombre del producto o servicio:** pendiente de definir.
- **Qué hace exactamente (mecanismo, no promesa):** son dos piezas. **(1)** Un PDF que explica por qué los textos de ChatGPT y Claude no suenan humanos, con cuatro causas: **sintaxis predecible** (las mismas estructuras de frase), **hiperformalidad** (el registro de «asistente corporativo»), **vocabulario delator** (las palabras y muletillas que todo el mundo ya reconoce) y **cadencia uniforme** (frases de la misma longitud y párrafos de la misma forma). **(2)** Una *skill* o plugin que guía paso a paso, sin saber programar, para crear una **configuración permanente** dentro de la IA del propio usuario (Instrucciones personalizadas de ChatGPT, Proyectos de ChatGPT o Claude, o el equivalente), de forma que escriba con voz humana desde el primer mensaje. Así el usuario no tiene que pelearse con ella cada vez ni pasar después el texto por una herramienta externa «humanizadora».
- **A quién va dirigido:** personas de 35 a 60 años (también interesa gente más joven) que usan ChatGPT o Claude en modo chat normal, que **no** se atreven con herramientas de código (Claude Code, Codex, APIs) y que sienten que la tecnología les ha superado. No tienen que ser copywriters ni tener negocio propio.
- **Precio:** unos 29 € (**aproximado**; el creador puede bajarlo; no se trata como dato fijo).
- **Formato de entrega:** PDF más skill/plugin.
- **Prueba disponible:** pendiente de definir. Es un producto nuevo y todavía no tiene testimonios propios. **Restricción para el copy: no puede usarse prueba social propia hasta que exista, y bajo ningún concepto puede fabricarse.**
- **Competidores directos que ya existen:** herramientas «humanizadoras» de texto de IA (Undetectable.ai, StealthGPT, BypassGPT, Humbot, Walter Writes, HIX Bypass, BypassAI, WriteHuman, BypassDetection). Según el research tienen una reputación muy mala: destruyen el sentido del texto, siguen dando positivos en los detectores, facturan de forma opaca con cargos inesperados y añaden latencia y fricción de uso (D1-D42). **Competidores indirectos [HIP + corpus]:** prompts sueltos («que suene natural»), listas de palabras prohibidas, plantillas gratuitas de Instrucciones personalizadas en YouTube o TikTok (E53), parafraseadores y correctores, reescribir a mano, contratar a un redactor y dejar de usar la IA.
- **Qué lo diferencia:** no es una herramienta de terceros a la que se paga cada mes para que reescriba el texto **después** de generarlo (y que, según el research, falla constantemente, cobra de más y a veces empeora el texto). Es una configuración que el propio usuario crea **una vez** dentro de su propia IA, gratis a partir de ahí y sin depender de ningún servicio externo.
- **Fuente de los datos de investigación:** `voc-textos-ia.md`, con 189 entradas de Reddit, Trustpilot, LinkedIn y un short de YouTube, recopiladas mediante Deep Research de GPT y de Gemini. Todas en inglés. Ver la auditoría 0.1-0.9.
- **Cura frente a prevención:** **cura.** Resuelve un dolor presente: la vergüenza de que te descubran, la pérdida de confianza de clientes o jefes, la frustración y el tiempo perdido reescribiendo. Una matización del análisis: para la parte del mercado que **todavía no ha tenido el incidente** (el que usa la IA y no sabe que se nota, ver Niveles de consciencia), el producto se percibe como **prevención** («por si acaso me pillan»), y la prevención vende peor. El dolor presente que permite enmarcarlo como cura para ese subgrupo es **el tiempo que ya pierde hoy reescribiendo cada texto** (A20, A21, A28, A31, F2): ese tiempo lo pierde aunque nadie le haya pillado todavía.
- **Big Idea del producto en una frase:** pendiente de definir en la ficha original. **Propuesta tras el análisis** (ver la justificación en el Quality Gate): **«Lo que te delata no es que uses IA; es que tu IA todavía no sabe cómo hablas tú.»** Variante más corta para el titular: **«A nadie le molesta que uses IA. Le molesta que se note.»** La variante se apoya en E35: «Nobody cares if you use AI… What people hate is when your posts look obviously AI generated or sound robotic».

---

## 2. LISTA DETALLADA

### Demografía

**[DATO INSUFICIENTE]** El corpus no contiene ni edad, ni sexo, ni ingresos, ni país de ninguna voz. Lo que sigue combina la definición del target que da el creador con las señales indirectas del corpus. Cada subgrupo lleva su etiqueta.

**Rango de edad de los prospectos probables, en subgrupos:**

| Subgrupo | Rango | Base | Descripción breve |
|---|---|---|---|
| **Núcleo: «el que firma con su nombre»** | 38-55 | Definición del creador + señales de madurez profesional del corpus (managers, periodista de 12 años, relación comercial de más de 20 años, abogado senior, el «1.000 años» de E46) **[HIP con anclaje parcial]** | Empleado de oficina, mando intermedio, autónomo o profesional liberal (inmobiliaria, asesoría, seguros, formación, comercio, sector sanitario o administrativo). Escribe emails, propuestas, posts de LinkedIn, mensajes a clientes y resúmenes. Usa ChatGPT (y a veces Claude) en el navegador o en el móvil, «como quien usa Google». No ha tocado nunca una API y la palabra «prompt» le suena a jerga. Ha descubierto que la IA le ahorra el miedo a la página en blanco, pero el resultado «no es él». |
| **Veterano desbordado** | 50-62 | A36, E46, A35 **[HIP, residual en el corpus]** | Siente que la tecnología avanza más rápido de lo que puede asimilar. Usa la IA porque «hay que usarla» (lo dice su jefe o su sector), con cierta culpa y cierto pudor. Es el más vulnerable a la vergüenza de que le pillen y el que menos sabe cómo arreglarlo. |
| **Profesional joven de oficina** | 28-37 | A5, A7, A11, A17, F4 **[ANCL]** | Más soltura técnica, pero tampoco programa. Usa la IA a diario para Slack, Teams, el email y LinkedIn. Su riesgo es el jefe o el cliente que «ya se está dando cuenta» (A7). Interesa como mercado secundario. |
| **Excluido del núcleo: estudiante o candidato** | 17-26 | Bloque B y parte del D | Su juez es un algoritmo (Turnitin, GPTZero). Tiene otra motivación y otro criterio de éxito. Ver Segmentación y Anti-Persona. |

**Breve descripción del núcleo:** adulto en plena vida laboral que ha incorporado ChatGPT a su forma de escribir **sin haberlo aprendido nunca de verdad**. Pega su borrador y pide «mejóralo», «que suene más profesional» o «que suene más natural». Recibe un texto correcto que **no suena a él**, y entonces le toca elegir entre mandarlo así (y arriesgarse a que se note) o reescribirlo a mano (y perder el tiempo que pretendía ahorrar). No es copywriter, y lo dice con cierta disculpa: A22, «so much reshaping needed to make it sound like "me"», donde aclara que no es copywriter profesional. No quiere aprender ingeniería de prompts. Quiere que **la herramienta que ya usa** deje de delatarle.

**[DATO INSUFICIENTE]**: sexo, ingresos, situación sentimental, país. **Hipótesis basada en mercados similares** (infoproductos de productividad y de IA para no técnicos en español): ligera mayoría femenina en perfiles administrativos, de formación, inmobiliarios y de servicios, y mayoría masculina en mandos intermedios y autónomos técnicos. Ingresos medios; sensibilidad alta al pago recurrente y baja al pago único por debajo de 50 €. Hay que validarlo con los datos de ventas o de la lista del creador.

---

### Patrones Lingüísticos

#### Paso de conteo (dato, antes de interpretar)

Escala de proporción: **mayoritario** (> 25 % del corpus o del subconjunto relevante), **frecuente** (10-25 %), **minoritario** (3-10 %) y **residual** (< 3 %, entre 1 y 5 entradas). Doy dos denominadores: el corpus completo (189) y el subconjunto de **emisores ante personas** (≈ 42), que es la voz del comprador.

**A) Puntos de dolor**

| # | Patrón (frase o familia) | Entradas aprox. | % corpus | % emisores ante personas | Tipo de voz dominante |
|---|---|---|---|---|---|
| D1 | «Suena a IA / suena a ChatGPT / se nota que es IA» (*sounds like AI / ChatGPT*, *reads like AI*, *written the way AI writes*, *AI-like*) | ≈ 45 | **Mayoritario** (24 %) | Mayoritario | Todos los roles |
| D2 | Genérico, sin alma, robótico, impersonal, estéril, soso (*generic, soulless, robotic, impersonal, sterile, bland, flat*) | ≈ 32 | Frecuente (17 %) | Frecuente | Juez > emisor |
| D3 | Reescribir, rehacer, editar a fondo, «acabo reescribiéndolo todo» (*rewriting, reshaping, basically rewriting it anyway, rewrite about half*) | ≈ 22 | Frecuente (12 %) | **Mayoritario (≈ 45 %)** | Emisor (recién llegado + insider) |
| D4 | Acusación o marcado (*accused, flagged, reported to the Dean, zero*) | ≈ 30 | Frecuente (16 %) | Minoritario | Acusado y estudiante |
| D5 | El humanizador sigue detectado (porcentajes) | ≈ 22 | Frecuente (12 %) | Residual | Emisor ante detector |
| D6 | El humanizador destroza el texto (*gibberish, nonsense, scrambled, worse grammar, changes meaning, random capitals*) | ≈ 11 | Minoritario (6 %) | Residual | Emisor ante detector |
| D7 | Estafa o cobro opaco (*scam, charged the full amount, hidden charge, credits instead of refund*) | ≈ 9 | Minoritario (5 %) | Residual | Ocasional y recién llegado |
| D8 | Palabras y signos delatores (*tapestry, delve, journey, spearheaded, em dash, semicolons, "I hope this message finds you well", "In summary"*) | ≈ 16 | Minoritario (8 %) | Minoritario | **Insider** |
| D9 | Las instrucciones o prompts no lo arreglan, o se degradan (*it gets worse over time*, *don't tell it to "not sound like an AI"*) | ≈ 10 | Minoritario (5 %) | Frecuente (≈ 20 %) | Insider + recién llegado |
| D10 | Coste en tiempo cuantificado (15 min por frase, de 5 a 30 min, 20 min, 1 hora por 1.000 palabras, 6-8 prompts, «una semana») | ≈ 10 | Minoritario (5 %) | Frecuente (≈ 20 %) | Emisor |
| D11 | Vergüenza explícita (*embarrassing, mortified, cringe, am I cooked*) | ≈ 7 | Minoritario (4 %) | Minoritario | Emisor recién llegado |
| D12 | «Me está volviendo loco» (*driving me crazy, making me crazy, maddening, insane*) | ≈ 8 | Minoritario (4 %) | Minoritario | Ocasional |
| D13 | Insulto o falta de respeto (*insulting, so insulting, lazy*) | ≈ 6 | Minoritario | Residual (es más del juez) | Juez y víctima |
| D14 | Sentirse superado por la tecnología (*not technical, moving faster than I can absorb, I don't even know how to use AI*) | ≈ 4-5 | **Residual** | Minoritario | Recién llegado |
| D15 | Coste comercial directo (descuento, cliente perdido, 50 horas rechazadas, cold emails borrados) | ≈ 5 | Residual | Minoritario | Juez y ocasional |

**B) Emociones (palabras exactas)**

| Emoción | Frases exactas del corpus | Recuento aprox. |
|---|---|---|
| Hartazgo o enfado | «driving me crazy» (A1, C5), «making me crazy» (C22), «maddening» (B16, B20), «I hateee it!!» (A5), «tired of feeling angry» (C6), «sick and tired» (A33), «sad, annoyed, angry» (A17) | ≈ 10 |
| Vergüenza | «It's so embarrassing 😭😭😭» (E33), «cringe» (A27), «am I cooked 😭» (B22), «Ouch my heart» (A15), «the most embarrassing thing» (E27-E29) | ≈ 7 |
| Pánico o ansiedad | «kinda freaking out» (B7), «now I am freaking out» (B15), «Horrified» (B11), «can't even use semicolons without feeling scared» (B5), «Am I good or should I be worried?» (B14), los errores «le mantienen despierto» (B4, PAR) | ≈ 8 (casi todos estudiantes) |
| Asco o rechazo físico | «my soul left my body» (C1), «leaves a bad taste in my mouth… Yuck» (E27), «ganas de vomitar» (E39, PAR), «my brain just turns off» (E48), «AI stink» (E23) | ≈ 6 |
| Ofensa | «It's so insulting» (A9), «insulting» (C11), «deeply offended» (A13) | ≈ 4 |
| Impotencia o confusión | «no idea what to do» (B19), «literally so frustrated rn» (B19), «defeats the purpose» (A28), «don't recognize it anymore» (A34) | ≈ 6 |

**C) Resultados deseados**

| # | Deseo | Entradas aprox. | Proporción |
|---|---|---|---|
| R1 | Que «suene natural / humano / a persona real» (*sound more natural*, *real modern human*, *conversational tone*, *more authentic*) | ≈ 10 | Minoritario en el corpus, **frecuente entre emisores** |
| R2 | Que «suene a mí» (*sound like "me"*, *doesn't sound like me*, *don't want to lose my voice*, *esto no lo escribí yo*) | ≈ 8 | Minoritario en el corpus, frecuente entre emisores |
| R3 | Imperfección o autenticidad (*imperfect personality*, *less perfect but authentic*, meter imperfecciones deliberadas, «¿vuelvo atrás y cometo faltas?») | ≈ 6 | Minoritario |
| R4 | Indetectable, 100 % humano, pasar el detector | ≈ 25 | Frecuente en el corpus, **pero del segmento estudiante/detector** |
| R5 | No perder el ahorro de tiempo (*defeats the purpose*, *basically rewriting it anyway*, *might as well have written it myself*) | ≈ 5 | Minoritario |
| R6 | Configurar una vez y no pelearse cada vez (*give it a rulebook once*) | 1 | **Residual. [FUENTE ÚNICA], de creador** |

**D) Objeciones recurrentes**

| # | Objeción | Entradas aprox. | Proporción |
|---|---|---|---|
| O1 | «Los humanizadores son una estafa / no funcionan / mira las reseñas» | ≈ 15 | Frecuente |
| O2 | «Ya probé a darle instrucciones o ejemplos y sigue sonando a IA» | ≈ 9 | Minoritario-frecuente |
| O3 | «Los detectores no funcionan» (y por tanto «demostrar que es humano» no tiene sentido) | ≈ 6 | Minoritario |
| O4 | «Para lo que tardo en explicárselo, lo escribo yo» | ≈ 3 | Residual |
| O5 | «Evitar las palabras típicas también suena a IA» | 2 | Residual |
| O6 | «No soy técnico / esto va demasiado rápido» | ≈ 4-5 | Residual |

#### Interpretación (lectura, separada del dato)

1. **El dolor que más pesa en la voz del comprador no es «me han pillado», sino «tengo que reescribirlo».** En el corpus completo domina «suena a IA», pero entre los emisores ante personas, que son el comprador, el patrón más repetido es la **reescritura** (≈ 45 %). El miedo a que le pillen es el **motivo** de la reescritura. La reescritura es el **síntoma diario**. Para el copy: **la escena de apertura con más base empírica no es la acusación, sino la de estar reescribiendo por tercera vez el mismo email.**
2. **La acusación es el pico; la reescritura, el valle.** La acusación (D4) es frecuente, pero se concentra en estudiantes y en acusados sin culpa. Para el comprador adulto, el corpus muestra el comentario del juez como **el miedo que le empuja a reescribir** («Did ChatGPT write this?», F1; «It sounds like ChatGPT», F7; el jefe que «is catching on», A7/E17). Ese miedo funciona en el copy como **detonante** y como **escena temida**, no como rutina.
3. **El vocabulario delator es lenguaje de insider.** *Delve*, *tapestry*, los em dashes y los punto y coma los discuten devotos de r/ChatGPT y r/writing. El recién llegado no dice «el problema son los em dashes». Dice «no sé qué tiene, pero se nota» (C23: «people aren't stupid, they know when something feels off even if they can't put finger on exactly what it is»). **Consecuencia: el PDF puede enseñar el vocabulario delator, pero el copy de entrada no debe abrir con jerga de «tells». Tiene que abrir con la sensación de «se nota y no sé por qué».**
4. **La promesa de «indetectable» es del otro segmento.** El 25 % del corpus que persigue porcentajes en un detector no es el comprador principal. Usar «indetectable» o «pasa los detectores» atraería al anti-persona y además activaría la desconfianza que generaron los humanizadores.
5. **La sensación de estar superado por la tecnología es residual en los datos, pero central en la definición del producto.** No puede presidir el copy con la base actual. Puede ser **tono** (calma, pasos claros) antes que **ángulo**, hasta que el research en español lo confirme.

#### Filtro de calidad — frases conservadas por granularidad

Solo conservo como material de copy las frases con anclaje temporal, sensorial o situacional. Primero las del corpus y después su adaptación.

| Frase original (corpus) | Anclaje | Etiqueta | Adaptación al español para copy |
|---|---|---|---|
| «I find myself writing and rewriting every email and message I send at work because everything sounds like it was written by AI now… It is driving me crazy!» (A1) | Situacional (cada email del trabajo) | LIT | «Me paso el día escribiendo y reescribiendo cada email del trabajo porque todo me suena a escrito por una máquina. Me está volviendo loca.» **[ANCL A1]** |
| Quince minutos atascado con una sola frase de un email importante a un cliente → lo copia en ChatGPT para pedir que «suene más natural» (A20) | Temporal + situacional | PAR · BCT | «Llevo un cuarto de hora con la misma frase del email al cliente. Al final se la pego a ChatGPT y le pido que suene natural. Y me devuelve algo peor.» **[ANCL A20, A11]** |
| Cambiar de pestaña, copiar, pegar y volver a corregir le rompe el ritmo (A21) | Situacional + quasi-físico (el gesto) | PAR · BCT | «Pestaña, copiar, pegar, corregir, otra pestaña, copiar, pegar… cuando termino ya no sé ni lo que quería decir.» **[ANCL A21]** |
| Un email de cinco minutos se convierte en media hora de relecturas, con la duda de dejar un error a propósito: «Does this sound like me… or ChatGPT?» (F2) | Temporal + situacional | LIT/PAR | «Un email de cinco minutos y llevo media hora releyéndolo. Hasta me planteo dejar una falta a propósito para que se note que es mío.» **[ANCL F2, B21, A24]** |
| «Did ChatGPT write this?», después de veinte minutos escribiéndolo a mano (F1, voz con agenda) | Temporal + social | LIT | «Veinte minutos escribiendo yo el email, palabra por palabra, y el cliente me contesta: "¿Esto lo ha escrito ChatGPT?".» **[ANCL F1]** |
| «It sounds like ChatGPT», en una llamada con el cliente después de más de 50 horas de trabajo (F7) | Temporal + situacional | LIT | «Cincuenta horas de trabajo y el cliente lo despacha en la llamada con un "esto suena a ChatGPT".» **[ANCL F7]** |
| «terribly AI», tras 6-8 prompts, ejemplos e instrucciones; le da *cringe* (A27) | Cuantitativo + corporal leve | LIT · BCT | «Le he dado ejemplos, le he explicado cómo escribo, ocho intentos… y sigue saliendo eso que te da vergüenza ajena al leerlo.» **[ANCL A27]** |
| «defeats the purpose» (se le acaba el límite de uso corrigiendo el tono) (A28) | Situacional | LIT · BCT | «Se me acaba el límite del día pidiéndole que no suene a robot. ¿Para qué lo pago entonces?» **[ANCL A28]** |
| «by the time I've figured out how to explain to it exactly what I want, I might as well have just written the thing myself» (E22) | Temporal implícito | LIT · BCT | «Para cuando consigo explicarle lo que quiero, ya lo habría escrito yo.» **[ANCL E22]** |
| «It's so embarrassing 😭😭😭… Just have to remember to triple check before sending next time» (E33) | Situacional (el envío) | LIT · BCT | «Qué vergüenza. Se me quedó pegado el texto de la IA y lo mandé así. A partir de ahora lo miro tres veces antes de darle a enviar.» **[ANCL E33, B22]** |
| «my soul left my body» al ver el email de ChatGPT que un junior mandó a un cliente en un asunto facturado por miles (C1) | Corporal + situacional | LIT | Material de **juez**: «Se me cayó el alma a los pies cuando vi lo que le había mandado al cliente.» **[ANCL C1]** |
| «I try to read it it is like my brain just turns off» (E48) | Corporal | LIT | Material de **juez**: «Empiezo a leerlo y se me apaga el cerebro. En la segunda línea ya sé que es de máquina.» **[ANCL E48]** |
| «If customers know that AI is used to do the job then they will ask for a discount» (E19) | Situacional / económico | LIT · [FUENTE ÚNICA] | «Si el cliente huele que lo ha hecho la IA, me pide descuento. Así de claro.» **[ANCL E19]** |
| «Started letting my AI handle work messages, my boss is catching on» (E17/A7) | Situacional | LIT | «Empecé a dejar que la IA me escribiera los mensajes del trabajo y creo que mi jefe ya se ha dado cuenta.» **[ANCL E17]** |
| «I hateee it!!» (su jefe le repite que sus emails, mensajes de Slack y resúmenes «suenan a ChatGPT») (A5) | Situacional | LIT | «Mi jefe me ha vuelto a decir que mis emails suenan a ChatGPT. Lo odio.» **[ANCL A5]** |
| «I didn't like that I was charged the full amount when the ad said it's per month» (D14) | Situacional | LIT · BCT | «El anuncio decía al mes y me cobraron el año entero. "Cancela cuando quieras", decían.» **[ANCL D14]** |
| «I thought I'd canceled this subscription!!! … I didn't recognize the name at first until I searched it» (D25) | Situacional | LIT · BCT | «Veo un cargo en la cuenta, no sé ni de qué es, lo busco… y es la herramienta esa que creía haber cancelado.» **[ANCL D25]** |
| «for the love of god don't tell it to "not sound like an AI". I tried that and I swear it used all its favorite cliches as much as it possibly could!» (E12) | Situacional | LIT · BCT | «Le pedí que no sonara a IA y me metió todas las frases de IA juntas. Te lo juro.» **[ANCL E12]** |
| «this might make me sound 1000 years old, but I don't even know how to use AI» (E46) | Identitario (edad) | LIT · BCT | Única señal de edad del corpus: «Igual sueno a que tengo mil años, pero es que yo ni sé usar eso.» **[ANCL E46]** |

**Frases descartadas por baja granularidad** (frecuentes, pero no sirven como material de copy): «It doesn't sound like me» (A4) sin más contexto, «Still reads generic though» (A11), «sigue sonando raro» (A12), «Awful writing» (A19), «it doesn't work» (D4-D6) en abstracto. Se pueden usar como **léxico** («no suena a mí», «sigue sonando raro», «no funciona»), pero no como escenas. **[DATO INSUFICIENTE: falta granularidad]** en su forma original.

**Vocabulario nativo probable en español [HIP, a validar con research en español]:** «se nota a la legua», «suena a robot», «suena a ChatGPT», «parece un folleto», «parece escrito por un comercial», «queda muy de plantilla», «muy de manual», «muy acartonado», «no es mi forma de hablar», «esto no lo diría yo nunca», «lo tengo que retocar todo», «me pego más rato corrigiendo que escribiendo», «me pillan», «quedar fatal», «quedar como un vago», «que no se note».

---

### Prisma de interpretación

Cómo interpreta este prospecto la categoría («herramientas y trucos para que lo que escribe la IA no suene a IA»). Doy peso especial a las voces [BAJA CONFIANZA TÉCNICA].

**¿Qué significa para él «calidad» en esta categoría?**
No es «indetectable». Para el comprador principal, calidad significa **que el texto pase por suyo ante la persona que lo va a leer**: que su jefe, su cliente o su compañero lo lean sin pararse. El estándar de calidad es **la ausencia de reacción**. El mejor resultado posible es que nadie diga nada. Lo dicen de forma indirecta varias entradas: el lector «sabe cuando algo chirría aunque no sepa decir qué es» (C23); «people hate… when your posts look obviously AI generated» (E35); prefiere mensajes «menos perfectos pero auténticos» (C4). La segunda capa de calidad es **que no tenga que tocarlo**: que el primer resultado sirva (A31, «basically rewriting it anyway», es la definición negativa de calidad). **[ANCL]**

**¿Qué considera «riesgo» en esta compra?**
1. **Que le cobren sin entender por qué.** Es el riesgo más concreto y con más carga emocional entre las voces BCT: D14 (cobro anual cuando el anuncio decía mensual), D25 (cargo no reconocido de una suscripción que creía cancelada), D8 (más de 200 $ anuales no esperados y días por email intentando resolverlo), D10 (le ofrecen créditos en lugar de devolverle el dinero). **El riesgo no es solo perder 29 €. Es caer otra vez en una de esas webs que te cobran cosas que no entiendes.**
2. **No ser capaz de hacerlo.** Es la versión del recién llegado: A35 (confuso incluso tras dedicar mucho tiempo), A36 (todo avanza más rápido de lo que asimila). El miedo es comprarlo, abrirlo y no entender dónde se pone cada cosa. **[ANCL + HIP de intensidad]**
3. **Que no funcione, como todo lo anterior.** A26 (probó instrucciones de personalización: «ridículo»), A27 (ejemplos e instrucciones: «terribly AI»), A29 (las listas de patrones no meten su personalidad).
4. **Romper algo o liarla con la cuenta.** **[HIP]** El usuario de chat que nunca ha tocado los ajustes de ChatGPT teme estropear algo, que le cambien el plan o que la IA «se vuelva rara». No hay base directa en el corpus. Hay que validarlo en las entrevistas.
5. **Quedar como alguien que hace trampas.** **[ANCL E19, C27]** Comprar un producto para que «no se note la IA» puede vivirse como una confesión. C27: «está bien usar IA para editar tu trabajo, pero tiene que ser TU trabajo».

**¿Qué es para él «una buena decisión»? ¿Y una mala?**
- **Buena:** algo que pago **una vez**, que entiendo, que hago en una tarde y que a partir de ahí me deja **dejar de pensar en esto**. Que no dependa de una web que mañana cierra o cambia los precios. **[ANCL A21, A28, D8, D25 + HIP]**
- **Mala:** otra suscripción que se renueva sola, otra herramienta en otra pestaña, otro «modelo actualizado» que vuelve a fallar a la semana (D28, D29: «algo que funcionaba la semana pasada deja de funcionar»), otro curso de 12 horas del que veo 20 minutos.

**¿Qué proyecta en esta compra a nivel de identidad?**
Ambivalencia. Por un lado: **«soy de los que usan la IA bien, no de los que la usan a lo bruto»**. Es la distinción que repiten los jueces. E35 (nadie se queja de que uses IA, se quejan de que suene a IA), E36 («have it write the email, and then rewrite it in your own words»), E34 («usar IA responsablemente no debería ser un secretito sucio»). Por otro lado: **cierto pudor**, porque comprar esto confirma que lo estaba haciendo mal y que necesita ayuda con algo que «todo el mundo» parece manejar. **[ANCL + HIP]**

**¿Qué experiencias pasadas condicionan cómo filtra lo que ve ahora?**
1. Haber pedido «que suene más natural» y recibir algo **más** artificial (A20, E12).
2. Haber dado instrucciones y ejemplos y que no sirviera, o que funcionara un rato y se degradara en la conversación (A19: «It gets worse over time»; A27).
3. Haber visto, o al menos leído, que las herramientas humanizadoras son una estafa (D1: «IT'S A $20 SCAM FOR BROKEN GARBAGE!!!»; D6: «Look at the reviews»).
4. Haber recibido un comentario de una persona: el jefe (A5, C27), el cliente (F1, F7), un amigo (C19).
5. Haber estado del otro lado: haber recibido un email de IA de otro y haber sentido ese rechazo (bloque C). **Este es un filtro poderoso. El comprador sabe cómo se siente el juez porque él mismo lo ha sido.** **[ANCL C, E13, E48]**

**¿Qué ejemplos le vienen a la mente de forma automática?**
- **De engaño:** la web que prometía «100 % humano» y luego te cobraba el año entero (D8, D14, D25).
- **De fracaso:** el texto «humanizado» que salió con palabras raras, mayúsculas en medio de la frase o un sentido distinto (D23, D30, D33, D34, D40).
- **De vergüenza ajena:** el compañero que pegó en el correo «Claro, aquí tienes una versión más profesional de tu email:» (B22, C18, C20, E29 «Written by ChatGPT and I forgot to edit it»).
- **De vergüenza propia:** la frase de la IA que se le quedó pegada o el comentario del jefe.
- **Casi ningún ejemplo de éxito.** El corpus no contiene ni un solo testimonio de «lo configuré y ahora escribe como yo». Hay quien dice que algunas listas «quitan algunos tics» (A29), pero no hay éxito completo. **Su punto de partida emocional es el escepticismo con una pizca de esperanza.**

**Frases en primera persona que revelan su forma de interpretar la categoría:**
1. «Cada vez que me prometen que ChatGPT va a escribir "como un humano" acabo igual: a las once de la noche, reescribiendo el email a mano.» **[ANCL A1, A31 · anclaje temporal HIP]**
2. «Con estas cosas siempre pasa lo mismo: la web dice "cancela cuando quieras" y a los dos meses ves en el banco un cargo que no reconoces.» **[ANCL D14, D25]**
3. «Si fuera tan fácil como poner una frase en los ajustes, ya lo habría hecho. Lo probé y a los tres mensajes volvía a hablar como un folleto.» **[ANCL A19, A26, A27]**

**Umbral MAYA (novedad frente a seguridad):**

- **Barrica vieja (lo familiar obligatorio):**
  - Que funcione **dentro de ChatGPT o Claude, la pantalla que ya conoce**. Ni otra web, ni otra app, ni otra pestaña. (Se deduce de A21: el ciclo de pestañas es justo lo que odia.)
  - **Pago único y claro**, sin suscripción. (Se deduce de D8, D14, D25.)
  - Ver **un antes y un después** con un texto como los suyos (un email, un mensaje a un cliente), no con un ensayo académico.
  - Instrucciones **paso a paso, con capturas**, del tipo «haz clic aquí y pega esto». **[HIP fuerte: estándar de los infoproductos para no técnicos]**
  - Que alguien con cara y nombre esté detrás. **[HIP]**
- **Vino nuevo (la sorpresa aceptable):**
  - **«No es un truco de prompt. Es enseñarle a tu IA cómo hablas tú, una sola vez.»** Es una novedad que se apoya en algo que ya conoce (los ajustes de ChatGPT existen, aunque no los haya tocado).
  - **Entender por qué suena a IA**, con nombres sencillos para las cuatro causas. Al recién llegado le da control: «ah, por eso».
  - **La paradoja de E12**: pedirle «que no suene a IA» lo empeora. Es contraintuitivo, verificable y no da miedo.
  - Que **la imperfección es una virtud** (C4, A24, A25): ver un texto «menos perfecto» y que funcione mejor.
- **Zona de shock (novedad rechazada):**
  - Cualquier mención a **código, API, terminal, Claude Code, agentes, archivos .json o «instalar»**. Activa el «esto no es para mí» al instante.
  - **«Indetectable», «100 % humano», «engaña a los detectores».** Le suena a los humanizadores-estafa y, para el adulto honrado, a trampa.
  - **Plugin o extensión del navegador** sin explicar qué hace con sus datos. **[HIP]** Hay que ir con cuidado con la palabra «plugin»: para un usuario de 55 años puede sonar a «algo que me instalo y me espía».
  - Promesas del tipo «escribirá exactamente como tú» o «clona tu voz». Las voces A30 (probó «clonadores de voz») y A29 lo desmienten por experiencia.
- **Dos frases en primera persona que ilustran su umbral:**
  1. «Si me dices que tengo que instalar algo o tocar código, cierro la pestaña. Si me dices que es dentro de mi ChatGPT, el mismo de todos los días, te escucho.» **[HIP con anclaje A21, A36]**
  2. «Otra web que "humaniza" no, gracias. Ya he visto lo que hacen con el texto y con la tarjeta.» **[ANCL D1, D14, D25, D30]**

---

### Problema central

**El problema principal:** el prospecto usa ChatGPT o Claude para escribir cosas que firma con su nombre y que van a leer personas que le importan (su jefe, sus clientes, sus compañeros). El resultado **suena a máquina**, y lo nota él o, peor, lo notan los demás. Para evitarlo tiene que reescribirlo a mano, con lo que pierde el tiempo que la IA prometía ahorrarle, o mandarlo tal cual y arriesgarse a quedar como un vago, un falso o alguien que ya no hace su trabajo. Los atajos que ha probado (pedir «que suene natural», darle instrucciones, pasarlo por un humanizador) no lo han resuelto. A veces lo han empeorado y otras le han costado dinero. Y **no tiene los conocimientos técnicos** para entender por qué pasa ni cómo arreglarlo de raíz.

**Síntomas del problema** (problema → síntoma observable):

| Síntoma | Base |
|---|---|
| Relee el mismo email tres, cuatro o cinco veces antes de enviarlo, preguntándose si «suena a él o a ChatGPT» | F2, F3, F6 [LIT/PAR] |
| Un texto de cinco minutos se le convierte en media hora | F2 [PAR] |
| Se queda un cuarto de hora atascado en una frase y acaba pegándola en ChatGPT… que la empeora | A20 [PAR · BCT] |
| Borra palabras «que jamás usaría» y reescribe más o menos la mitad de cada borrador | A4 [PAR] |
| Ha desarrollado un ritual de pestañas: ChatGPT, el correo, ChatGPT otra vez, el corrector… | A21 [PAR · BCT] |
| Mete errores o frases torpes **a propósito** para que parezca humano | A24, B21, F2 [PAR] |
| Ha dejado de usar ciertos signos (rayas, punto y coma) por miedo a que «parezcan de IA» | A6, B5 [PAR/LIT] |
| Se le acaba el límite de uso del día en correcciones de tono | A28 [LIT · BCT] |
| Revisa tres veces antes de enviar desde que una vez se le coló la frase del asistente | E33, B22 [LIT · BCT] |
| Ha empezado a sospechar de su **propia** forma de escribir («¿escribo como una IA?») | A13, A15, F6 [LIT/PAR] |
| Evita usar la IA para cosas importantes, justo donde más le ayudaría, por miedo a que se note | E19, E22 [ANCL] + **[HIP]** |
| Siente un pinchazo de alerta cuando alguien comenta algo sobre «lo bien redactado» que está un email suyo | **[HIP]**, inferido de A5, F1 |

**Impacto emocional:**
- **Vergüenza anticipatoria.** Vive con el miedo de que «se note» incluso cuando nadie ha dicho nada. Es el «Does that sound like AI?» que se pregunta **casi a diario** (F6).
- **Sensación de impostor.** El texto que manda no es suyo, y lo sabe. A9: «It's so insulting», con la sensación de que su criterio y su forma de escribir han sido sustituidos por una versión impersonal. F3: «esto no lo escribí yo».
- **Frustración de bucle.** Cada intento de arreglarlo vuelve al mismo sitio (A31, A30).
- **Incompetencia tecnológica** (para el subgrupo veterano): la sospecha de que «los demás sí saben hacerlo» y él no (A35, A36). **[ANCL residual + HIP]**
- **Pérdida de la autoestima como escritor.** El acusado sin culpa (E46, A15 «Ouch my heart») y el que ya no distingue su voz de la de la máquina (A13, «deeply offended»).

**Impacto social:**
- **Trabajo:** el jefe que «se está dando cuenta» (A7, E17), que le cita para hablar de una diapositiva (C27: «He was NOT happy»), que repite que sus emails suenan a ChatGPT (A5). Un estudio citado en el corpus (E16, no verificado) dice que los managers que usan IA para escribir emails se perciben como **menos sinceros, menos atentos y menos seguros**.
- **Clientes:** el cliente que pregunta «¿esto lo ha escrito ChatGPT?» (F1); el que despacha 50 horas de trabajo con «suena a ChatGPT» (F7); el que pide descuento si sospecha que se ha usado IA (E19, fuente única); la relación comercial de más de 20 años que se rompe tras una cadena de respuestas de IA (C11, desde el lado del juez); el VP que borra entre 30 y 40 cold emails por semana en segundos (C17).
- **Compañeros:** el compañero que se queja de los emails de IA «perezosos, impersonales y extraños» (C4); los mensajes de IA que «ni el propio remitente entiende» (C10).
- **Círculo personal:** la amiga que «feels like talking to a robot» (C18), el amigo de años con expresiones que nunca usaba («really glad ChatGPT cares…», C19), el hermano que te acusa en medio de una discusión (B3). Ojo: en el corpus estas son **voces de juez**. Como impacto social sobre el comprador son **[ANCL indirecto]**.

**5 frases conversacionales (pero hirientes) que otras personas podrían decirles:**
1. «¿Esto lo has escrito con ChatGPT?» **[ANCL F1, «Did ChatGPT write this?»]**
2. «Está bien que uses la IA para repasar, pero tiene que ser TU trabajo. Esto no dice nada de nuestro proyecto.» **[ANCL C27, casi literal]**
3. «Qué bonito. Me alegra ver que a ChatGPT le importo.» **[ANCL C19, «really glad ChatGPT cares…»]**
4. «Hablar contigo últimamente es como hablar con un robot.» **[ANCL C18]**
5. «Si me lo vas a mandar escrito por la máquina, mándame directamente el prompt y nos ahorramos los dos el rato.» **[HIP, construida con el tono de E36, C4, C10]**

---

### Clasificación del dolor (tres capas)

- **Capa dominante: DOLOR PERSONAL** (identitario y relacional). El corpus está lleno de **escenas** (el jefe, el cliente, la llamada, la amiga) y de **identidad** («no suena a mí», «esto no lo escribí yo», «¿escribo como una IA?»). El daño no se mide en euros, sino en **cómo te ven** y en **cómo te ves**. Entre los emisores ante personas, la mayoría de las entradas describen un momento social o una pérdida de voz propia, no una pérdida económica.
- **Capa secundaria: DOLOR FINANCIERO en forma de TIEMPO** (y, para los que ya probaron humanizadores, de dinero tirado). El tiempo está cuantificado en el corpus (15 minutos por frase, de 5 a 30 minutos por email, 20 minutos, 6-8 prompts, una hora por 1.000 palabras, «una semana» intentándolo, más de 50 horas rechazadas). El dinero tirado también: 20, 60, 180 y más de 200 $ en humanizadores. Sirve para **justificar con lógica** y para el **anclaje de precio**. No sirve para abrir.
- **Capa terciaria: DOLOR ESTRATÉGICO** (reputación a 1-3 años: «el que despacha con robot», «el que ya no aporta»). **[HIP con anclaje E16, C4, C16]** Está presente en la sombra, pero apenas se verbaliza.

**Consecuencia directa para el copy:** el argumento que activa la decisión en este mercado es **una escena específica y reconocible**: el email releído por cuarta vez a las once de la noche, el «¿esto lo has escrito con ChatGPT?» en la bandeja de entrada, la llamada en la que el cliente lo despacha. Las cifras de tiempo y de dinero van **detrás**, en el body copy y en el bloque de precio, como justificación racional («y encima te ahorras X horas al mes y no vuelves a pagar una suscripción»). **Abrir con números (ROI, horas ahorradas) es un error para este mercado**, porque el dolor primero se vive y después se cuenta.

---

### Disparadores de motivación

**Costes futuros de no resolver el problema:**
- Seguir **pagando con tiempo** cada texto: la IA, que debía ahorrarle horas, se las sigue quitando (A31: «basically rewriting it anyway»).
- Que un día **le pillen de verdad** con algo importante: la propuesta al cliente grande, el email al director, el post de LinkedIn que lee todo su sector. **[ANCL F7, C1, E19]**
- **Quedarse atrás**: no poder usar la IA en lo que de verdad importa por miedo a que se note, mientras ve que otros la usan «sin que se note». **[HIP con anclaje E35, E22]**
- **Erosión lenta de la reputación**: convertirse en «el de los emails de ChatGPT», sin que nadie se lo diga a la cara. **[ANCL C12, C13, C15, E16]**
- Seguir **perdiendo dinero** en herramientas que no funcionan (para quien ya probó humanizadores). **[ANCL D8, D9, D36]**

**Impacto social de no resolverlo:**
- El jefe deja de fiarse de sus textos y empieza a corregírselos (A8: el jefe pasa sus emails por ChatGPT; ironía total) o a revisarlos más.
- El cliente empieza a tratarle como «alguien que despacha con plantillas», le pide descuento (E19) o, simplemente, deja de contestar (C17, los cold emails borrados en segundos).
- Los compañeros lo comentan en el café. **[HIP]**: no hay voz directa del emisor sobre esto, solo voces de jueces que se quejan entre ellos (C12, C15, E30).
- En lo personal, la sensación de que sus mensajes «no son él» se cuela también en WhatsApp con amigos y familia. **[HIP con anclaje C18, C19]**

**Si un genio pudiera resolverlo al instante, ¿cómo cambiaría su vida el prospecto?**
Abre ChatGPT, le pide el email a un cliente y **lo que sale ya suena a él**: sus expresiones, su forma de saludar y de despedirse, sin «Espero que este mensaje te encuentre bien», sin esa simetría de folleto. Lo lee una vez, cambia un dato y le da a enviar. No relee. No le da vueltas por la noche. Cuando el cliente contesta, contesta **al contenido**, no a la forma. Recupera la media hora diaria que se le iba en retoques. Y deja de tener esa vigilancia de fondo de «¿se notará?». **[ANCL F2, A31, A20 + HIP de escena]**

**¿Cómo afectaría esta transformación a las relaciones clave de su vida?**
- **Con el jefe:** pasa de «el que manda cosas que suenan a ChatGPT» a «el que escribe claro y rápido». El jefe deja de citarle por diapositivas genéricas (C27). **[ANCL + HIP]**
- **Con los clientes:** las respuestas vuelven a ser conversación, no trámite. Desaparece el «¿esto lo has escrito tú?» (F1). **[ANCL]**
- **Con los compañeros:** deja de ser parte del problema de la «bandeja llena de slop» (C7, C10). **[ANCL indirecto]**
- **Consigo mismo:** recupera la sensación de que lo que firma es suyo (F3, A9). **[ANCL]**
- **En casa** **[HIP]**: deja de cerrar el portátil a las once con la sensación de haber trabajado dos veces el mismo email.

**Frases específicas post-transformación** (lo que se diría o le dirían):
1. «Le he pedido a ChatGPT el email de la reclamación y lo he mandado tal cual. Tal cual. Ni una coma.» **[HIP con anclaje A31, F2]**
2. «El lunes me dijo el cliente "da gusto leerte". Y lo había escrito con la IA en tres minutos.» **[HIP, inversión de F1]**
3. «Ya no abro tres pestañas. Escribo, leo y envío.» **[ANCL A21, inversión]**
4. «Mi jefe ha dejado de reenviarme los emails con comentarios en rojo.» **[HIP con anclaje A5, A8]**

---

### Las tres capas de motivación

**Motivación funcional** (la tarea concreta): que la IA que ya usa escriba **a la primera** textos que no hay que reescribir y que suenan a una persona concreta (él), sin herramientas externas ni pasos adicionales cada vez.
1. «Quiero pegarle el borrador del email al cliente a las nueve de la mañana y que lo que me devuelva lo pueda mandar a las nueve y cinco, no a las nueve y media.» **[ANCL F2, A20]**
2. «Quiero que deje de meterme en cada email el "no dudes en contactarme" y el "espero que estés bien" que no he dicho en mi vida.» **[ANCL E13 «please don't hesitate to reach out», A4 · versión española HIP]**

**Motivación emocional** (lo que siente): **alivio** (dejar de vigilar), **tranquilidad** al darle a enviar y **orgullo recuperado** («esto es mío»).
1. «Lo que quiero es darle a enviar sin ese nudo de "a ver si se nota", y no pasarme la tarde mirando si ha contestado.» **[ANCL F6, F2 · anclaje corporal HIP]**
2. «Quiero volver a leer algo que he mandado y reconocerme, no pensar "esto no lo he escrito yo".» **[ANCL F3, A9]**

**Motivación social** (cómo le ven los demás). Casi nunca se verbaliza y se infiere de quién sabía de la decisión y qué dijo:
1. «No quiero ser la del equipo de la que todos saben que lo pasa todo por ChatGPT, la que cuando escribe "gracias" ya nadie se lo cree.» **[ANCL C13, C15, E30 · desde el lado del juez, invertido]**
2. «Delante del cliente quiero seguir siendo yo, el que conoce su negocio, no uno más que le manda plantillas. Porque el día que lo huela me pide descuento o se va con otro.» **[ANCL E19, C11, F7]**

**Nota:** la motivación social está inferida casi siempre **a partir de los jueces** (bloque C), porque los emisores casi nunca cuentan qué pensaron los demás de ellos, salvo cuando hubo un comentario directo (A5, C27, F1, F7). Es la capa de más impacto y la de menor base directa. **Requiere validación en entrevistas, con preguntas indirectas:** «¿Quién de tu trabajo sabe que usas ChatGPT para escribir? ¿Qué crees que piensa?».

---

### Pulso del mercado (5 necesidades eternas)

| Motor | ¿Relevante? | Intensidad (1-10) | Frase del prospecto | Base |
|---|---|---|---|---|
| **Pertenecer** | Sí, moderado: «ser de los que usan la IA bien», no de los «vagos» que copian y pegan | 5 | «No quiero ser de los que mandan el email con la frase de ChatGPT pegada al final. Quiero ser de los que la usan y no se nota.» | **[ANCL E29, E35, E36]** |
| **Escapar** | Sí, alto: del bucle de reescritura, del ciclo de pestañas, de la vigilancia constante | 8 | «Quiero dejar de pasarme media hora con cada email preguntándome si suena a mí o a la máquina.» | **[ANCL F2, F6, A21]** |
| **Aspirar** | Sí, moderado: parecer alguien que escribe claro, rápido y con criterio propio | 5 | «Quiero que me lean y piensen "qué bien escribe", no "qué bien escribe ChatGPT".» | **[HIP, inversión de F1/F7]** |
| **Entender** | Sí, alto **para el recién llegado**: por qué suena a IA, qué es lo que «chirría» | 7 | «Por fin entendería qué es eso que se nota y que yo no sé ni nombrar.» | **[ANCL C23 «even if they can't put finger on exactly what it is», A35]** |
| **Ser entendido** | Sí, alto: nadie habla del que no es técnico, nadie le explica las cosas a su ritmo | 7 | «Todo lo que encuentro es para gente que sabe de esto. Prompts, tokens, APIs… yo solo quiero que el email no suene a robot.» | **[ANCL A36, E46 + HIP de vocabulario]** |

**Motor dominante: ESCAPAR**, seguido de cerca por **Entender** (en el recién llegado).
**Por qué:** es el motor con más base empírica entre los emisores ante personas (la reescritura domina con ≈ 45 %) y el que encaja con la palabra clave del producto: «**una vez**». El comprador no busca subir de estatus. Busca **salir** de un bucle que le cuesta tiempo cada día y le tiene en vigilancia constante. *Entender* es el **puente** hacia la solución, porque explica el bucle y da control, pero el titular y el lead deben estar presididos por la salida del bucle. *Ser entendido* debe impregnar el tono (calma, «no tienes que saber nada técnico»), no el ángulo.

---

### Mass Desire dominante (Schwartz)

**Mass Desire dominante:** **«Usar la IA sin que se note»**, es decir, beneficiarse de lo que la IA ahorra sin pagar el precio social de que lo que firmas suene a máquina.

Es la fuerza social que mueve a millones de personas en la misma dirección. En 2026 casi todo el mundo que trabaja delante de un ordenador usa o ha probado la IA para escribir, y casi todo el mundo ha aprendido a detectar (y despreciar) el texto que «huele» a IA. El corpus lo formula con exactitud desde el lado del juez: **«Nobody cares if you use AI… What people hate is when your posts look obviously AI generated or sound robotic»** (E35). También: «have it write the email, and then rewrite it in your own words» (E36); «Use of AI… will alienate people» (A2).

| Dimensión | Puntuación | Justificación |
|---|---|---|
| **Urgencia** | 7/10 | Se vive cada día, con cada texto (frecuencia alta). Pero no es un dolor agudo constante: se agudiza tras un incidente (comentario del jefe o del cliente) y luego se adormece en «lo reescribo y ya». |
| **Staying power** | 8/10 | El deseo de «no parecer falso / que lo mío sea mío» es perenne, porque es autenticidad, reputación y estatus. La forma concreta («que no se note la IA») durará mientras los modelos tengan voz por defecto reconocible. Hay riesgo: si los modelos se vuelven indistinguibles, la urgencia baja. Pero el corpus muestra lo contrario (A34: «Claude ha empeorado hasta parecer el primer GPT»; A33: patrones «casi imposibles de eliminar»). |
| **Scope** | 8/10 | Afecta a cualquier persona que escribe en el trabajo con IA, no solo a copywriters. El corpus incluye abogados, managers, RR. HH., marketing, SaaS, freelancers, periodistas, ghostwriters, pequeños negocios, docentes (A16) y comercio (C23). |

**Justificación frente a las dos motivaciones más fuertes descartadas:**

1. **Descartada: «Dejar de perder tiempo reescribiendo»** (eficiencia). Es la más frecuente entre los emisores (≈ 45 %) y la más fácil de demostrar. **Pierde** porque es una consecuencia, no la causa: la gente reescribe **porque** teme que se note. Si nadie fuera a notarlo, mandarían el texto tal cual. Además, «ahorra tiempo» es la promesa agotada de toda la categoría de la IA (ver Schwartz). **Uso:** body copy y justificación lógica.
2. **Descartada: «Recuperar mi propia voz»** (identidad, «que suene a mí»). Es potente y emocionalmente rica (A4, A22, F3, F4), pero **pierde en scope**: es más fuerte en escritores, creadores, copywriters y profesionales de la comunicación, que se acercan al perfil insider. El adulto de 35 a 60 años que escribe emails a clientes no se piensa a sí mismo como alguien «con una voz». Se piensa como alguien que «no quiere quedar mal». **Uso:** promesa secundaria y mecanismo («enseñarle cómo hablas tú»). Es la *forma* de conseguir el deseo de masa, no el deseo en sí.
3. (Descarte adicional) **«Pasar el detector / ser indetectable»**: frecuente en el corpus (≈ 25 entradas), pero pertenece al segmento estudiante/detector. Su motivación es distinta, choca con el producto y con la ética del posicionamiento, y está asociada a la categoría más desprestigiada (los humanizadores). Va al anti-persona.

**Implicación operativa:** el titular y el lead hablan de **que no se note** (o de que la gente deja de notarlo). El ahorro de tiempo y la voz propia son material de body copy. Si el titular promete «ahorra horas», compite con todos los vendedores de IA. Si promete «suena a ti», solo resuena con los que ya se piensan como escritores.

---

### Disparador situacional (Priority Initiative)

**¿Qué pasó exactamente?** El paso del «algún día lo arreglo» al «necesito arreglarlo ya» llega, según el corpus, por cuatro vías, ordenadas por peso para el comprador principal:

1. **Un comentario directo de una persona con poder sobre él** (jefe o cliente): «suena a ChatGPT» (F7), «¿esto lo ha escrito ChatGPT?» (F1), el jefe que lo cita para hablar de la diapositiva (C27) o que repite que sus emails suenan a IA (A5). **Es el detonante más nítido y el más triangulado.**
2. **La vergüenza de un error visible:** se le queda pegada la frase meta del asistente en un email («am I cooked 😭», B22; «It's so embarrassing», E33). Es minoritario, pero de intensidad máxima.
3. **El hartazgo acumulado del propio emisor:** la tercera reescritura del mismo mensaje (F3), la media hora por un email de cinco minutos (F2), el límite de uso consumido corrigiendo tonos (A28), el *cringe* tras el octavo intento (A27). No hay un tercero: el detonante es **él mismo** diciendo «hasta aquí».
4. **Verse en el espejo del otro:** recibir un email de IA de un compañero o proveedor, sentir el rechazo (C1, C4, E48) y pensar de repente: «¿y si los míos suenan igual?». **[ANCL bloque C + HIP del giro introspectivo]**. El corpus tiene muchísimos jueces, pero ninguno cuenta este giro de forma explícita.

**¿Quién o qué fue el detonante?** En las vías 1 y 2, **un tercero** (jefe, cliente, compañero o el propio error visible ante otros). En las vías 3 y 4, **él mismo**. Para el comprador principal, el peso relativo estimado es: tercero ≈ 55 %, él mismo ≈ 45 %. **[HIP de proporción]**

**¿Qué estaba tolerando antes que dejó de tolerar?** La **duda privada**. Antes del detonante sabía, o sospechaba, que «a veces suena un poco a IA», pero lo resolvía reescribiendo en silencio. El detonante convierte la duda privada en **exposición pública**: otro lo ha visto. A partir de ahí la reescritura silenciosa ya no basta, porque **ya no se fía de su propio criterio para saber si se nota**.

**3 frases en primera persona, crudas, del momento de quiebre:**
1. «El cliente me contestó al presupuesto con una sola línea: "¿Esto lo ha escrito ChatGPT?". Y lo peor es que esa vez lo había escrito yo. Me quedé mirando la pantalla con la cara ardiendo.» **[ANCL F1 · sensorial HIP]**
2. «Mi jefe me llamó al despacho por la presentación. "Está bien que uses la IA, pero tiene que ser tu trabajo." Volví a mi mesa y estuve una hora sin poder escribir ni un correo.» **[ANCL C27 · temporal HIP]**
3. «Lo vi en la bandeja de enviados a las ocho y diez: había mandado al cliente el email con el "Claro, aquí tienes una versión más profesional:" de ChatGPT arriba del todo. Ahí dije: o aprendo a usar esto bien o lo dejo.» **[ANCL B22, E33 · temporal HIP]**

---

### La frase exacta del segundo anterior

**Si llega desde Google** (búsqueda activa, normalmente tras un incidente) **[HIP en el vocabulario de búsqueda en español; ANCL en la intención]**:
- «cómo hacer que chatgpt no suene a chatgpt»
- «chatgpt escribe como un robot cómo arreglarlo»
- «cómo hacer que chatgpt escriba como yo»
- «humanizar texto chatgpt gratis»: ojo, esta búsqueda lleva directamente a los humanizadores.

**Si llega desde redes sociales** (scroll pasivo, por la noche o entre tareas) **[ANCL]**:
- Pensamiento de fondo tras releer un email suyo o tras recibir uno de IA de otro.

**Si llega por recomendación** **[HIP]**:
- «Mira esto, que tú siempre estás con lo de que ChatGPT te escribe como un folleto.»

**8 frases candidatas en primera persona, en el vocabulario del mercado y sin filtrar:**
1. «¿Por qué todo lo que me escribe ChatGPT suena a ChatGPT?» **[ANCL A1, A27]**
2. «Otra vez reescribiendo el email entero. Para esto no me hacía falta la IA.» **[ANCL A31, E22]**
3. «¿Se notará que esto lo ha escrito la máquina?» **[ANCL F2, F6]**
4. «Le he dicho mil veces que no suene a robot y sigue igual.» **[ANCL A26, A27, E12]**
5. «No quiero que el cliente piense que le mando cualquier cosa.» **[ANCL F1, F7, E19]**
6. «Seguro que hay una forma de configurar esto y yo no tengo ni idea.» **[ANCL A35, A36, E53]**
7. «Esto no suena a mí. Yo no hablo así.» **[ANCL A4, F3]**
8. «Como mi jefe me vuelva a decir que suena a ChatGPT…» **[ANCL A5, A7]**

**La más probable: la n.º 1, «¿Por qué todo lo que me escribe ChatGPT suena a ChatGPT?».**
**Por qué:** (a) usa la palabra exacta del mercado («suena a ChatGPT» es el patrón D1, el más repetido del corpus); (b) es una **pregunta**, y el recién llegado está en modo «entender» (motor secundario), no en modo «comprar»; (c) contiene una pequeña frustración («todo», «siempre») sin exigir un incidente previo, así que sirve para tráfico frío en *Passive Looking*; (d) conecta de forma natural con la primera pieza del producto (el PDF que explica **por qué**); (e) no da por sentado que se sepa nada técnico. **Es la candidata a primera línea de la carta.** Variante de segunda prioridad para tráfico que viene tras un incidente: la n.º 3, «¿Se notará que esto lo ha escrito la máquina?».

**Advertencia:** todas son traducciones-adaptaciones **[ANCL]**. Antes de usarlas como titular conviene validar con search data en español (volumen de «suena a chatgpt», «no suene a chatgpt» o «escribir como humano chatgpt») y con comentarios reales de YouTube o Facebook.

---

### Predicción del lector y diseño al revés de la emoción objetivo

**Predicción por canal:**

| Canal | Qué predice el lector típico al encontrarse con esta categoría | Base |
|---|---|---|
| **Anuncio en redes (Instagram, Facebook, LinkedIn)** | «Otro vendedor de prompts.» «Otro que dice que con su truco ChatGPT escribe como un humano.» Predice **hype**, una lista de «10 prompts secretos» y luego un curso de 200 €. En LinkedIn predice al creador de contenido que vende su método. | **[HIP con anclaje E53, F6, D1]** |
| **Landing tras búsqueda en Google** | Si ha buscado «humanizar texto», predice **otra web de humanizador**: una caja donde pegar el texto, un porcentaje de «humano», una suscripción. Si ha buscado «cómo hacer que ChatGPT no suene a ChatGPT», predice **un artículo de blog** con una lista de palabras prohibidas y prompts. | **[ANCL D-bloque, E-bloque]** |
| **Email** | Si está en la lista del creador: confianza moderada, pero predice «otro producto de IA». Si es frío: lo borra en segundos (C17, que borra 30-40 por semana porque reconoce la «falsa efusividad» de la IA). **Riesgo enorme: un email que venda «escribe como un humano» y suene a IA se autodestruye.** | **[ANCL C17, E13]** |
| **Vídeo corto** | Predice un tutorial gratis: «pega esto en tus Instrucciones personalizadas» (E53). Si ya lo ha visto, predice que no funciona (A26). | **[ANCL E53, A26]** |

**Contaminación de predicción** (lo que le hace pensar «otra promesa vacía» antes de leer la primera línea):
- **«100 % humano», «indetectable», «pasa todos los detectores»**: es el lenguaje de los humanizadores (D12, D18, D31), desacreditado por las reseñas.
- **«Con este prompt ChatGPT escribirá como un humano»**: la promesa del prompt mágico, desmentida por la experiencia de A20, A26 y E12.
- **«Clona tu voz»**: desmentido por A30 («tras probar humanizadores, clonadores de voz y prompts de estilo… sabe que tendrá que reescribirlo»).
- **«Ahorra 10 horas a la semana con IA»**: la promesa genérica de productividad de toda la industria. **[HIP]**
- **La estética del gurú de la IA** (fondos oscuros con neón, «IA» con mayúsculas por todas partes, cuentas atrás). **[HIP]**
- **Cualquier texto de venta que suene a IA**: si la landing usa el «En el vertiginoso mundo actual…», pierde a la primera frase. **Es la contaminación más letal y la más probable, porque el propio copy de la categoría está escrito con IA.**

**Emoción objetivo concreta:** **el alivio de reconocimiento**. Es la sensación de «vale, no soy yo, no soy torpe: le pasa a todo el mundo, y hay una razón concreta por la que me pasa», seguida inmediatamente de un **«esto lo puedo hacer yo»**. Formulado con granularidad: *«el alivio de quien llevaba meses reescribiendo cada email a escondidas, creyendo que el problema era su torpeza con la tecnología, y descubre en un párrafo que el problema tiene nombre, tiene cuatro causas y se arregla una sola vez dentro de su propio ChatGPT»*.

**Predicciones que hacen probable esa emoción:**
1. Que el lector prediga que **le van a explicar algo**, no que le van a vender algo. El formato tiene que parecer una explicación (problema, causa, demostración) y no un anuncio.
2. Que prediga que **es para gente como él** (no técnica). Necesita señales tempranas: «sin programar», «dentro de tu ChatGPT», «si sabes copiar y pegar».
3. Que prediga que **no le van a cobrar nada recurrente**. La señal «pago único» tiene que aparecer pronto.
4. Que prediga **honestidad**: que no le prometan «indetectable», sino algo modesto y verificable («que deje de sonar a plantilla»).

**Decisión: ROMPER la predicción** en los tres primeros segundos.
**Por qué:** la predicción que trae el lector («otro vendedor de prompts o de humanizadores») es **incompatible** con la emoción objetivo (alivio y «puedo hacerlo»). Si el copy la valida (titular de promesa, cifra, «indetectable»), el lector la categoriza como sospecha. Hay que romperla con uno de estos patrones: (a) **la paradoja de E12**: «Si le pides a ChatGPT que no suene a ChatGPT, suena más a ChatGPT»; (b) **la verdad incómoda de E35**: «A nadie le molesta que uses IA. Le molesta que se note»; o (c) **escribir la propia landing con una voz tan humana que el contraste sea la prueba**: el texto de venta es la demostración del producto.

Esta capa informa a Schwartz (abrir con la paradoja como «Secreto») y a Sugarman (la primera frase existe para que se lea la segunda).

---

### Tarea vital (etapa de vida dominante)

**Tarea dominante: CONSOLIDACIÓN / CONTROLAR**, con un componente secundario de **SIMPLIFICACIÓN / CERRAR**.

**Por qué:** el comprador principal, de 38 a 55 años, en plena vida laboral, no está construyendo nada desde cero (agencia) ni buscando entrar en un grupo (pertenencia). **Ya tiene una posición** (un puesto, una cartera de clientes, una reputación) y la IA ha aparecido como una amenaza a la vez que como una herramienta. Lo que quiere es **mantener el control de su imagen profesional** sin tener que convertirse en experto en algo nuevo. El componente de simplificación aparece en el deseo de «una vez y no volver a pensar en esto» y en el rechazo a sumar herramientas, pestañas y suscripciones (A21, D8, D25). **[ANCL + HIP de etapa vital, porque no hay datos de edad]**

**¿Cómo cambia el criterio de compra según esta tarea?**
- Busca **certeza y estructura**: pasos cerrados, un resultado previsible y la garantía de que no se rompe nada.
- Busca **reversibilidad**: poder deshacerlo si no le gusta. **[HIP]** Saber que borrar unas instrucciones personalizadas devuelve ChatGPT a como estaba es un dato tranquilizador muy potente.
- Rechaza **el aprendizaje abierto** («aprende a dominar la IA») y prefiere **la solución cerrada** («deja esto configurado»).
- Valora **no depender de terceros** (encaja con el diferencial: «tu IA, gratis a partir de ahí»).

**¿Qué tono activa y cuál rechaza?**
- **Activa:** calma, claridad, cercanía de igual a igual, honestidad sobre lo que hace y lo que no. El tono de «te lo explico como se lo explicaría a un amigo listo que no es técnico».
- **Rechaza:** euforia tecnológica («¡la IA lo va a cambiar todo!»), jerga, urgencia artificial, el tono juvenil o de *growth hacker*, la condescendencia («es facilísimo, cualquiera lo hace») y el miedo apocalíptico («la IA te va a quitar el trabajo»).

**2 frases en primera persona que expresan esa tarea vital en relación con este producto:**
1. «A estas alturas no voy a ponerme a aprender a programar. Lo que quiero es dejar esto bien configurado una tarde de domingo y que el lunes funcione sin acordarme.» **[HIP con anclaje A36 · temporal HIP]**
2. «Me ha costado veinte años que mis clientes se fíen de mí. No voy a dejar que un email con pinta de robot me lo estropee.» **[ANCL C11 (relación de más de 20 años, invertida al emisor) + HIP]**

---

### Otras soluciones

**Qué han probado en el pasado (5 soluciones distintas):**

| # | Solución probada | Base | Resultado reportado |
|---|---|---|---|
| 1 | **Pedirle en cada mensaje que «suene más natural / humano / casual»** | A20, A25, A26, E12, E24 | La cadencia impecable vuelve en los textos largos (A25). Si le dices que «no suene a IA», mete aún más clichés (E12). |
| 2 | **Darle instrucciones, ejemplos de su propia escritura o Instrucciones personalizadas** | A19, A26, A27, A29, A30 | Funcionan al principio y se degradan en la conversación (A19). Tras 6-8 prompts con ejemplos, sigue sonando «terribly AI» (A27). Las listas de patrones prohibidos quitan tics, pero no ponen personalidad (A29). |
| 3 | **Herramientas humanizadoras de pago** (Undetectable.ai, StealthGPT, BypassGPT, Humbot, Walter Writes, HIX Bypass, WriteHuman, BypassAI, BypassDetection) | D1-D42 | Siguen detectadas, destrozan el sentido, cobran de forma opaca, son lentas y el soporte no responde. |
| 4 | **Reescribirlo a mano** después de generarlo | A1, A4, A22, A23, A31, F3 | Funciona, pero anula el ahorro de tiempo: «basically rewriting it anyway» (A31). |
| 5 | **Meter imperfecciones deliberadas** o empobrecer el lenguaje (frases más simples, errores a propósito, quitar rayas y punto y coma) | A6, A24, B5, B21, F2, E7 | Le da inseguridad y vergüenza («¿vuelvo atrás y cometo faltas?», B21). Algunos se niegan («dumb ourselves down», E7). |
| (6) | **Trucos de «identidad falsa»** («di que el inglés es tu segunda lengua») | E25 | Truco casero, sin evaluación de resultado [FUENTE ÚNICA]. |
| (7) | **Alimentarla con cientos de textos propios** para que imite el estilo | E18 | «desperately fed ChatGPT 100's of emails». La palabra *desperately* lo dice todo. [FUENTE ÚNICA] |
| (8) | **Clonadores de voz / prompts de estilo / herramientas de terceros con «tu voz»** | A30 | Tras una semana, sabe que tendrá que reescribirlo entero. |

**Frases que usarían para describir esas soluciones fallidas:**
- Sobre pedir «que suene natural»: «Le pedí que sonara natural y me devolvió un folleto de agencia de viajes.» **[ANCL A20, A26 · imagen HIP]**
- Sobre las instrucciones: «Funciona tres mensajes. Al cuarto vuelve a ser el de siempre.» **[ANCL A19]**
- Sobre los humanizadores: «Pagué para que lo hiciera humano y me lo devolvió con palabras que no existen y mayúsculas en medio de la frase.» **[ANCL D23, D40]** / «Es una estafa de 20 dólares. Mira las reseñas.» **[ANCL D1, D6]**
- Sobre reescribir a mano: «Al final lo reescribo yo, así que dime tú para qué uso la IA.» **[ANCL A31, E22]**
- Sobre la imperfección deliberada: «He llegado a meter una falta a propósito para que se vea que es mío. Fíjate a lo que he llegado.» **[ANCL B21, F2]**

**Soluciones populares en el mercado actual:**
1. **Humanizadores de texto por suscripción** (los nueve citados y otros). Es la solución más visible en publicidad y SEO. **[ANCL D-bloque]**
2. **Listas de «palabras y frases que delatan a la IA»** en blogs, LinkedIn y TikTok. **[ANCL E1-E12]**
3. **Packs de prompts** («50 prompts para que ChatGPT escriba como un humano»). **[HIP, coherente con E24]**
4. **Plantillas gratuitas de Instrucciones personalizadas** en YouTube, TikTok o Shorts («pega esto en tus ajustes»). **[ANCL E53]**
5. **Detectores de IA para «comprobar» el texto** (GPTZero, ZeroGPT, Turnitin, Pangram, el detector de Grammarly, QuillBot). Más que solución, se usan como medidor. **[ANCL B18, D12]**
6. **Parafraseadores y correctores con IA** (QuillBot, Grammarly). **[ANCL D12, B12-B13 · HIP de uso en el target]**

**Principales objeciones a esas soluciones:**
- **Humanizadores:** no funcionan (D7, D15-D18), destrozan el texto (D19, D30, D34), son caros (D4, D36, D39), cobran de forma opaca (D8, D14, D25), son lentos (D37), el soporte es pésimo (D24, D41) y se rompen con cada actualización de los detectores (D28, D29).
- **Listas de palabras:** quitan tics pero no ponen voz (A29). Evitarlas también puede sonar a IA (E9). Los tics cambian con cada versión del modelo (*delve* y *tapestry* son de 2023-2024; en 2026 se quejan de «frases cortadas» y «cadencia entrecortada», A33). **[ANCL + inferencia temporal]**
- **Packs de prompts:** hay que pegarlos cada vez (el ciclo de pestañas, A21) y se degradan (A19). **[ANCL + HIP]**
- **Plantillas de Instrucciones personalizadas:** son genéricas, no saben cómo hablas tú (A29) y a veces simplemente no funcionan (A26). **[ANCL]**
- **Detectores:** se contradicen: el mismo texto da 0 %, 40 % y 100 % (B18) y oscilan «entre 0 y 100 pese a miles de modificaciones» (B20). Además, el lector humano no usa detector: usa el olfato (C23). **[ANCL]**
- **Correctores y parafraseadores:** pueden **convertir en IA** un texto humano. B12: usó ChatGPT para mejorar la gramática y Turnitin lo marcó. A8 y C9: el jefe y RR. HH. pasan el texto humano por IA y lo vuelven «slop».

---

### La opción «no comprar nada»

**¿Qué gana el prospecto si no compra nada?**
- Ahorra 29 €.
- **No se arriesga a otra decepción** (o a otro cargo raro, D14, D25).
- **No tiene que enfrentarse a los ajustes de ChatGPT**, que nunca ha tocado. **[HIP]**
- **No tiene que admitir que lo estaba haciendo mal.** Comprar es reconocer el problema. **[HIP]**
- Mantiene su sistema actual, que **funciona lo suficiente**: reescribe a mano, revisa tres veces y «tira» (A1, E33).
- Conserva la excusa de que «la IA es así», que le libra de responsabilidad sobre el resultado. **[HIP]**

**¿Qué se dice a sí mismo para justificar la inacción indefinida?**
- «Total, lo retoco un poco y ya está.» **[ANCL A4, A23]**
- «Seguro que en la próxima versión de ChatGPT esto ya viene arreglado.» **[HIP con anclaje A34: la percepción de que los modelos cambian]**
- «Si ni los que saben de esto lo arreglan con prompts, yo menos.» **[ANCL A29, A33]**
- «Ya buscaré algo gratis en YouTube.» **[ANCL E53]**
- «Tampoco me ha pillado nadie… todavía.» **[HIP]**

**¿Qué coste real está asumiendo sin saberlo al no hacer nada?**
- **El tiempo.** Lo reconocería si lo sumara: si tarda media hora en vez de cinco minutos en cada email importante (F2), y escribe tres o cuatro al día, son entre 1 y 1,5 horas diarias **retocando lo que la máquina debía ahorrarle**. **[ANCL F2 + cálculo HIP]**
- **La vigilancia de fondo**: la tensión de «¿se notará?» cada vez que le da a enviar (F6, casi a diario).
- **La reputación invisible**: los jueces no siempre lo dicen a la cara. Lo comentan entre ellos (C12, C15, E30) o simplemente borran sin leer (C17). **Puede que ya le estén juzgando sin que lo sepa.** El prospecto reconocería este coste como real porque él mismo ha sido ese juez.

**¿Qué evento o umbral haría insostenible seguir sin actuar?**
- El **comentario directo** del jefe o del cliente (Disparador situacional, vía 1).
- El **error visible** (la frase meta pegada, vía 2).
- Un **texto de alto riesgo** en el horizonte: una propuesta importante, una candidatura, una presentación ante dirección, una carta de reclamación. **[HIP]**
- **La orden de arriba de «usar IA para todo»** (E15: el compañero que presiona para usar la herramienta de IA incluso en emails de dos frases; C14: el CEO fanático de la IA; C23: el jefe que pregunta «por qué no podemos usar IA para todo»). Si la empresa le obliga a usar IA, el problema de que se note se multiplica. **[ANCL]**

**2 frases en primera persona que expresan la comodidad del statu quo:**
1. «Bah, lo repaso un poco antes de mandarlo y ya. Llevo así todo el año y no me ha dicho nadie nada… creo.» **[ANCL A4, E33 · temporal HIP]**
2. «Ya lo miraré en verano, cuando tenga una tarde tranquila. Ahora con el cierre de trimestre no estoy para aprender cosas nuevas.» **[HIP: anclaje temporal construido, sin base directa]**

---

### Ruta de decisión

**Secuencia de pasos** **[ANCL para los pasos 1-4; HIP para la parte de compra, porque el corpus no documenta compras de infoproductos]**:
1. **Nota el problema** (por sí mismo o por un comentario). Empieza a reescribir más.
2. **Lo intenta arreglar dentro del propio chat**: «que suene natural», «más casual», «no suenes a IA» (A20, A26, E12). Primera decepción.
3. **Busca en Google o pregunta en un foro o a un compañero** (A26: «How do I make GPT sound like a real modern human?»; A27: «How do I make it write better?»). Encuentra dos tipos de resultados: humanizadores (anuncios y SEO) y listas de palabras.
4. **Bifurcación:**
   - 4a. Prueba un humanizador (la prueba gratuita, D13) → decepción o cargo inesperado → **desconfianza hacia cualquier solución de pago** de la categoría.
   - 4b. Prueba una plantilla o un truco gratis (E24, E25, E53) → resultado parcial o degradación → **desconfianza hacia «los trucos»**.
5. **Vuelve a reescribir a mano** (statu quo) y deja el problema «aparcado».
6. **Nuevo detonante** → búsqueda o atención renovada, ahora más escéptica.
7. **Encuentra la oferta** (anuncio, contenido del creador, recomendación). **[HIP]**
8. **Evalúa:** ¿es otra herramienta?, ¿hay que pagar cada mes?, ¿hay que saber programar?, ¿hay un ejemplo con textos como los míos?
9. **Último paso antes de comprar:** buscar una señal de que **no es una estafa** (una cara, una garantía, la confirmación de que es pago único) y una señal de que **podrá hacerlo él** (una captura, un vídeo corto del paso a paso). **[HIP]**

**Filtro de preselección (lista corta mental):**
- **Entra en consideración si:** (1) funciona **dentro de su ChatGPT/Claude**; (2) **pago único** o gratis; (3) parece **para gente normal**, no para programadores; (4) lo explica alguien que **se nota que escribe bien** (la propia landing es la prueba).
- **Queda excluido automáticamente, aunque sea bueno, si:** (1) lleva las palabras «humanizador», «bypass», «indetectable» o «100 % humano» (lo asocia con estafa, D-bloque); (2) pide **instalar** algo sin explicar qué es; (3) menciona **API, código, terminal, tokens, agentes**; (4) es **suscripción**; (5) **la propia página suena a IA**. **[ANCL + HIP]**
- Este filtro es crítico para el tráfico frío: **la palabra «plugin»**, que forma parte del formato del producto, puede activar la exclusión 2. Hay que nombrarlo de otra forma en la parte superior de la página (por ejemplo, «una guía que te lleva de la mano dentro de tu propio ChatGPT») y explicar el plugin o skill más abajo, con capturas. **[HIP, a testear]**

**¿Dónde busca información?** Google (búsqueda directa), Reddit (sobre todo en inglés, en el corpus), YouTube (tutoriales cortos, E53), LinkedIn (posts de creadores, F-bloque), Trustpilot (para comprobar herramientas, D-bloque). **[ANCL]** **[DATO INSUFICIENTE]** para el hispanohablante: probablemente Google, YouTube en español, Facebook (grupos), Instagram, LinkedIn en español y **el compañero de trabajo que «sabe de esto»**. **[HIP]**

**¿A quién consulta antes de decidir?** **[DATO INSUFICIENTE]**. El corpus no documenta consultas previas a una compra. **Hipótesis basada en mercados similares:** al compañero de trabajo más joven o más técnico («oye, tú que sabes de esto»), al hijo o la hija («mamá, eso lo puedes hacer en los ajustes»), o a nadie (compra discreta, por pudor). La compra discreta es probable, por la motivación social de que no se sepa que necesita ayuda. **[HIP]**

**¿Qué hace que descarte una opción? (momento de descarte):**
- Ver que se renueva sola o que no queda claro cuánto cuesta (D14, D25).
- Leer en Trustpilot o en Reddit «it's a scam», «look at the reviews» (D1, D6).
- Ver un ejemplo de «antes y después» en el que el «después» también suena a IA. **[HIP]**
- Ver jerga técnica en las primeras líneas. **[HIP]**
- Que la oferta prometa «indetectable» (para el comprador adulto honrado suena a trampa y a estafa). **[ANCL + HIP]**

**¿Qué le da el último empujón para comprar?**
- La **demostración**: ver un email suyo, o uno muy parecido, reescrito por una IA configurada, frente a la versión por defecto. **[HIP con anclaje en el patrón «antes/después» de toda la categoría]**
- **Pago único y bajo** frente a los 20, 60, 180 o 200 $ de los humanizadores. **[ANCL D-bloque]**
- **Garantía de devolución sin preguntas.** **[HIP]**: es especialmente potente aquí porque el agravio n.º 1 de la categoría es «me ofrecieron créditos en vez de devolverme el dinero» (D10).
- La frase «**una vez, y es tuyo para siempre, dentro de tu propia IA**».

**3 frases en primera persona que describen cómo vive el proceso:**
1. «Estuve un domingo por la tarde mirando webs de esas de "humaniza tu texto". Todas te piden la tarjeta antes de enseñarte nada. Cerré todas.» **[ANCL D13, D14 · temporal HIP]**
2. «Le pregunté a mi compañero, el que siempre está con estas cosas, y me pasó un vídeo de TikTok con unas instrucciones para pegar en los ajustes. Funcionó dos días.» **[ANCL E53, A19 · HIP de escena]**
3. «Antes de pagar busqué el nombre en Google con la palabra "estafa". Ya me han pillado una vez.» **[ANCL D1, D25 + HIP de comportamiento]**

**Dark Broadcasters (difusores invisibles):**
- **Creadores de LinkedIn que hablan de «sonar humano»** (F2, F4, F6: content mentors, ghostwriters, consultores de marca personal). El prospecto los percibe como «profesionales como yo», no como publicidad. **[ANCL]**
- **Tutoriales cortos de YouTube, TikTok o Shorts** del tipo «el truco para que ChatGPT no suene a ChatGPT» (E53). **[ANCL]**
- **Newsletters de productividad y de IA para no técnicos.** **[HIP]**
- **Los propios hilos de Reddit** en el caso del público anglófono (r/ChatGPT, r/ClaudeAI). **[ANCL]**
- **El algoritmo de recomendación**: quien ha buscado «ChatGPT suena a robot» empieza a ver anuncios de humanizadores. **[HIP]**
- **[DATO INSUFICIENTE]**: los nombres propios de influencers de IA en español que sigue el target de 35 a 60 años no salen en el corpus.

**Plataformas-radar:**
- **Trustpilot**: el corpus muestra que es **el tribunal** de la categoría de humanizadores. Una mala nota en Trustpilot elimina cualquier opción (D-bloque). **[ANCL]**
- **Reddit** como verificador de «¿esto es legit?» (D4: «Undetectable AI review is it legit»; D3: «How legit is BypassGPT»). **[ANCL]**
- **Los «mejores humanizadores de 2026»** y las listas de comparativas SEO. **[HIP]**
- **Para el hispanohablante [DATO INSUFICIENTE]:** probablemente reseñas en Google, comentarios en YouTube y la opinión de un grupo de Facebook. **[HIP]**

**Voz pública frente a voz online:**
- **Cara a cara (práctico, contenido):** «Sí, uso ChatGPT para los emails, pero luego los repaso.» Lo presenta como un uso responsable y bajo control. **[HIP con anclaje E34, E36]**
- **Online (identitario, emocional):** «It is driving me crazy!» (A1), «I hateee it!!» (A5), «It's so embarrassing 😭😭😭» (E33), «am I cooked 😭» (B22). Exasperación, vergüenza, miedo.
- **La diferencia revela el motor real:** en persona proyecta **control**; a solas, o en el anonimato, admite **pérdida de control y vergüenza**. El motor de compra real es **recuperar el control sin tener que confesar que lo había perdido**. Consecuencia para el copy: la compra debe poder justificarse en público como «optimizar mi forma de trabajar», no como «arreglar que me pillaban».

---

### Solución ideal

**Qué NO quieren hacer para resolver su problema:**
- **Aprender a programar** ni tocar herramientas de código (definición del target).
- **Pagar una suscripción mensual** a otra herramienta (D8, D14, D25, D36).
- **Pasar el texto por otra web** después de escribirlo, con otra pestaña, otro copiar y pegar (A21).
- **Reescribirlo todo a mano** (A31).
- **Empobrecer su forma de escribir** ni meter faltas a propósito (E7, B21).
- **Aprender una lista de 200 palabras prohibidas** y vigilarlas una por una. **[ANCL A29, E9 + HIP]**
- **Ver un curso de 10 horas.** **[HIP]**
- **Dar sus datos o subir sus documentos** a un servicio desconocido. **[HIP; C21 apunta al miedo a la seguridad corporativa]**

**Frases conversacionales sobre lo que no están dispuestos a hacer:**
- «Yo no me pongo a aprender código a estas alturas, ni loco.» **[HIP]**
- «Otra suscripción no. Ya tengo bastantes cargos que no sé ni de dónde salen.» **[ANCL D25]**
- «No voy a estar copiando y pegando de una web a otra cada vez que escribo un email.» **[ANCL A21]**
- «Ni de broma voy a ponerme faltas de ortografía para parecer humano.» **[ANCL B21, E7]**
- «Si para que suene a mí lo tengo que escribir yo, entonces no me vendas nada.» **[ANCL E22, A31]**

**Transformación principal que buscan:** pasar de **«uso la IA a escondidas y con miedo, y luego la corrijo yo»** a **«uso la IA con tranquilidad, porque lo que escribe ya suena a mí»**. Desde el «cada texto es una batalla» hasta el «lo dejé configurado una vez y me olvidé».

---

### Criterios de selección final (Decision Criteria)

| # | Criterio | Cómo lo evalúa | Base |
|---|---|---|---|
| 1 | **Pago único / sin suscripción** | ¿Hay algo que se renueve? ¿Está claro el precio total? | D8, D14, D25 [ANCL] |
| 2 | **Funciona dentro de mi ChatGPT/Claude, sin otra herramienta** | ¿Tengo que abrir otra web? ¿Instalar algo? | A21 [ANCL] + diferencial |
| 3 | **Facilidad real para alguien no técnico** | ¿Hay capturas, un paso a paso, un vídeo? ¿Aparece alguna palabra técnica? | A35, A36 [ANCL] + HIP |
| 4 | **Demostración con textos como los míos** | ¿Hay un antes y después con un email o un mensaje normal, no con un ensayo? | HIP |
| 5 | **Que no destroce el sentido de lo que quiero decir** | ¿El resultado dice lo mismo que mi borrador? | D19, D33, D34 [ANCL] |
| 6 | **Que sea permanente** (no se degrade al cuarto mensaje) | ¿Se mantiene en conversaciones largas? ¿Qué pasa al abrir un chat nuevo? | A19 [ANCL] |
| 7 | **Garantía / reversibilidad** | ¿Me devuelven el dinero? ¿Puedo deshacer la configuración? | D10 [ANCL invertido] + HIP |

**Criterio eliminatorio:** **la suscripción o cualquier ambigüedad en el cobro.** «Si veo "al mes" en letra pequeña, cierro.» Lo apoyan D14 y D25, las dos voces BCT de la categoría. **Segundo eliminatorio: cualquier mención a código o instalación técnica** en las primeras líneas.

**Criterio diferenciador** (entre dos opciones similares): **la demostración con un texto como los suyos** y **la sensación de que quien lo vende escribe como una persona**. Entre dos guías parecidas, gana la que **ya suena humana en su propia página**. **[HIP]**

**Pruebas que busca para validar cada criterio:**
- Pago único → el precio visible, la palabra «único» y un botón sin letra pequeña.
- Dentro de mi IA → capturas de la pantalla de ChatGPT que él conoce.
- Facilidad → un vídeo de dos minutos en el que alguien lo hace en tiempo real.
- Demostración → el antes y después del mismo email.
- Permanencia → un ejemplo de una conversación larga o de un chat nuevo que mantiene la voz.
- Garantía → una política de devolución clara y en lenguaje humano.

**3 frases en primera persona que reflejan cómo razona en ese momento:**
1. «Si no me enseñan un email de verdad, de los que mando yo, antes y después, no me lo creo.» **[HIP con anclaje en la desconfianza del D-bloque]**
2. «Lo primero que miro es si se paga una vez o cada mes. Si es cada mes, fuera, no sigo leyendo.» **[ANCL D14, D25]**
3. «Que me lo enseñen en la pantalla de ChatGPT, la de siempre. Si sale una pantalla negra con letras, ya sé que no es para mí.» **[ANCL A36 + HIP de imagen]**

---

### Tipo de prueba por momento de decisión

**Prueba de entrada** (para que no le descarte en el acto):
- **Que el propio texto del anuncio o de la landing suene humano.** Es la prueba de entrada más potente y la más barata, y es exclusiva de este producto: **el copy es la demo**.
- Una **cara real** y un nombre (alguien que escribe, no una «plataforma»).
- **La palabra clave de exclusión de la competencia:** «no es otro humanizador».
- **Una idea que le haga pensar «ah, eso es verdad»**: por ejemplo, la paradoja de E12 («si le pides que no suene a IA, lo empeora»).
- Como el producto no tiene prueba social propia, en la entrada **no se puede fingir** con «miles de usuarios». La credibilidad de entrada debe ser **explicativa** (enseñar algo verdadero), no numérica.

**Prueba de cierre** (para comprometerse):
- **El antes y después** del mismo email: la versión por defecto de ChatGPT frente a la versión con la configuración, con las cuatro causas señaladas en el «antes».
- **Una demostración en vídeo de la configuración**, en tiempo real, sin cortes, en menos de 10 minutos, hecha en la pantalla normal de ChatGPT.
- **Garantía de devolución sin condiciones**, formulada como respuesta directa al agravio de la categoría: «si no te convence, te devuelvo el dinero. El dinero, no créditos».
- **Transparencia total de precio** (pago único, sin renovación).
- Cuando existan: **testimonios de personas no técnicas de 40-60 años** con su escenario concreto. **No antes de que existan.**

**Formato de prueba dominante para este mercado: la DEMOSTRACIÓN COMPARATIVA (antes/después del mismo texto), en formato texto y no solo en vídeo.**
**Justificación:** (1) el dolor dominante es personal, pero el **síntoma es visible y verificable**: el lector puede **ver** con sus propios ojos si un texto suena a IA, porque él mismo es juez (C23, E48); (2) la sofisticación del mercado es alta (nivel 3-4): ha oído todas las promesas y ya no se cree claims, solo **lo que ve**; (3) la categoría está contaminada por porcentajes de detectores, que el mercado ya sabe que no son fiables (B18, B20), así que una «puntuación de humanidad» no sirve como prueba, y sí sirve **el ojo del propio lector**; (4) el formato texto respeta que el producto es de escritura y que el lector quiere leer la diferencia, no que se la cuenten.

**Cruce con la etapa del journey:**
- **Passive Looking** (la mayoría del tráfico frío): prueba de entrada ligera, que consiste en **una sola frase o un par de líneas antes/después en el anuncio** («Esto es lo que te escribe ChatGPT. Esto es lo que te escribe cuando sabe cómo hablas»). Sin vídeos largos ni garantías todavía.
- **Active Looking / Deciding** (tráfico tras un incidente, o retargeting): la prueba de cierre completa (vídeo de la configuración, antes/después extenso, garantía, transparencia de precio).

---

### Especificidades del mercado

**¿De qué depende el éxito del mercado?** De que la IA del usuario deje de producir los cuatro patrones que el lector humano identifica como «máquina» (sintaxis predecible, hiperformalidad, vocabulario delator, cadencia uniforme) **y** de que empiece a producir rasgos de la persona concreta (sus expresiones, su registro, su forma de saludar y despedirse, su longitud natural de frase). Depende también de **la persistencia**: que eso se mantenga sin que el usuario tenga que repetirlo (A19). Y, de forma decisiva para este target, depende de que **el usuario sea capaz de hacer la configuración** sin abandonar a mitad.

**¿Qué debe «renunciar» el mercado para soltar su problema?**
- A la **ilusión de la solución mágica externa** (la web que «humaniza» con un clic).
- A la **excusa de que «la IA es así»**, que le exime de responsabilidad.
- A una parte de **la comodidad del statu quo**: invertir una tarde en configurarlo.
- A la idea de que **escribir «bien» es escribir «perfecto»**. Tiene que aceptar que el texto humano tiene asimetrías e imperfecciones (C4, A25).
- A **mantener la IA en secreto como si fuera una trampa**: el producto le pide reconocer que la usa, y usarla bien. **[HIP]**

**¿A quién culpa el mercado de su situación?**
- **A la IA** («ChatGPT escribe así», «Claude ha empeorado», A34).
- **A las empresas de IA** que no lo arreglan (A19: «I hope someone from OpenAI sees this post to fix…»).
- **A los humanizadores** que le estafaron (D-bloque).
- **A los jefes y empresas que empujan a usar IA para todo** (C14, C23, E15).
- **A los detectores y a quienes se los creen** (B-bloque, sobre todo el acusado).
- **A sí mismo**, en el recién llegado: «no soy técnico» (A36). Es la culpa más silenciosa y la más paralizante.

**Las 5 objeciones principales que tiene el mercado respecto a su problema:**
1. «No tiene solución: la IA siempre va a sonar a IA, por mucho que hagas.» **[ANCL A33, A29, A30]**
2. «Para lo que tardo en arreglarlo, lo escribo yo.» **[ANCL E22, A31]**
3. «Todo lo que se vende para esto es una estafa.» **[ANCL D1, D3, D6]**
4. «Yo no soy técnico, eso es para gente que sabe.» **[ANCL A35, A36]**
5. «Ya probé a darle instrucciones y no funcionó.» **[ANCL A19, A26, A27]**

---

### Sesgos cognitivos dominantes en este mercado

**1. Heurística de disponibilidad (con la estafa del humanizador como ejemplo disponible)**
- **Cómo se manifiesta aquí:** cuando piensa en «una herramienta para que mi texto no suene a IA», lo primero que le viene a la mente es la reseña de Trustpilot con el cargo de 200 $ (D8), el «$20 SCAM» (D1) o el texto convertido en *gibberish* (D22). Esos ejemplos vívidos y recientes dominan su juicio sobre **toda** la categoría.
- **A favor de la compra:** si el copy **nombra** esos casos («seguro que has visto las reseñas de esas webs que te cobran el año entero…»), el lector siente que el vendedor está **de su lado** y le coloca en la categoría opuesta.
- **En contra de la compra:** cualquier rasgo que le recuerde a un humanizador (una caja de texto, un porcentaje de «humano», una prueba gratuita que pide tarjeta, la palabra «humanizar») le activa el ejemplo disponible y lo descarta.
- **Instrucción concreta:** nombrar explícitamente la categoría de humanizadores **pronto** (en el primer tercio) como lo que **no** es el producto. No usar nunca el verbo «humanizar» para describir el producto. No mostrar porcentajes de detección. Explicar el precio con una sola cifra y la palabra «único».

**2. Sesgo de statu quo, reforzado por la «suficiencia» del sistema actual**
- **Cómo se manifiesta aquí:** reescribir a mano funciona (mal, pero funciona). Cada día que «no le pillan» confirma que puede seguir así (E33: «just have to remember to triple check»).
- **A favor de la compra:** si el copy cuantifica **lo que el statu quo ya le cuesta hoy** (media hora por email, F2; la vigilancia constante, F6), el statu quo deja de ser «gratis».
- **En contra de la compra:** si el copy exagera el riesgo («¡te van a despedir!»), el lector compara con su experiencia real («llevo un año así y no ha pasado nada») y desconfía.
- **Instrucción concreta:** atacar el statu quo por el **coste presente** (tiempo, vigilancia), no por un desastre futuro hipotético. Usar escenas cotidianas (el email de las once de la noche) y no catástrofes.

**3. Sesgo de autoeficacia baja / efecto «esto no es para mí»** (relacionado con la heurística de afecto ante lo técnico)
- **Cómo se manifiesta aquí:** el recién llegado infravalora su capacidad para configurar algo («yo no soy técnico», A36; «sigo confuso», A35). Cualquier señal de complejidad confirma esa creencia y le saca de la página.
- **A favor de la compra:** si el copy demuestra pronto que **el paso más difícil es copiar y pegar** dentro de la pantalla que ya usa, la autoeficacia sube y aparece el efecto IKEA (lo valorará más porque lo ha configurado él).
- **En contra de la compra:** las palabras «plugin», «skill», «instalar», «configurar» o «Proyectos», sin contexto, en el primer pantallazo. También los tutoriales con pantallas que no reconoce.
- **Instrucción concreta:** presentar la parte técnica **en el orden inverso** al habitual. Primero el resultado (el email), después lo que hay que hacer (en una frase: «le enseñas cómo hablas, una vez, dentro de tu ChatGPT») y solo al final el formato (PDF + guía/plugin), siempre con capturas. Llamarlo «guía paso a paso» antes que «plugin».

**(Sesgo adicional de soporte) Efecto de encuadre: «herramienta» frente a «configuración tuya»**
- La misma cosa (instrucciones permanentes dentro de ChatGPT) puede encuadrarse como «otro producto de IA» (pérdida) o como «enseñarle a tu IA cómo eres» (propiedad). El encuadre de **propiedad** («tu IA», «tu voz», «es tuyo») activa la aversión a la pérdida a favor: lo que es tuyo no se pierde ni se cancela.
- **Instrucción:** usar posesivos de segunda persona en todo el copy («tu ChatGPT», «tu forma de hablar») y evitar «nuestra herramienta» o «nuestro sistema».

---

### Balance de las 4 fuerzas del progreso

| Fuerza | Puntuación | Justificación |
|---|---|---|
| **F1 Push** | **7/10** | Dolor diario real (reescritura, vigilancia), con picos tras los incidentes. No llega a 9 porque el sistema actual «funciona» y la mayoría de los días no pasa nada visible. |
| **F2 Pull** | **5/10** | La idea de «configurarlo una vez» es atractiva, pero **el mercado no la tiene formulada como deseo** ([FUENTE ÚNICA] E53) y **tiene experiencias que la contradicen** (A19, A26, A27, A29). El Pull existe, pero es débil y escéptico. |
| **F3 Ansiedad** | **8/10** | Triple ansiedad: (a) «no voy a saber hacerlo» (A35, A36), (b) «será otra estafa o me cobrarán de más» (D-bloque), (c) «ya lo probé y no funcionó» (A26, A27). Está muy documentada para (b) y (c), y es residual pero central para (a). |
| **F4 Hábito / Inercia** | **6/10** | Reescribir a mano es un hábito asentado y «suficiente» (E33). Pero es un hábito **que no le gusta**, y esa insatisfacción reduce la inercia frente a hábitos cómodos. |

- **Fuerza dominante del lado positivo:** **F1 Push.**
- **Fuerza dominante del lado negativo:** **F3 Ansiedad.**
- **Ecuación actual:** (7 + 5) = 12 frente a (8 + 6) = 14 → **no hay compra**. Hay que mover al menos 3 puntos.
- **Palanca crítica del copy: REDUCIR LA ANSIEDAD.**

**Por qué la ansiedad es la prioridad sobre las otras tres:**
- **Frente a aumentar el Push:** el Push ya es alto y el mercado ya sabe que tiene el problema. Agitar más solo añade estrés a un lector que ya llega tenso (ver Mood Meter) y, con el sesgo de statu quo, la exageración se vuelve inverosímil.
- **Frente a aumentar el Pull:** el Pull choca con una ansiedad previa. Cuanto más bonito pinte el resultado («¡escribirá exactamente como tú!»), más activa el «ya, eso me dijeron los otros» (A30, D-bloque). El Pull solo crece **después** de bajar la ansiedad.
- **Frente a reducir la inercia:** la inercia es moderada, porque el prospecto no ama su sistema actual. Una vez que la ansiedad baja, la inercia cede casi sola.
- **Reducir la ansiedad son 3-4 puntos alcanzables:** pago único (-1), «dentro de tu ChatGPT, sin programar», con demostración visible (-1,5) y garantía de devolución real (-1) → la ansiedad baja a 4-5 y la ecuación se invierte.

**Consecuencia directa:** el copy **abre con seguridad y reducción de riesgo**, en este orden. (1) Un reconocimiento (*looping*) breve del problema que ya conoce, sin agitarlo de más. (2) Un **giro de seguridad** inmediato: «no es otro humanizador, no es una suscripción, no hay que programar». (3) La demostración. (4) La garantía, presentada pronto, no solo al final. Future Pacing: «el lunes, cuando abras ChatGPT para el primer email de la semana…».

---

### Por qué no compra nada (inacción real)

**Tipo dominante: INACCIÓN POR ANSIEDAD ANTE EL CAMBIO**, con un componente secundario de **resistencia al cambio** («tampoco es tan grave, lo retoco») en la parte del mercado que aún no ha tenido un incidente.
- **No es incapacidad de decidir.** No hay un abanico de opciones finalistas entre las que dude. El mercado ha descartado de antemano casi todo lo que existe (humanizadores, trucos). Su parálisis no viene de **qué elegir**, sino de **qué pasará si lo intenta**: que no sepa, que le cobren, que no funcione, otra vez.
- **Mezcla según el journey:** en *Passive Looking* domina la resistencia («ya lo arreglaré»); tras un incidente (*Active Looking*) domina la ansiedad («quiero arreglarlo, pero ¿y si…?»).

**¿Qué miedos específicos paralizan al indeciso?**
1. **Miedo a no ser capaz** de seguir los pasos y quedarse a medias, «con ChatGPT roto». **[HIP con anclaje A35, A36]**
2. **Miedo a que le cobren** algo más o algo recurrente. **[ANCL D8, D14, D25]**
3. **Miedo a que sea otra decepción** («ya lo probé con instrucciones»). **[ANCL A26, A27]**
4. **Miedo a que se note igual** después de pagar, y a quedar en evidencia ante sí mismo. **[HIP]**
5. **Miedo a que la empresa o el cliente se enteren** de que usa la IA (C21: revisión de seguridad; E19: descuento). **[ANCL, minoritario]**

**¿Qué le daría el «permiso» para moverse sin sentir que se arriesga?**
- **Ver a alguien como él hacerlo** (vídeo en tiempo real, en la pantalla normal).
- **Saber que es reversible** («si no te gusta, borras dos párrafos de los ajustes y ChatGPT vuelve a ser el de antes»). **[HIP, pero técnicamente cierto para las Instrucciones personalizadas]**
- **Garantía de devolución en dinero**, no en créditos.
- **Pago único**, sin renovación.
- **Una primera victoria rápida**: un paso que en 5 minutos ya cambia algo visible. **[HIP]**

**¿Qué tipo de copy le repele en este estado?**
- Urgencia artificial, cuentas atrás, «solo hoy».
- «Última oportunidad» o «el precio sube mañana».
- Comparaciones que le hacen sentir tonto («¿todavía no sabes usar las Instrucciones personalizadas?»).
- Euforia tecnológica, jerga, mayúsculas, emojis.
- Promesas absolutas («nunca más sonará a IA», «100 % indetectable»).

**3 frases en primera persona que revelan su estado de parálisis:**
1. «Me gustaría arreglarlo, de verdad, pero me da miedo ponerme a tocar los ajustes un martes por la noche y que mañana no me funcione el ChatGPT para el trabajo.» **[HIP con anclaje A36 · temporal HIP]**
2. «¿Y si pago y luego sigue sonando igual? Ya me pasó con la web esa: 60 dólares y el texto peor que antes.» **[ANCL D9, D11]**
3. «Llevo semanas con la pestaña abierta de un vídeo que explica cómo configurarlo. No lo he visto. Me da pereza y me da miedo, las dos cosas.» **[HIP con anclaje E53 · temporal HIP]**

---

### Capacidad real del prospecto

**Presupuesto percibido** **[DATO INSUFICIENTE para el target hispanohablante; anclas del corpus]**:
- **Anclas de la categoría en el corpus:** 20 $ (D1), 60 $ (D9), unos 180 $/año (D36) y más de 200 $/año (D8). El prospecto que ya probó humanizadores tiene esas cifras grabadas como **dinero tirado**.
- **Ancla de la herramienta base:** quien paga ChatGPT Plus o Claude Pro (unos 20-23 €/mes, **[HIP]**) compara cualquier producto con «otro mes de la suscripción». A28 sugiere un usuario que paga («defeats the purpose» porque gasta su límite de uso).
- **Disposición estimada:** 29 € como **pago único** está por debajo del umbral de «compra que hay que pensarse» para un profesional en activo. **[HIP basada en mercados similares de infoproductos para no técnicos]** Lo justificaría como «menos que un mes de la herramienta que no funcionaba» o «lo que me cuesta una comida».
- **Lo que de verdad pesa no es la cifra, sino la forma de pago:** una sola vez y sin sorpresas.

**Tiempo real:**
- Para **decidir**: poco y fragmentado (entre tareas, por la noche). No va a leer una carta de 8.000 palabras de corrido. **[HIP]**
- Para **implementar**: está dispuesto a invertir **una sesión** (30-90 minutos) si sabe de antemano que es una sola vez. No está dispuesto a «ir aprendiendo». **[HIP con anclaje en el rechazo a la repetición, A21]**
- Prisa: **moderada**, salvo tras un incidente (entonces la prisa es alta, durante unos días).

**Energía mental disponible:**
- Decide **desde el cansancio**, no desde la calma: al final del día, tras la tercera reescritura o tras el comentario del jefe. **Es una compra de alivio**, no de inversión deliberada. **[ANCL A1, F2, A27 + HIP]**
- Consecuencia: frases cortas, una sola idea por bloque y una ruta de compra sin bifurcaciones.

**Habilidades y conocimiento previo:**
- Sabe usar el chat: escribir, pegar, copiar, pedir.
- **No sabe** (o no lo ha usado nunca) que existen las Instrucciones personalizadas, los Proyectos o la memoria. **[HIP, con anclaje indirecto en A26, que sí las probó, frente a A36, que no sabe ni por dónde empezar]**
- No sabe **nombrar** lo que suena a IA (C23). Lo percibe, pero no lo puede explicar.
- Se siente perdido en la categoría: no distingue un humanizador de un detector, ni un prompt de una configuración. **[HIP]**

**Apoyo del entorno:**
- Decide **solo**, y probablemente **en silencio**. No va a decir en la oficina «me he comprado un curso para que no se note que uso ChatGPT». **[HIP con anclaje en la brecha voz pública/voz online]**
- **Quien facilita:** el compañero técnico o el hijo que le ayuda a configurarlo. **[HIP]**
- **Quien bloquea:** nadie de forma explícita. El freno es interno (ansiedad, vergüenza).
- **Facilitador estructural:** la empresa que le empuja a usar IA (C14, C23, E15). Paradójicamente, eso le **legitima** el gasto: «es para el trabajo». **[ANCL + HIP]**

**Restricciones físicas o logísticas:**
- **Plan de ChatGPT/Claude:** algunas funciones (Proyectos, memoria) varían según el plan gratuito o de pago y cambian con el tiempo. **[HIP técnico, a verificar al construir el producto]** Si la guía solo funciona en el plan de pago, es una restricción que hay que **declarar desde el principio**.
- **Cuenta de empresa con restricciones:** en entornos corporativos, la IA puede estar gestionada por IT y no permitir cambiar los ajustes (C21 apunta a controles de seguridad). **[HIP]**
- **Dispositivo:** muchos del target usan ChatGPT en el **móvil**. La guía debe funcionar también allí o aclarar que la configuración se hace una vez en el ordenador y luego sirve en el móvil. **[HIP]**
- **Idioma de la interfaz:** la interfaz de ChatGPT en español cambia los nombres de los menús («Personalizar ChatGPT», «Instrucciones personalizadas»). Las capturas deben ser **de la interfaz en español**. **[HIP]**

**Consecuencia directa para el copy:** facilitarle **una sola sesión de configuración, guiada, en su idioma, en su pantalla, con resultado visible en 5 minutos y reversible**. Reducir la fricción de la decisión (un precio, un botón, una garantía) y la de la implementación (capturas, vídeo, nada técnico). Declarar con honestidad los requisitos (plan, dispositivo).

---

## CONTEXTO DETALLADO

> Este bloque desarrolla en profundidad, en lenguaje narrativo y desde la perspectiva del prospecto, lo que la lista detallada resume. Mantengo las etiquetas de procedencia. Donde un punto ya está resuelto arriba, aquí solo añado capas nuevas en lugar de repetir.

### Demografía

- **Edad:** núcleo de 38 a 55 años, con extensión a 35-60. Hay un subgrupo más joven (28-37) que interesa como secundario. **[HIP con anclaje parcial; el corpus no declara edades]**
- **Situación sentimental:** **[DATO INSUFICIENTE]**. No hay ninguna señal en el corpus. Hipótesis: es irrelevante para la motivación de compra. El problema es laboral e identitario, no de pareja.
- **Nivel de ingresos:** **[DATO INSUFICIENTE]**. Hipótesis: ingresos medios o medio-altos (empleados de oficina, mandos intermedios, autónomos, profesionales liberales). Tienen capacidad de pago para 29 € sin fricción, pero mucha sensibilidad al **pago recurrente**.
- **Inclinaciones políticas o religiosas:** **[DATO INSUFICIENTE]**. No hay señales. Hipótesis: el mercado es **heterogéneo** en ambas dimensiones y no hay que segmentar por ellas. Una nota cultural sí relevante: en el corpus aparece cierta **ética del trabajo propio** («tiene que ser TU trabajo», C27; «stfu and pretend that your job is too complicated for AI», E19). El comprador valora el esfuerzo personal y siente que usar IA «a lo bruto» es hacer trampa.
- **Homogeneidad:** sí lo es en el **uso** (chat, sin código), en el **tipo de texto** (emails, mensajes profesionales, posts) y en la **relación ambivalente con la IA** (la usa, pero se avergüenza de que se note).

### Problema central

Es martes y son casi las once de la noche. Mañana a primera hora tiene que salir el email con la propuesta para el cliente. Lo ha empezado tres veces. La primera vez lo escribió él, pero le pareció torpe y se lo pegó a ChatGPT con un «mejóralo, que suene profesional». Lo que volvió era impecable, y por eso mismo no servía: «Estimado Sr. García: Espero que este mensaje le encuentre bien. Me complace presentarle…». Él no ha escrito «me complace» en su vida. El cliente lo conoce desde hace años y sabría al instante que eso no es suyo.

Así que lo pide otra vez: «más natural». Ahora sale algo más corto, pero con la misma música. Tres frases que empiezan igual. Un «no dudes en contactarme si tienes cualquier pregunta». Una lista de tres ventajas con el mismo número de palabras cada una. Lo lee y siente esa mezcla de **reconocimiento y vergüenza** de cuando ve un email de IA de otra persona, pero esta vez lleva su firma.

Termina reescribiendo la mitad a mano (A4). Un email que debería haberle llevado cinco minutos le ha llevado media hora (F2). Y al darle a enviar sigue sin estar seguro de si «se nota».

**Ese es el problema central: la IA, que debía ahorrarle trabajo y miedo a la página en blanco, le ha creado un trabajo nuevo (vigilar y desmontar el tono de máquina) y un miedo nuevo (que le pillen).** No sabe por qué pasa, y lo que ha probado para arreglarlo no ha servido. **[Escena: HIP construida sobre ANCL A4, A20, F2, E13; los textos en español son HIP]**

### Síntomas del problema

| Problema | → Síntoma concreto en su día a día | Base |
|---|---|---|
| La IA escribe con una voz que no es la suya | → Borra palabras «que jamás usaría» de cada borrador | A4 [PAR] |
| Teme que se note | → Relee cada email importante 3-5 veces antes de enviarlo | F2, F3, F6 |
| Teme que se note | → Le da un vuelco el estómago cuando un cliente responde «¿lo has escrito tú?» | F1 [ANCL · sensorial HIP] |
| Los trucos no funcionan | → Tiene una nota en el móvil con frases tipo «no uses palabras formales» que va pegando al final de cada petición | E24 [ANCL · escena HIP] |
| Los trucos se degradan | → En conversaciones largas, al tercer mensaje vuelve a ver el «En resumen,» o el «¡Claro!» | A19 [ANCL · HIP del tic en español] |
| Ha perdido la confianza en su propio criterio | → Empieza a quitar los guiones o los punto y coma de sus textos aunque los escriba él | A6, B5 |
| Ha perdido la confianza en su propio criterio | → Se pregunta si sus propios emails, escritos sin IA, «suenan a ChatGPT» | A13, A15, F6 |
| Vergüenza por lo visible | → Ha mandado alguna vez el texto con la frase del asistente pegada y desde entonces revisa tres veces | E33, B22 |
| Consumo de recursos | → Llega a mediodía sin mensajes disponibles en su plan porque los gastó corrigiendo el tono | A28 |
| Evitación | → Para lo más importante (la propuesta, la reclamación, la carta delicada) ya no usa la IA «por si acaso» | E22 [ANCL] + **[HIP]** |

### Impacto emocional

**En la autoestima:** cada vez que manda algo que no suena a él, se siente un poco **impostor**. Cuando se lo dicen, la sensación es de **ser descubierto en una pequeña trampa**, aunque no lo sea. Usar una herramienta para escribir no es trampa, pero así lo vive cuando se nota. A9 lo describe como «so insulting»: su criterio sustituido por una voz impersonal. **[ANCL]**

**En la percepción de sí mismo:** dos grietas.
1. **«Ya no sé escribir como yo.»** De tanto convivir con la voz de la IA, duda de la suya (A13: «deeply offended», con miedo a que su propia escritura natural ya parezca de un LLM).
2. **«Me he quedado atrás.»** El subgrupo veterano siente que los demás dominan la herramienta y él no (A36). **[residual + HIP]**

**En sus emociones cotidianas:**
- **Tensión de vigilancia**: una alerta de baja intensidad que se activa cada vez que va a enviar algo (F6: «Does that sound like AI?», casi a diario).
- **Fastidio**: la sensación de trabajar dos veces (A31, E22).
- **Picos de vergüenza** tras los incidentes (E33, B22, F1).
- **Rabia contenida** hacia la herramienta y hacia quienes le prometieron arreglarlo (D1: las mayúsculas y los signos de exclamación de la reseña lo dicen todo).

### Impacto social

**Trabajo — el jefe:** la relación pasa de la confianza a la **supervisión**. El jefe le dice que sus textos «suenan a ChatGPT» (A5), le cita por una diapositiva genérica (C27) o empieza a «darse cuenta» (A7). En el peor de los casos, la situación escala a una revisión formal (C21). Lo que se tensa es **la credibilidad profesional**: «si esto lo escribe la máquina, ¿qué aportas tú?». **[ANCL]**

**Trabajo — los clientes:** la relación pasa de lo personal a lo transaccional. El cliente que sospecha de la IA puede pedir descuento (E19), despachar el trabajo (F7) o perder la confianza tras una cadena de respuestas automáticas (C11, desde el lado del juez). Lo que se tensa es **el valor percibido** de su trabajo. **[ANCL]**

**Trabajo — compañeros:** pertenece, o teme pertenecer, al grupo que «pega cosas de ChatGPT en los correos». Los compañeros se quejan entre ellos (C4, C10, C15). **[ANCL indirecto]**

**Familia y amigos** **[ANCL indirecto + HIP]:** en el corpus, el lado personal aparece **como juez**. La amiga que «feels like talking to a robot» (C18), el amigo con frases que no eran suyas (C19), el hermano que acusa en medio de una discusión (B3), el match de una app de citas que deja ver la frase meta (C20). El comprador, si usa la IA para mensajes personales (felicitar, dar el pésame, mediar en el grupo de padres), corre el riesgo de **parecer frío o falso con la gente que quiere**. **[DATO INSUFICIENTE]** sobre cuántos del target usan la IA para eso.

### Frases sociales

**De aliados bienintencionados (pero dolorosos):**
1. «Oye, ¿por qué no lo escribes tú directamente? Tú escribes bien.» **[HIP con anclaje E36, «rewrite it in your own words»]**
2. «Pues pásalo por una de esas webs que lo humanizan, que dicen que funcionan.» **[HIP con anclaje D-bloque]**
3. «Yo le digo que finja que el español es su segunda lengua y así suena más normal.» **[ANCL E25, adaptado]**
4. «Bah, nadie se da cuenta, no te ralles.» **[HIP]**
5. «Tienes que aprender a hacer buenos prompts, es lo que se lleva ahora.» **[HIP]**

**De antagonistas o jueces (crueles o fríos):**
6. «¿Esto lo ha escrito ChatGPT?» **[ANCL F1]**
7. «Suena a ChatGPT.» **[ANCL F7, A5]**
8. «Está bien usar la IA para revisar, pero tiene que ser TU trabajo.» **[ANCL C27]**
9. «Me alegra ver que a ChatGPT le importo.» **[ANCL C19]**
10. «Parece que hablo con un robot.» **[ANCL C18]**
11. «Si el cliente se entera de que esto lo hace la IA, nos pide descuento.» **[ANCL E19]**
12. «Decirte que escribes como una IA no es ningún cumplido, que lo sepas.» **[ANCL E21]**
13. «Cuando digo que algo suena a IA no te estoy diciendo que esté bien escrito. Te estoy diciendo que no tiene alma.» **[ANCL E42, casi literal]**
14. «Lo he borrado en dos segundos, se veía de lejos que era de IA.» **[ANCL C17]**

### Disparadores de motivación (urgencia ahora)

El «ahora» lo provoca uno de estos eventos (desarrollados en «Disparador situacional» y en «Eventos disparadores»):
1. **El comentario de una persona con poder** (jefe, cliente). Es el más potente.
2. **El error visible** (frase meta pegada).
3. **El texto de alto riesgo inminente** (propuesta, candidatura, presentación ante dirección). **[HIP]**
4. **La enésima reescritura**: el día en que el hartazgo supera la pereza (F3).
5. **La presión corporativa** para usar IA en todo (C14, C23, E15).
6. **Verse reflejado en el email de IA de otro.** **[HIP del giro introspectivo]**

### Costes futuros (lo que le quita el sueño a las 3 a. m.)

- **«¿Y si ya lo saben todos y nadie me lo dice?»** Es el miedo a la reputación invisible: los jueces del corpus comentan entre ellos y borran sin contestar (C12, C15, C17, E30). Es un miedo especialmente nocturno, porque no tiene confirmación ni desmentido. **[ANCL + HIP de escena nocturna]**
- **«¿Y si el día que me juego algo grande se nota?»**: la propuesta que no se firma, el cliente que se va. **[ANCL F7, E19]**
- **«¿Y si me estoy quedando atrás?»** Los otros saben usar esto bien y él va a ser el de los emails de robot, o directamente el que no sabe. **[HIP con anclaje A36]**
- **«¿Y si llega un momento en que ya no sé escribir sin la máquina?»** **[ANCL A13]**
- B4 aporta la única mención literal de **insomnio** del corpus: los errores gramaticales y las decisiones de estilo le mantienen despierto porque teme que una escritura demasiado limpia parezca artificial. Es una voz de estudiante, **[PAR]**, pero el mecanismo (la rumiación nocturna sobre el estilo) es transferible. **[ANCL con cautela]**

### Efectos en las relaciones

- **El jefe**: «Desde lo de la presentación, Marta, mi jefa, me pide que le pase los emails importantes antes de enviarlos. No me lo ha dicho así, pero sé que es por eso.» **[HIP, construida sobre C27 y A5]**
- **El cliente de toda la vida**: «Don Ernesto, que lleva quince años conmigo, me llamó por teléfono en vez de contestarme el correo. "Prefiero hablarlo, que por escrito te noto raro." Colgué y me fui directo a releer lo que le había mandado.» **[HIP, construida sobre C11 (que llama directamente al propietario) y C12]**
- **El equipo**: «En el canal del equipo alguien puso un emoji de robot debajo de mi mensaje. Era una broma. Me lo tomé fatal.» **[HIP, construida sobre C15 y E30]**
- **La pareja o la familia**: «Le felicité el cumpleaños a mi hermana con un mensaje que me ayudó a escribir ChatGPT y me contestó "qué formal". Formal. A mi hermana.» **[HIP, construida sobre C18, C19 y B3; DATO INSUFICIENTE sobre la frecuencia de este uso]**

### Transformación mágica

Si un genio lo solucionara: **abre ChatGPT el lunes a las nueve, escribe «contéstale a Pedro que el jueves no puedo, que lo movemos al viernes, y que me mande el contrato» y lo que sale suena exactamente a un email suyo**: su saludo de siempre, sus frases cortas y alguna larga, la palabra que él usa y no la del diccionario, sin fórmulas, sin listas innecesarias. Lo lee una vez y lo envía. A media mañana ha despachado diez correos sin releer ninguno tres veces. Por la tarde se atreve a pedirle la propuesta importante, la que antes escribía él solo por miedo. La propuesta sale con su voz y con datos ordenados. El cliente contesta: «Perfecto, adelante». **Nadie dice nada de cómo está escrito. Eso es el éxito.**

**Qué proyectaría:** control tranquilo, la imagen de alguien que **usa la IA como un profesional y no como un atajo**. Los demás le verían más resolutivo y más rápido, **sin notar la herramienta**. **[HIP construida sobre la inversión de los síntomas]**

### Impacto de la transformación

- **Confianza:** deja de dudar antes de enviar. **[ANCL F6, invertido]**
- **Reputación:** recupera, o protege, la imagen de «el que escribe bien» o «la que se explica claro». **[HIP]**
- **Estilo:** su forma de escribir vuelve a ser reconocible; incluso se refuerza, porque la configuración le obliga a describirla. **[HIP, efecto IKEA y autoconocimiento]**
- **Relaciones:** los clientes y el jefe vuelven a responder al contenido.
- **El momento de sentirse «superior»** (el prompt lo pide): ver el email de IA de un compañero lleno de «Espero que este mensaje te encuentre bien» y pensar, con una sonrisa por dentro, **«eso me pasaba a mí»**. Es la superioridad del que ha salido del grupo de los que «se les nota». También: ser **a quien le preguntan** «¿cómo haces para que no se note?». **[HIP con anclaje E29, E35]**

### Identidad y significado de la compra

**¿Qué quiere demostrarse a sí mismo con esta compra?**
- Que **todavía puede con la tecnología**, que no le ha superado del todo. **[HIP con anclaje A36]**
- Que **usa la IA con criterio**, no a lo bruto. **[ANCL E34, E35]**
- Que **lo que firma sigue siendo suyo**. **[ANCL F3, A9]**

**¿Qué quiere que los demás piensen o sientan cuando vean esta decisión?**
Idealmente, **nada**: que no lo vean. El éxito es invisible. Si alguien lo supiera, querría que pensara: «qué listo, lo ha configurado bien». **[HIP]**

**¿Hay un «nuevo yo» implícito?**
Sí: **«alguien que tiene la IA domada»**. No un experto en IA, sino una persona que tiene su herramienta ajustada a su medida, como quien tiene el coche con el asiento y los espejos a su gusto. **[HIP de metáfora, ver Momento Aha]**

**¿Cierra o abre algún capítulo?**
- **Cierra:** el capítulo de «uso la IA a escondidas y con miedo» y el de «he tirado dinero en webs que no funcionaban».
- **Abre:** el de usar la IA para cosas importantes, no solo para borradores. **[HIP]**

**3 frases en primera persona:**
1. «Por fin soy de los que usan ChatGPT y no se les nota. Y no he tenido que aprender a programar ni nada de eso.» **[ANCL E35 + HIP]**
2. «Esto demuestra que yo también puedo con estas cosas, aunque tenga cincuenta y dos años y mi hijo se ría de cómo uso el móvil.» **[HIP: anclaje de edad construido, sin base directa en el corpus]**
3. «Ya no tengo excusa para no usar la IA en las propuestas grandes. Antes me escudaba en que "se notaba".» **[HIP con anclaje E22]**

**Gusto por la popularidad:** **Intermedio / validado**, con inclinación hacia el **buscador de consenso** en lo relativo al **riesgo** (quiere ver que otros como él lo han hecho) y hacia el **anti-mainstream** en lo relativo al **resultado** (no quiere sonar como todo el mundo, porque ese es el problema: la IA hace que todos suenen igual, C7: «tan intercambiables que ya no distingue a una persona de otra»).
**Implicación para la prueba social:** cuando exista, nada de «10.000 usuarios»; más bien «personas como tú (administrativas, comerciales, autónomos que no son técnicos) ya lo han configurado». Mientras no exista, la «prueba social» disponible es **la del problema** («le pasa a todo el mundo: mira lo que dicen los jefes y los clientes»), no la de la solución. Paradoja que hay que explotar: el producto vende **sonar distinto de la masa** a quien quiere **la seguridad de la masa**.

**Código de tribu:**

*5-8 palabras o expresiones que usa este mercado entre sí:*
1. «Suena a ChatGPT» / «se nota que es de ChatGPT». **[ANCL D1]**
2. «Slop» o «AI slop», y en español [HIP] «paja de IA», «relleno de IA», «texto de plantilla». **[ANCL C5, C9, C16, C22]**
3. «Tiene pinta de IA» / «huele a IA» (*AI stink*, E23).
4. «Copiar y pegar» como acusación («se ha limitado a copiar y pegar»). **[ANCL E27]**
5. «Sin alma» (*soulless*, A14, E42).
6. «Robótico». **[ANCL A17, E13]**
7. **[HIP en español]** «Muy de ChatGPT», «ChatGPTero», «eso es muy de IA», «se le ve el plumero».
8. **[Insider, NO usar con el recién llegado]**: *delve*, *tapestry*, *em dash*, *tells*, *prompt engineering*, *Pangram*.

*2-3 cosas que este mercado ridiculiza u odia:*
1. **La frase meta pegada** («Claro, aquí tienes una versión más profesional:»), que ridiculizan como «la versión 2026 del "Enviado desde mi iPhone"» (E29).
2. **El «Espero que este mensaje te encuentre bien»** y la efusividad falsa (E13, C17). En español [HIP]: «Espero que estés teniendo una semana increíble», «¡Gran pregunta!».
3. **Los humanizadores** y quien se cree sus porcentajes (D-bloque).

*La norma no escrita del grupo:*
**«Usar la IA está bien; que se note, no.»** Está bien visto que se use como ayuda y se revise; delata que «no eres de los nuestros» mandar algo **sin leerlo**, con la marca de la máquina, o **fingir** que es tuyo algo que suena a folleto. Lo dicen E35, E36, E34 y C27. **[ANCL, convergencia muy alta]**

### Frases post-transformación

**De apoyo:**
- «¿Has cambiado algo? Tus emails se leen mucho mejor últimamente.» **[HIP]**
- «Da gusto leerte, se nota que eres tú.» **[HIP, inversión de F1]**
- «¿Cómo lo haces para que la IA te escriba así? Pásamelo.» **[HIP]**

**De antiguos críticos:**
- «Perdona lo del otro día, pensaba que lo habías hecho con ChatGPT.» **[HIP, inversión de F1, C27]**
- (El jefe) «Este informe sí, este es tuyo. Así sí.» **[HIP, inversión de C27]**
- (El cliente) «Ahora sí te reconozco.» **[HIP]**

### Soluciones fallidas

Ver la tabla de «Otras soluciones». Matiz adicional para el contexto detallado: **el corpus contiene evidencia directa en contra del mecanismo del propio producto**, y hay que tratarla con honestidad:
- A26: «Después de probar **varias instrucciones de personalización**… sigue recibiendo textos que considera ridículos». **[PAR · BCT]**
- A19: «las instrucciones para evitar ciertos tics funcionan al principio, pero **se degradan** a medida que avanza la conversación». **[PAR]**
- A29: «Las listas de "patrones que evitar" quitan algunos tics, pero **no consiguen meter su propia personalidad**». **[PAR]**
- A33: patrones «casi imposibles de eliminar **solo con instrucciones**». **[PAR]**
- E9: «evitando activamente esas frases, puedes acabar pareciendo una IA a la que le han dicho que nunca use esos términos». **[LIT]**

**Lectura:** el mercado más experimentado **ya ha intentado** lo que este producto propone (instrucciones permanentes) y le ha fallado. El fallo tiene, según el propio corpus, **tres causas identificables**: (1) instrucciones **en negativo** (listas de «no hagas»), que según E9 y A29 no meten voz; (2) instrucciones **genéricas** («más casual», «más cínico», A26), no basadas en la voz real del usuario; (3) **degradación** en conversaciones largas (A19). **Consecuencia para el producto y el copy: el producto solo es creíble si explica por qué su configuración es distinta de «unas instrucciones personalizadas cualquiera»**. Tiene que basarse en la voz real del usuario y no en prohibiciones, atacar las cuatro causas y no solo el vocabulario, y dar pautas contra la degradación. Si el producto real no hace esto, la promesa fallará como falló a A26.

### Soluciones populares

Ver «Otras soluciones», punto 3. Objeciones del público a cada una, resumidas en su lenguaje:
- Humanizadores: «Estafa. Te lo deja peor y te cobra el año.» **[ANCL]**
- Listas de palabras: «Quitas cuatro palabras y sigue sonando igual.» **[ANCL A29]**
- Packs de prompts: «Tienes que pegarlo cada vez y a la tercera se le olvida.» **[ANCL A19, A21]**
- Plantillas de Instrucciones personalizadas: «Te ponen la de otro. No suena a ti, suena a la del youtuber.» **[HIP con anclaje A29]**
- Detectores: «Te dan lo que les da la gana: cero, cuarenta, cien.» **[ANCL B18]**

### Solución ideal

**Creíble pero casi demasiado buena:** una tarde, con una guía que le lleva de la mano en su propio ChatGPT, escribe (o dicta) cómo habla, pega unos cuantos textos suyos, sigue unos pasos y deja configurada su IA. **A partir de ahí, todo lo que le pide sale con su voz**: en el ordenador y en el móvil, hoy y dentro de tres meses, sin repetirle nada. Si un día quiere un tono más formal para un organismo oficial, se lo pide y lo hace **sin perder su forma de ser**. No paga nada más. No depende de ninguna web. Si algún día cambia de opinión, lo borra en un minuto. **Lo que permitiría hacer «sin esfuerzo»: escribir el email importante en cinco minutos y enviarlo sin releerlo tres veces.** **[HIP construida sobre los criterios]**

### El momento del «Aha» (fricciones de comprensión)

**Fricciones de comprensión:**
- **«¿Por qué suena a IA si yo le doy mis ideas?»** No entiende que el problema no está en el **contenido** sino en la **forma** (sintaxis, registro, cadencia). **[ANCL C23: «know when something feels off even if they can't put finger on exactly what it is»]**
- **«¿No es lo mismo que pedirle que suene natural?»** No distingue entre una petición puntual y una configuración permanente. **[ANCL A20, A26]**
- **«¿Dónde se pone eso?»** No sabe que ChatGPT tiene ajustes de personalización, o los ha visto y le parecen territorio técnico. **[HIP con anclaje A36]**
- **«¿Plugin? ¿Skill? ¿Eso se instala?»** El vocabulario del formato le resulta técnico. **[HIP]**
- **«Si ya lo probé y no funcionó…»** No entiende por qué esta vez sería distinto. **[ANCL A26]**

**El concepto que hace click:**
**«Tu IA no suena a IA porque sea mala escribiendo. Suena a IA porque no sabe cómo hablas tú, así que escribe como el "asistente educado por defecto" que alguien le dijo que fuera. No necesitas pedirle cada vez que suene natural. Necesitas decirle UNA VEZ quién eres.»**
Le acompaña la demostración de las **cuatro huellas** en un email cualquiera (frases que empiezan igual, «Espero que te encuentre bien», tres párrafos de la misma longitud, la lista de tres) señaladas con un subrayador. **El click llega cuando ve sus propias sospechas nombradas**: «¡eso es lo que yo notaba y no sabía decir!». **[HIP construida sobre C23, E38 y el mecanismo del producto]**
E38 («ChatGPT writes very formally and formulaically. It uses fancy words when a normal one would do, it often has perfect grammar and syntax, it doesn't vary sentence structure or length… just banal») es casi una definición literal de las cuatro causas del PDF. **El corpus valida que el mecanismo del PDF es el que la gente intuye.**

**Metáfora de resolución** **[HIP, a testear]**:
- **El asiento del coche:** «Es como cuando coges el coche de otra persona: todo funciona, pero el asiento, los espejos y la radio están a su medida. No hace falta cambiar de coche ni pedir que te lleven. Ajustas el asiento una vez y ya es tu coche.» Encaja con la tarea vital (control) y con la baja confianza técnica (todo el mundo ha ajustado un asiento).
- **El nuevo empleado:** «Contratas a un asistente brillante el lunes y no le dices nada de cómo trabajas. Escribirá como un manual. Si el primer día le explicas cómo hablas con tus clientes, el martes ya escribe como tú. Tu IA es ese asistente al que nadie le hizo la acogida.»
- **El acento:** «La IA tiene acento, como el que se nota a un extranjero que habla perfecto, demasiado perfecto. No hay que corregirle cada frase: hay que enseñarle a hablar como en tu pueblo.» (Más arriesgada culturalmente.)
- **Recomendada: la del nuevo empleado**, porque encaja con el contexto laboral del comprador principal y explica a la vez el problema (nadie le dijo cómo trabajas) y la solución (se lo dices una vez).

**La prueba que convence:** el **mismo email** escrito por ChatGPT por defecto y por ChatGPT configurado, uno junto al otro, con el lector como juez. Sin detectores ni porcentajes: **su propio ojo**.

**2 frases en primera persona:**
1. «Hasta que no vi los dos emails uno al lado del otro, con las frases marcadas en amarillo, no entendí qué era lo que me chirriaba. Era eso: todo medía lo mismo.» **[HIP con anclaje en E38 y A25]**
2. «Cuando me lo explicaron como "es un empleado nuevo al que nadie le ha dicho cómo hablas", dije: claro. Llevo un año pidiéndole cosas sin decirle quién soy.» **[HIP]**

### Lo que no quieren hacer

«No pienso aprender a programar.» «No pienso pagar otra suscripción.» «No voy a estar pasando cada email por tres webs.» «No voy a ponerme faltas a propósito para parecer humano.» «No voy a memorizarme una lista de palabras prohibidas.» «No voy a ver un curso de diez horas.» «No voy a darle mis documentos a una web que no sé de quién es.» **[Ver «Solución ideal» en la lista detallada para la base de cada una]**

### Creencias del mercado (condiciones que creen necesarias para el éxito)

- «Para que la IA escriba bien hay que saber hacer **prompts**.» **[HIP con anclaje E24, A35]**
- «Hay que **pagar una herramienta específica** para que no se note.» **[ANCL D-bloque]**
- «Hay que **revisarlo todo a mano** al final, sí o sí.» **[ANCL E36, A31]**
- «Hay que **quitar las palabras típicas** de la IA.» **[ANCL E-bloque]**
- «Hay que **ser escritor** para tener "una voz".» **[ANCL A22: aclara que no es copywriter, como disculpa]**
- «Hay que **meter imperfecciones**.» **[ANCL A24, B21]**
- «Hay que **pasar el detector**.» **[ANCL B-bloque; creencia del segmento estudiante que se filtra al adulto]**

### Lo que deben soltar

- **La excusa de «la IA es así»**, que le libera de la responsabilidad de lo que firma. **[HIP]**
- **La autocompasión del «yo no soy técnico»**, que le exime de intentarlo. **[HIP con anclaje A36]**
- **El ritual de la reescritura**, que, aunque le fastidie, le da una sensación de control y de «trabajo propio». **[HIP]** Hay algo de orgullo en «al final lo reescribo yo», y soltar ese ritual es soltar una pequeña prueba de que sigue haciendo su trabajo.
- **El secretismo**: si la IA escribe como él, ya no tiene excusa para ocultar que la usa, ni para usarla poco. **[HIP]**
- **La búsqueda de la herramienta mágica**, porque mientras busca la web perfecta no tiene que hacer el esfuerzo de configurar la suya. **[HIP]**

### A quién culpan

**Fuerzas externas:**
- **Las empresas de IA**, por la voz por defecto («I hope someone from OpenAI sees this post», A19; «Claude has become so bad at writing», A34).
- **Los humanizadores**, por estafadores (D-bloque).
- **Los jefes y empresas que imponen la IA para todo** (C14: «I feel like ChatGPT is my boss now»; C23; E15).
- **Los detectores** y quienes se los creen (B-bloque).
- **«Los demás»**, que han llenado el mundo de *slop* y han hecho que todo lo bien escrito parezca IA (C22: «making me crazy»; A1: «everything sounds like AI now»).
- **[HIP]** Los vendedores de cursos y prompts que prometen sin enseñar.

**Limitaciones autoimpuestas:**
- «No soy técnico.» (A36)
- «No soy escritor / copywriter.» (A22)
- «Ya soy mayor para esto.» (E46, **[residual]**)
- «No tengo tiempo para configurar nada.» **[HIP]**

---

## RESUMEN COMPLETO DEL BUYER PERSONA

> Retrato simbólico del comprador principal. No describe a una persona real: concentra los sentimientos compartidos que la mayoría del segmento reconocería como propios. Nombre ficticio para facilitar el trabajo de copy.

### «Carmen / Javier, el que firma con su nombre»

**Quién es.** Tiene entre 38 y 55 años. Trabaja delante de un ordenador: en una oficina, en una pequeña empresa propia, como autónomo o como mando intermedio. Escribe mucho, aunque nunca se ha considerado «alguien que escribe». Emails a clientes, respuestas a proveedores, mensajes al equipo, alguna propuesta, algún post en LinkedIn de vez en cuando. Hace uno o dos años empezó a usar ChatGPT (algunos, también Claude) para lo que más le costaba: arrancar, ordenar ideas, encontrar la palabra. Lo usa **como usa Google**: abre la página, escribe, copia el resultado. Nunca ha tocado los ajustes. La palabra «prompt» le suena a jerga, y «API», «Claude Code» o «agente» le suenan a otro planeta. Siente, sin decirlo en voz alta, que **la tecnología va más rápido de lo que él puede seguir**. **[Composición: definición del creador + ANCL del corpus; la edad y el contexto español son HIP]**

**Qué le pasa.** La IA le ha quitado el miedo a la página en blanco y le ha dado otro a cambio: **que se note**. Lo que le devuelve ChatGPT es correcto, ordenado e impecable, y precisamente por eso **no es él**. Lleva «Espero que este mensaje te encuentre bien», «no dudes en contactarme», tres párrafos de la misma longitud y frases que empiezan igual. Lo reconoce al instante, porque también él recibe emails así de otros y sabe lo que piensa cuando los lee: **«esto lo ha escrito una máquina; no se ha molestado ni en leerlo»**. Así que reescribe. Un email de cinco minutos se le va a media hora (F2). Borra las palabras que nunca usaría y rehace la mitad (A4). A veces se queda un cuarto de hora con una sola frase, se la pega a ChatGPT para que «suene natural»… y le sale peor (A20).

**Lo que más le duele.** No es el tiempo, aunque lo cuenta. Es **la posibilidad de que le pillen**. Ha oído, o ha vivido, la frase que más teme: **«¿Esto lo has escrito con ChatGPT?»** (F1). O la del jefe: «está bien que uses la IA, pero tiene que ser TU trabajo» (C27). O la del cliente que despacha semanas de trabajo con un «suena a ChatGPT» (F7). En su cabeza, que se note no significa «uso una herramienta moderna». Significa **«soy un vago, soy falso, ya no aporto»**. Y lo sabe porque es exactamente lo que **él** piensa de los demás cuando se les nota (E35, E36, C4, E48).

**Lo que ha probado.** Pedirle que suene natural (le metió más clichés, E12). Darle instrucciones y ejemplos (funcionó tres mensajes y luego volvió a lo de siempre, A19; tras ocho intentos seguía sonando «terribly AI», A27). Mirar, o probar, una de esas webs que «humanizan» el texto. Lo que encontró allí fue un texto con palabras raras y mayúsculas en medio de la frase (D23, D40), un porcentaje de «humano» que ningún otro detector confirmaba (D31) y un cargo en la tarjeta que no reconocía (D25), o el año entero cuando el anuncio decía «al mes» (D14). **De esa experiencia ha sacado una regla: «todo lo que se vende para esto es una estafa»** (D1, D6).

**Cómo está cuando le llega el mensaje.** Cansado. Escéptico. Llega al final del día, tras la tercera reescritura, o tras un comentario que le ha dejado tocado. No está ilusionado: está **harto y con miedo a equivocarse otra vez**. Su energía es baja y su valencia es negativa. Cualquier cosa que suene a gurú, a hype, a «IA» en mayúsculas o a «100 % indetectable» le hace cerrar la pestaña. Cualquier cosa que suene a código o a instalación le confirma que «esto no es para mí».

**Lo que de verdad quiere.** No quiere ser un experto en IA. Quiere **usar la IA sin que se note**: que lo que salga de su ChatGPT suene a él, a la primera, sin pelearse cada vez, sin otra pestaña, sin otra suscripción. Quiere darle a enviar **sin ese nudo** de «a ver si se nota». Quiere dejar de vigilar. Y, en el fondo, quiere demostrarse que **todavía puede con esto**: que la tecnología no le ha dejado atrás.

**Qué le frena.** El miedo. A no saber hacerlo («¿dónde se pone eso?»). A que sea otra estafa. A que le cobren de más. A que no funcione, como las instrucciones que ya probó. A estropear algo en la herramienta que usa para trabajar. **Su inacción no es pereza: es ansiedad ante el cambio.** Ya está convencido del problema. Lo que le falta es la seguridad de que intentarlo no le saldrá caro.

**Qué le movería.** Ver el **mismo email** escrito por su ChatGPT de siempre y por su ChatGPT configurado, uno junto al otro, con las «huellas» de la máquina señaladas. Entender en un párrafo **por qué** pasa (y que no es culpa suya). Comprobar que se hace **dentro de su propio ChatGPT, en la pantalla que ya conoce, sin programar, en una tarde**, y que **se paga una vez**. Una garantía de devolución en dinero, no en créditos. Y que la propia página que se lo vende **suene a persona**.

**Cómo habla de esto** **[ANCL, adaptado al español]**: «suena a ChatGPT», «se nota a la legua», «parece un folleto», «no es mi forma de hablar», «lo tengo que retocar todo», «para lo que tardo, lo escribo yo», «todo lo de esto es una estafa», «yo no soy técnico», «¿se notará?».

**Su norma de tribu:** **«Usar la IA está bien; que se note, no.»**

**Su Mass Desire:** **usar la IA sin que se note.**

**Su palanca de compra:** **reducir la ansiedad** (seguridad, demostración, reversibilidad, pago único), no agitar más el problema.

**Su frase interna más probable justo antes de leer el anuncio:** **«¿Por qué todo lo que me escribe ChatGPT suena a ChatGPT?»**

**Advertencia final del resumen:** este retrato está construido con voces **anglófonas**, mayoritariamente de foros con usuarios más técnicos que el target. El **qué** (el problema, las reacciones, el fracaso de las soluciones) está sólidamente documentado. El **quién** (edad, idioma, vocabulario nativo, canales en español, sensación de «la tecnología me ha superado») es hipótesis informada. Antes de escribir el titular definitivo hay que hacer al menos la investigación n.º 1 y la n.º 3 de la sección 0.9.

---

## Customer Job Statement (la frase de síntesis)

**Versión principal:**
> **«Cuando son las once de la noche, llevo media hora con el email al cliente que tiene que salir mañana a primera hora y ChatGPT me lo sigue devolviendo con ese "Espero que este mensaje te encuentre bien" que se huele a la legua, quiero que mi propia IA me escriba como hablo yo, sin pelearme con ella cada vez y sin que el cliente piense que le despacho con un robot, para darle a enviar a la primera, cerrar el portátil y no pasarme la mañana mirando si me contesta con un "¿esto lo has escrito con ChatGPT?".»**

**Comprobación de las reglas de construcción:**
- **Situación concreta:** día y hora (las once de la noche, víspera), lugar implícito (casa, portátil), tarea concreta (el email al cliente), sensación (media hora perdida y el «se huele»). ✔
- **Integra varias capas:** funcional («que mi IA me escriba como hablo yo, sin pelearme cada vez»), emocional («no pasarme la mañana mirando…», el alivio) y social («sin que el cliente piense que le despacho con un robot»). ✔ (las tres)
- **Resultado visualizable:** darle a enviar, cerrar el portátil, una mañana sin vigilar la bandeja. ✔
- **Lenguaje del prospecto:** «se huele a la legua», «le despacho con un robot», «darle a enviar». ✔ (registro **[HIP]** de español de España; los elementos son **[ANCL]**: F1, F2, A20, E13, A31)

**Versión corta (semilla directa de headline):**
> «Cuando ChatGPT me devuelve otra vez el email con pinta de robot, quiero que mi IA escriba como yo de una vez por todas, para darle a enviar sin pensar "¿se notará?".»

**Versión para el subgrupo con jefe (en lugar de cliente):**
> «Cuando mi jefe me vuelve a decir que el informe "suena a ChatGPT" y yo sé que me he pasado una hora retocándolo, quiero que la IA que uso cada día escriba con mi forma de explicar las cosas, sin tener que aprender nada técnico, para que la próxima vez lo que comente sea el contenido y no quién lo ha escrito.»

---

## Pilares de mensaje (Message Themes)

**Pilar 1 — «A nadie le molesta que uses IA»**
- **Tensión que resuelve:** siente que usar la IA es una pequeña trampa y vive su uso con culpa y secretismo.
- **Frase en voz del buyer:** «Yo no quiero dejar de usar ChatGPT. Lo que no quiero es que se me note cada vez que lo uso.» **[ANCL E35, E36]**
- **Implicación para copy:** abrir con la norma del grupo («usar la IA está bien; que se note, no») para **quitar la culpa** antes de vender. Citar el lado del juez («lo que la gente odia no es que uses IA, es que suene a robot») como validación externa. Es el pilar que rompe la predicción y establece complicidad. Va en el **titular o subtitular**.

**Pilar 2 — «No es culpa tuya: tiene cuatro huellas»**
- **Tensión que resuelve:** nota que «algo chirría», pero no sabe qué es. Lo atribuye a su torpeza o a la herramienta, y se siente impotente.
- **Frase en voz del buyer:** «Yo notaba que algo no cuadraba, pero no sabía decir el qué. Ahora lo veo en todas partes.» **[ANCL C23]**
- **Implicación para copy:** mecanismo único educativo. Explicar las cuatro causas (sintaxis predecible, hiperformalidad, vocabulario delator, cadencia uniforme) con un ejemplo subrayado. Es la **prueba de entrada** (enseñar algo verdadero) y el núcleo del lead tipo «Secreto». Es el pilar del PDF.

**Pilar 3 — «Una vez, y es tuyo»**
- **Tensión que resuelve:** está harto de pelearse cada vez (pedir «más natural» en cada mensaje, pegar trucos, pasar el texto por otra web) y de pagar cada mes.
- **Frase en voz del buyer:** «Quiero dejarlo configurado una tarde y olvidarme. No quiero repetirle lo mismo en cada email.» **[ANCL A21, A19, E53]**
- **Implicación para copy:** el diferencial central frente a humanizadores y prompts. Va en el **contraste central** y en la **oferta** (pago único, sin suscripción, sin dependencia externa). Prueba: la demostración de una conversación larga o de un chat nuevo que mantiene la voz.

**Pilar 4 — «Si sabes copiar y pegar, sabes hacer esto»**
- **Tensión que resuelve:** quiere arreglarlo, pero le aterra no ser capaz o romper algo («yo no soy técnico»).
- **Frase en voz del buyer:** «Si me dices que tengo que instalar algo o tocar código, me voy. Si es en mi ChatGPT, el de siempre, te escucho.» **[ANCL A36, A35 + HIP]**
- **Implicación para copy:** es **la palanca crítica (reducir la ansiedad)**. Capturas de la interfaz en español, vídeo en tiempo real, «primer cambio visible en 5 minutos», «reversible en un minuto». Evitar «plugin», «skill» o «configurar» sin explicación en el primer pantallazo. Va **inmediatamente después del hook**.

**Pilar 5 — «No es otro humanizador»**
- **Tensión que resuelve:** desconfía de todo lo que se vende en la categoría, por experiencia propia o ajena (cargos ocultos, texto destrozado, porcentajes que no cuadran).
- **Frase en voz del buyer:** «Otra web que me cobra el año entero y me deja el texto con palabras que no existen… no, gracias.» **[ANCL D14, D23, D25]**
- **Implicación para copy:** nombrar la categoría de los humanizadores **como lo que no somos**, con datos de sus reseñas (sin nombres de marca en el copy público). Garantía en **dinero, no en créditos** (respuesta directa a D10). Nunca usar «humanizar», «indetectable» ni «bypass».

**Pilar 6 — «Que suene a ti, no a perfecto»**
- **Tensión que resuelve:** cree que escribir bien es escribir «perfecto», y la IA es perfecta y suena falsa. Duda entre empobrecer el texto o mandarlo impecable y frío.
- **Frase en voz del buyer:** «Prefiero un email con una frase un poco torpe pero mía que uno perfecto que huela a máquina.» **[ANCL C4, A25, B21]**
- **Implicación para copy:** reencuadre de la calidad: lo humano es asimétrico y tiene personalidad. Mostrar en el antes y después que el «después» es **menos pulido y más eficaz**. Es el pilar de la promesa secundaria (la voz propia) y protege contra la objeción «quiero que suene profesional».

**Pilar 7 — «Recupera la media hora»**
- **Tensión que resuelve:** la IA debía ahorrarle tiempo y se lo está quitando.
- **Frase en voz del buyer:** «Un email de cinco minutos y me tiro media hora retocándolo. Para eso lo escribo yo.» **[ANCL F2, E22, A31]**
- **Implicación para copy:** **justificación lógica** (body copy y bloque de precio), no apertura. Cuantificar en tiempo («30 minutos × 4 emails al día»). Encaja con el formato numérico de coste de la inacción por unidad de tiempo.

**Regla de calidad aplicada:** he descartado un posible pilar «La IA te hace parecer mayor / anticuado» por falta de base (es residual) y porque podría ser un disparador de expulsión. También he descartado «Pasa los detectores», que es del anti-persona.

---

## Contraste central del copy

- **Estado A (sin solución):** **son las once de la noche y llevas media hora releyendo un email de cinco líneas porque ChatGPT te lo ha devuelto con «Espero que este mensaje te encuentre bien» y no sabes si el cliente notará que no es tuyo.**
- **Estado B (con solución):** **son las nueve y cinco de la mañana, le has pedido el email a tu ChatGPT, ha salido con tu forma de hablar, lo has leído una vez y ya está enviado.**
- **La yuxtaposición más poderosa: «a las once de la noche, reescribiendo» frente a «a las nueve y cinco, enviado».** Es un par **antes/después en el tiempo**, apoyado en un contraste secundario **«cada vez» frente a «una vez»** (pelearse con la IA en cada mensaje frente a configurarla una sola vez).

Versión alternativa del contraste, más visual y apta para un anuncio: **dos emails, uno al lado del otro**: el de ChatGPT por defecto, con las huellas subrayadas, y el de ChatGPT configurado. El cerebro construye el antes y después en menos de diez segundos **sin leer una sola línea de copy**.

**Los tres momentos de la carta donde reaparece el contraste:**
1. **Al inicio (titular / hook):** «Las once de la noche y el email sigue sonando a robot». Primera aparición del Estado A, o la imagen de los dos emails.
2. **A mitad (transición de la historia al producto):** tras explicar las cuatro huellas: «Hasta aquí, lo que hacías cada vez. Ahora, lo que haces una vez». Es el giro de «cada vez» a «una vez», donde se presenta la configuración.
3. **Al final (cierre antes del precio):** el Future Pacing del Estado B: «El lunes a las nueve abres ChatGPT para el primer email de la semana. Lo pides. Lo lees una vez. Lo envías. Y sigues con tu día». Inmediatamente después, el precio único.

---

## Diagnóstico de Schwartz

### 1. Nivel de consciencia predominante

**Consciente del Problema**, con una franja amplia de **Consciente de la Solución** (de las soluciones equivocadas).
**Por qué:** el corpus entero gira en torno a gente que **sabe** que su texto suena a IA (patrón D1, mayoritario) y que ha probado o ha visto soluciones (humanizadores, prompts, listas). Pero para el target real (35-60 años, recién llegado, hispanohablante), la consciencia de la solución se limita a **trucos genéricos** («que suene natural») y a **la existencia de humanizadores**. No conoce la solución de configuración permanente, o la conoce de oídas y no la ha probado. Desglose en «Niveles de consciencia».

### 2. Nivel de sofisticación

**Nivel 4** (mercado saturado de mecanismos) en el segmento angloparlante e insider. **Nivel 3**, con tendencia al 4, en el segmento hispanohablante de baja confianza técnica **[HIP: no hay datos de saturación en español]**.

**Justificación con ejemplos de lo que ya existe:**
- **Promesas de nivel 1-2 ya agotadas:** «Haz que tu texto de IA suene humano» y «más humano, más rápido» (todos los humanizadores).
- **Mecanismos de nivel 3 ya en el mercado:**
  - **Reescritura algorítmica** («cambiamos el ritmo, no solo las palabras», D2; «modelo actualizado para superar a Pangram», D18; «niveles de undetectability», D28).
  - **Listas de palabras prohibidas** (E1-E12: *delve*, *tapestry*, *journey*, etc.).
  - **Prompts de estilo** («use conversational tone, less corporate jargon», E24; «say English is your second language», E25).
  - **Clonadores de voz / alimentar con tus textos** (A30, E18).
  - **Instrucciones personalizadas / «rulebook once»** (E53, A26, A29). **Ojo: el mecanismo exacto de este producto ya circula gratis en vídeos cortos.**
- **Por eso el nivel 4:** «configurar tu IA para que suene humana» ya no es nuevo como mecanismo. **Hay que expandirlo**: explicar **por qué** las instrucciones habituales fallan (en negativo, genéricas, se degradan) y **qué hace distinta** esta configuración (basada en tu voz real, contra las cuatro causas, guiada para no técnicos y resistente a la degradación).
- **Señales de nivel 5** (escepticismo y muerte emocional) en una parte del mercado: «IT'S A $20 SCAM» (D1), «AI detectors don't work» (E9), «I hate the future» (C24), «Am I the only one sick and tired of how AI writes» (A33). Para esta franja, la entrada tiene que ser **identitaria** (la norma del grupo, «usar la IA con criterio»).

### 3. La «Promesa Agotada»

**«Haz que tu texto de IA suene 100 % humano / sea indetectable.»** Es la promesa que han repetido nueve marcas de humanizadores y que el mercado asocia con estafa, texto destrozado y cobros opacos. Con ella van las agotadas secundarias:
- «Con este prompt, ChatGPT escribirá como un humano.»
- «Ahorra horas con la IA.»
- «Clona tu voz.»
**Ninguna debe usarse como gancho principal.** La palabra «humano» puede aparecer en el body copy, pero no en el titular de forma aislada.

### 4. Recomendación de Lead

**Lead de Secreto con apertura de Problema reconocido (Problema-Secreto)**, apoyado en una **micro-historia**.
- **Apertura:** la frase interna del lector («¿Por qué todo lo que me escribe ChatGPT suena a ChatGPT?») o la escena del Estado A, en dos o tres líneas, sin agitar de más.
- **Ruptura de predicción:** la paradoja («si le pides que no suene a ChatGPT, suena más a ChatGPT», E12) o la verdad incómoda («a nadie le molesta que uses IA; le molesta que se note», E35).
- **Secreto / mecanismo:** las cuatro huellas, «tu IA no sabe cómo hablas tú».
- **Giro de seguridad:** «no es otro humanizador, no es una suscripción, no hay que programar».
- **Demostración y oferta.**
**Por qué no un lead de Proclamación** («¡Por fin, ChatGPT escribirá como tú!»): es una promesa agotada en un mercado de nivel 4 y dispara el filtro de estafa. **Por qué no un lead de Problema-Agitación puro:** el Push ya es alto y la palanca es la ansiedad, así que agitar añade tensión a un lector ya tenso.

---

## Etapa del tráfico frío en el journey de decisión

| Etapa | % estimado del tráfico frío | Evidencia |
|---|---|---|
| First Thought | 10 % | Usuarios que aún no han notado que su texto suena a IA (los «emisores inconscientes» que los jueces del bloque C describen: C3, C10, C15, C16, E30). Rara vez llegan por sí mismos. |
| **Passive Looking** | **55 %** | La mayoría del corpus describe una molestia **crónica** que se resuelve reescribiendo, sin búsqueda activa sostenida (A1, A4, F2, F6, E33). Están en modo radar: si ven algo, lo miran. |
| Active Looking | 30 % | Tras un incidente: hilos de «How do I make it…» (A26, A27), «How do you stop AI writing sounding like AI» (A11, A16), comparativas y reseñas de humanizadores (D-bloque). |
| Deciding | 5 % | Casi nadie está decidiendo entre finalistas, porque no hay finalistas creíbles para el adulto honrado (los humanizadores están descartados). |

**[HIP de porcentajes basada en la distribución del corpus; el corpus, por su naturaleza de foro, sobrerrepresenta el Active Looking]**

**Implicación para el ángulo de entrada:** el copy de tráfico frío debe estar diseñado para **Passive Looking**: hook de **reconocimiento** (la escena o la frase interna), prueba de entrada ligera (dos líneas antes/después), nada de comparativas detalladas ni garantías largas en el anuncio. Para el 30 % en Active Looking (búsquedas en Google tras un incidente), una landing con más profundidad: la explicación de las cuatro huellas, la comparación con humanizadores y el vídeo de configuración. **No mezclar:** un anuncio con «compara: pago único frente a suscripción de 180 $» fatiga al de Passive Looking; un anuncio de solo «¿te pasa esto?» se queda corto para el de Active Looking que viene de Google.

---

## Niveles de Consciencia (Schwartz)

### 1. Nivel predominante, con porcentajes aproximados

| Nivel | % | Descripción en este mercado |
|---|---|---|
| Inconsciente | 15 % | Usa ChatGPT para escribir y **no nota** que suena a IA. Los demás sí lo notan (bloque C: managers y compañeros que se quejan de que los otros lo pegan sin más). **[ANCL indirecto]** |
| **Consciente del Problema** | **45 %** | Sabe que «suena a ChatGPT», lo reescribe a mano y no sabe que exista una forma de arreglarlo de raíz. |
| Consciente de la Solución | 35 % | Conoce los humanizadores (y desconfía de ellos), los trucos de prompt y las listas de palabras. Quizá ha oído hablar de las «Instrucciones personalizadas». |
| Consciente del Producto | 5 % | Conoce al creador o ha visto contenido suyo. |
| Totalmente consciente | 0 % | Es un producto nuevo y sin clientes. |

**[HIP de porcentajes]**

### 2. Evidencias

- **Problema:** el patrón D1 («suena a IA») es el más frecuente del corpus (≈ 45 entradas). La gente nombra el problema con soltura.
- **Solución (equivocada):** 42 entradas sobre humanizadores. La categoría existe en la mente del mercado y está desacreditada. Unas 10 entradas sobre prompts e instrucciones que fallan.
- **Solución correcta poco conocida:** una sola mención directa a la «configuración una vez» (E53). Para el recién llegado, la consciencia de que se puede configurar ChatGPT de forma permanente es baja. **[HIP con anclaje A36]**
- **Inconsciente:** el bloque C muestra a muchos emisores que mandan IA sin editar (C3, C10, C16, E30), lo que indica una masa de usuarios que **no percibe** su propio problema.

### 3. Implicaciones para el copy

- **Nivel 2 (Problema, 45 %):** educar y agitar el problema **suavemente**. Reconocer, nombrar las cuatro huellas, explicar que tiene solución.
- **Nivel 3 (Solución, 35 %):** **diferenciar** de humanizadores y trucos: «por qué lo que has probado no funcionó» y «por qué esto es distinto».
- **Nivel 1 (Inconsciente, 15 %):** no es tráfico rentable para ads directos. Se alcanza con contenido («¿Tus emails suenan a ChatGPT? Haz esta prueba») o con la paradoja (lead magnet: el PDF de las cuatro huellas como regalo).

### 4. Ángulo de entrada recomendado

**Abrir hablando del PROBLEMA**, en forma de reconocimiento y no de agitación, y **pasar rápidamente a la explicación** (las cuatro huellas) antes de presentar la solución. **No abrir hablando del producto**, porque nadie lo conoce y el formato («PDF + plugin») activaría el filtro técnico. **Abrir con la solución** («configura tu ChatGPT») funcionaría solo con el 35 % consciente de la solución, y además choca con la sofisticación de nivel 4 («ya lo probé»).

---

## Matriz de los Problemas

| Dimensión | Puntuación (1-10) | Consecuencia específica |
|---|---|---|
| 1. Fuente (Psicológica → Fisiológica) | **2** | El problema se vive como **psicológico y social** (vergüenza, identidad, reputación), no físico. El copy debe trabajar barreras emocionales con historias empáticas y validación. La «prueba tangible» no es corporal, sino **visual** (el texto). |
| 2. Claridad causal (Baja → Alta) | **3** | El prospecto **no sabe por qué** suena a IA (C23: «can't put finger on exactly what it is»). Los insiders hablan de palabras sueltas, pero no hay consenso (E4: «usar una sola palabra como rúbrica es terrible»). → Ofrecer **una explicación simple y convincente**: las cuatro huellas. Es la gran oportunidad del PDF. |
| 3. Visibilidad (Baja → Alta) | **8** | El problema es **muy visible para los demás**: cualquiera que lea el texto puede notarlo (C17 lo nota en segundos; E48, en la primera línea). Pero el emisor no siempre lo ve en sí mismo. → Usar **antes/después** visual y resultados inmediatos («mira la diferencia en el mismo email»). |
| 4. Urgencia (Baja → Alta) | **6** | Crónica con picos. Media en el día a día, alta tras un incidente. → En tráfico frío, amplificar **el coste presente** (tiempo, vigilancia), no el futuro catastrófico. En retargeting tras el incidente, lenguaje más inmediato. |
| 5. Estigma social (Bajo → Alto) | **7** | Que se note tiene estigma: vago, falso, «no aporta», tramposo (C27, E19, E21, E16). Comprar ayuda para esto también tiene un estigma leve («confieso que lo hacía mal»). → **Tono confidencial y empático**, sin exponer. Compra discreta. Nada de «¡únete a la comunidad de 10.000!» en público. |
| 6. Medibilidad (Baja → Alta) | **4** | El progreso se puede «ver» en el texto, pero no se mide con fiabilidad: los detectores no sirven (B18, B20) y el estándar es subjetivo («suena a mí»). Lo medible es el **tiempo** (de 30 a 5 minutos). → Visualizar resultados con **ejemplos de texto e historias**. Usar el tiempo como única métrica concreta. Nunca porcentajes de detección. |
| 7. Frecuencia (Baja → Alta) | **9** | Cada día, varias veces al día: cada email, cada mensaje (A1, F6). → **Aliviar el dolor diario**: el copy habla del «cada vez» y de la solución «una vez». |
| 8. Locus de control (Interno → Externo) | **6** | Mixto. Culpa a la IA y a las empresas (externo) y a la vez se culpa a sí mismo por no ser técnico (interno). → Por la parte interna: **«no es culpa tuya»** (la IA está diseñada para sonar a asistente educado). Por la externa: **ofrecer una vía para recuperar el control** (tu configuración, tu IA). |
| 9. Intensidad emocional (Baja → Alta) | **6** | Moderada-alta en los picos (vergüenza, «freaking out», «my soul left my body») y moderada en la rutina (fastidio, vigilancia). → Empatía alta sin reabrir la herida (no recrear la humillación con detalle morboso). Las historias deben **reconocer**, no **revivir**. |
| 10. En primera persona (Otro → Yo) | **7** | Afecta sobre todo **al propio prospecto** (su reputación, su tiempo, su voz), aunque con una capa relacional (el cliente, el jefe). → Enfocar en el **beneficio personal** («tú, tu tiempo, tu voz») con un apoyo relacional («tu cliente vuelve a leerte a ti»). |

### Resumen final de la matriz

Según la lógica de la **Problem Matrix Prime**, este mercado combina un problema **altamente psicológico (2)**, de **claridad causal baja (3)**, **muy visible para los demás (8)**, **muy frecuente (9)** y con **estigma social apreciable (7)**. Esa combinación tiene una consecuencia nítida:

1. **Potenciar la explicación causal.** Cuando la claridad causal es baja, la Problem Matrix Prime indica que gana quien ofrece **la explicación simple y convincente**. Las cuatro huellas son el activo más valioso del producto para el copy. **El PDF no es un complemento: es la llave de la venta.**
2. **Potenciar la demostración visual.** Con visibilidad alta, el antes/después funciona. Como el problema es visible **para los demás**, la demostración tiene que ponerse en los ojos del lector como juez («¿cuál de los dos emails te creerías?»).
3. **Potenciar el alivio diario.** Con frecuencia 9, el copy debe hablar del **«cada vez»**: cada email, cada mensaje, cada vigilancia. El «una vez» del producto es la respuesta exacta.
4. **Evitar la exposición.** Con estigma 7, nada de tono burlón sobre «los que se les nota la IA» que el lector pueda sentir dirigido a él. Nada de prueba social pública que le obligue a reconocerse.
5. **Evitar métricas falsas.** Con medibilidad 4 y detectores desacreditados, cualquier porcentaje de «humanidad» destruye la credibilidad.
6. **Evitar la culpa.** Con locus mixto, el «no es culpa tuya» debe llegar pronto, antes de pedirle que haga algo.

**Motores emocionales profundos que la matriz confirma:** vergüenza anticipatoria, deseo de control, fatiga de vigilancia, miedo a la pérdida de reputación, deseo de seguir siendo «uno mismo» en lo que firma, y el temor silencioso a quedarse atrás.

---

## Un Día en la Vida (Cine-Verité)

> Escenas **[HIP narrativa]** construidas sobre síntomas **[ANCL]**. Cada escena indica su anclaje.

### 1. El Despertar y el Espejo

Las siete y diez. La alarma del móvil suena por segunda vez. Carmen abre los ojos con esa pesadez en la frente de haber dormido mal, y lo primero que hace, antes de levantarse y antes de mirarse al espejo, es **coger el móvil y abrir el correo**. Busca una sola cosa: si el cliente ha contestado al email de anoche, el que mandó a las once y veinte después de reescribirlo cuatro veces.

Ha contestado. Una línea: «Recibido, lo vemos el jueves.» Nada más. Carmen se queda mirando la pantalla con el pulgar suspendido. **«¿Solo eso? ¿Se habrá dado cuenta?»** Relee su propio email en la bandeja de enviados. «Espero que te encuentre bien»: no lo quitó. Lo quitó en la primera versión, ChatGPT lo volvió a meter en la segunda y ella no lo vio en la tercera. El estómago se le encoge un poco.

En el espejo del baño, mientras se lava la cara con agua fría, el juicio dura un microsegundo: **«Cincuenta y un años y no sé ni escribir un email sin una máquina. Y encima la máquina me deja en evidencia.»**
*[ANCL: F2 (relecturas), F1 (miedo a la pregunta del cliente), A19 (el tic vuelve), A36 (no técnico) · escena y anclajes sensoriales HIP]*

### 2. El Punto de Fricción Diurno

Las once y cuarto, en la oficina. Su responsable le pide «un resumen de la reunión de ayer para mandárselo a dirección, algo cortito». Carmen tiene las notas, pero le cuesta ordenarlas, así que abre ChatGPT, pega las notas y escribe: «hazme un resumen profesional».

Lo que sale tiene un título en negrita, cuatro apartados con sus viñetas, la palabra «sinergias», un «En resumen,» al final y una frase que empieza por «Es importante destacar que». **Ella no ha dicho «sinergias» en su vida.** Su responsable tampoco. Y su responsable ya le dijo hace dos semanas, medio en broma, que «últimamente escribes como un robot».

Abre otra pestaña con el documento en blanco. Copia. Pega. Borra «sinergias». Borra el «Es importante destacar que». Quita las negritas. Vuelve a ChatGPT: «más natural, menos formal». Copia. Pega. Ahora sale un «¡Claro!» al principio que tiene que borrar. Llevan veinticinco minutos para un resumen de diez líneas.

Cuando su compañero se asoma y le pregunta «¿te queda mucho?», ella dice: **«Nada, estoy repasando las cifras, que no me cuadraba una cosa.»** No hay cifras. Lo que está repasando es que no se note.
*[ANCL: A21 (ciclo de pestañas), A5 (el jefe que dice que suena a ChatGPT), E13 (fórmulas), F2 (tiempo multiplicado), A20 (petición «más natural») · tics en español HIP]*

### 3. Las Punzadas de Envidia

Las cuatro y media. Reunión por videollamada con un proveedor nuevo. Al final, el comercial del proveedor, un chico de unos treinta y pocos, dice: «Te mando ahora un resumen por correo». A los dos minutos llega. Es perfecto y suena a él: corto, con una broma sobre el retraso de la conexión, con una frase un poco torcida («lo dicho, que nos ponemos con ello ya mismo»). Carmen sabe, porque él lo ha dicho en la reunión («yo todo esto lo hago con ChatGPT, eh»), que lo ha escrito con IA.

**«¿Cómo lo hace? Lo ha hecho en dos minutos y suena a persona. Yo tardo media hora y sueno a folleto. Seguro que estos jóvenes saben algún truco que yo no sé. Ellos se han criado con esto.»**
*[ANCL: E35 (la IA bien usada no se nota), A36 (la sensación de ir por detrás) · escena HIP]*

### 4. El Monólogo Nocturno

Las doce y diez de la noche. Luz apagada. Javier, su marido, ya duerme. Carmen tiene los ojos abiertos en la oscuridad. En la cabeza le da vueltas la frase de su responsable de hace dos semanas («escribes como un robot») mezclada con el «Recibido, lo vemos el jueves» del cliente. Y el pensamiento en bucle es este:

**«¿Y si lo saben todos? ¿Y si en la oficina comentan "la de los emails de ChatGPT" y nadie me lo dice a la cara? Yo lo he pensado de otros. Lo pensé de Raúl el mes pasado cuando mandó aquel correo con el "Claro, aquí tienes una versión mejorada" pegado arriba. Nos reímos todos. ¿Se estarán riendo de mí? Y lo peor es que no puedo dejar de usarlo, porque ahora todo el mundo va más rápido y si yo tardo el doble se nota más todavía. Pero si lo uso, se nota. Y si lo arreglo a mano, tardo el doble. No hay salida.»**
*[ANCL: C12, C15, E30 (los jueces comentan entre ellos), B22 / E29 (la frase meta), E33, B4 (rumiación nocturna sobre el estilo), A31 (anula el ahorro de tiempo) · escena HIP]*

### 5. El Detonante de Compra (The Breaking Point)

El jueves, la reunión con el cliente. Todo va bien hasta que, al final, el cliente (al que Carmen lleva doce años) le dice, con una sonrisa que no es del todo una sonrisa: **«Por cierto, el último presupuesto que me mandaste… ¿lo escribiste tú o ChatGPT? Porque no parecías tú.»**

Carmen se ríe, dice algo como «uy, qué va, es que lo escribí con prisas», y nota cómo le sube el calor a las orejas. En el coche, de vuelta, con las manos apretadas en el volante en un semáforo, lo dice en voz alta, sola:

**«Basta. O aprendo a usar esto bien o lo dejo. Pero así no sigo ni una semana más.»**
*[ANCL: F1 («Did ChatGPT write this?»), C11 (relación comercial larga dañada), E19 (cliente que sospecha) · escena y detalles sensoriales HIP]*

---

## Mapa emocional del momento de compra (Mood Meter)

**Eje 1, valencia:** **negativa**. Llega con hartazgo y con miedo, no con esperanza activa. **[ANCL: el vocabulario emocional del corpus es casi exclusivamente negativo: crazy, maddening, embarrassing, insulting, freaking out, hate]**

**Eje 2, energía:** **mixta, con predominio de la baja energía en el target real.**
- El corpus muestra mucha **energía alta** («driving me crazy», «I hateee it!!», mayúsculas, exclamaciones). Pero es la energía de quien **escribe en un foro** justo después del incidente, y eso sobrerrepresenta el pico.
- El comprador típico, en el momento de encontrarse con el anuncio (de noche, tras el día, en scroll pasivo), está **cansado y escéptico**: «otra vez esto», «ya lo he probado todo». **[HIP con anclaje A27 (tras 6-8 intentos), A31, F2]**

**Cuadrante dominante: ANSIEDAD (baja energía + negativo).**
**Por qué:** el estado más común no es la rabia activa, sino la **vigilancia cansada**. Reescribe sin protestar, revisa tres veces y vive con un «¿se notará?» de fondo. La palanca de las cuatro fuerzas (reducir la ansiedad) y la inacción por ansiedad confirman el cuadrante.

**Cuadrante secundario: FRUSTRACIÓN (alta energía + negativo)**, justo después de un incidente (comentario del jefe o del cliente, frase meta pegada, cargo de un humanizador).

**Implicación concreta para el ritmo del copy (cuadrante Ansiedad):**
- **Frases cortas.** Una idea por frase y párrafos de una a tres líneas.
- **Densidad de información baja al principio y creciente después.** Primero el reconocimiento, luego la explicación y luego los detalles.
- **Pasos claros y numerados** (las cuatro huellas, los pasos de la configuración).
- **Sin presión**: nada de cuentas atrás, mayúsculas o «¡AHORA!».
- **La oferta, pronto pero sin empujar.** Mencionar el precio único y la garantía en el primer tercio, como alivio de la ansiedad («y no, no es una suscripción»), y hacer la llamada a la acción formal al final.
- **Tono de acompañamiento:** «te lo enseño paso a paso», «no tienes que saber nada técnico».

**Si hay más de un cuadrante, cuál priorizar y en qué pieza:**
- **Landing principal, emails de secuencia, contenido orgánico → Ansiedad** (calma, estructura, seguridad).
- **Anuncios de retargeting tras búsquedas de crisis** («mi jefe dice que suena a chatgpt», «cliente me ha preguntado si uso chatgpt») **→ Frustración**: copy directo que valida el hartazgo y ofrece contraste inmediato («Lo que te ha pasado tiene una explicación. Y un arreglo que haces una vez»). Ritmo ágil.
- **Nunca Ilusión** (alta energía + positivo): el tono aspiracional de «¡la IA va a transformar tu forma de escribir!» rebota en este mercado.

---

## Herida Central

### 1. Los 2-3 Recursos Ontológicos más amenazados

1. **Validación cultural o social** (ser percibido como auténtico, honrado, «de los nuestros»). Que se note la IA amenaza con convertirle en el falso, el vago, el que hace trampa (C27, E19, E21, E16).
2. **Títulos profesionales y logros** (la competencia profesional y el valor de su trabajo). «Si esto lo escribe la máquina, ¿qué aportas tú?» Es el cliente que pide descuento (E19), las 50 horas despachadas (F7) o el copywriter que dimite al ver su trabajo convertido en IA (C6).
3. **Capacidad intelectual y adquisición de conocimiento** (sentirse capaz, vigente, no superado). Es la sensación de que la tecnología avanza más rápido de lo que puede asimilar (A36) y de que «los jóvenes saben un truco que yo no». **[residual en el corpus, central en el target]**

### 2. Conexión con la Herida Nuclear

- **Validación social → miedo a la expulsión del grupo.** Ser descubierto como «el que despacha con robot» es ser marcado como **alguien en quien no se puede confiar**. En su extremo existencial, es el miedo a quedarse **solo**: que los demás dejen de leerle, de contestarle y de considerarle una persona real (C7: «tan intercambiables que ya no distingue a una persona de otra»). Es la aniquilación como **disolución en la masa de máquinas**.
- **Logros profesionales → miedo a ser reemplazable.** Si su texto es indistinguible del de una IA, **él es sustituible por la IA**. La herida aquí es la del **trabajador que deja de ser necesario**: el miedo a la irrelevancia, que es una forma de muerte social. **[ANCL C6, C14 + HIP de profundidad]**
- **Capacidad intelectual → miedo a quedarse atrás, a envejecer de golpe.** «La tecnología me ha superado» es, en el fondo, «el mundo sigue sin mí». Es la versión digital del miedo al abandono: el tren que se va. **[HIP con anclaje A36, E46]**

### 3. Frases en primera persona (voz natural, cruda, de madrugada)

1. «Si lo que escribo yo y lo que escribe la máquina suena igual, ¿para qué me quieren a mí? Cualquier día me lo dicen.» **[ANCL C6, E19, F7 · DATO INSUFICIENTE: falta un anclaje sensorial directo en el corpus]**
2. «Lo que me aterra no es que me pillen una vez. Es que ya lo sepan todos, que lo comenten cuando no estoy y que un día me dé cuenta de que hace meses que nadie me toma en serio.» **[ANCL C12, C15, E30, A17 «people don't take it seriously»]**

### 4. Implicación para el copy: tocar la herida sin abrirla

- **Tocarla:** con la **escena social reconocible** (el comentario, la pregunta del cliente) y con la norma del grupo («que se note, no»). El lector siente el pinchazo y se reconoce.
- **No abrirla:** **nunca** decir «la IA te va a reemplazar», «vas a quedar obsoleto», «los jóvenes te van a pasar por encima» ni «tu jefe ya sabe que no aportas». Eso convierte la empatía en amenaza y dispara la ansiedad, que es justo la fuerza que hay que bajar. Tampoco recrear la humillación con detalle morboso.
- **Cerrarla:** con **control y agencia**: «tú sigues siendo quien escribe; la IA solo aprende a sonar como tú». La herida de la sustitución se cura **devolviendo la autoría**: la configuración es **suya**, describe **su** voz y la máquina se convierte en **su** herramienta, no en su sustituta.
- **La diferencia entre conectar y manipular:** conectar es nombrar lo que ya siente para aliviarlo. Manipular sería inventar o inflar un riesgo («te van a despedir») para venderle. Con este mercado, además, la manipulación es ineficaz: el lector es juez experto en detectar falsedad.

---

## Frases de Looping (el espejo)

1. **«Lo que estás viviendo es esto: le pides a ChatGPT que te ayude con un email, te lo devuelve perfecto y no puedes mandarlo, porque no eres tú. Y tiene todo el sentido que te sientas así, porque tú también recibes emails así de otros, y sabes muy bien lo que piensas cuando los lees.»**
   *(Base: A4, E13, E48, C4. Causa real, no obvia: el lector es también juez.)*

2. **«Si sientes que te pasas más rato arreglando lo que escribe la IA que si lo hubieras escrito tú, probablemente no es que la uses mal. Es que cada vez que le pides "más natural" le estás pidiendo que adivine cómo hablas, y no lo sabe.»**
   *(Base: E22, A31, A20, A26. Insight no verbalizado: el problema es la falta de información sobre ti, no tu habilidad.)*

3. **«No es que te falte saber de tecnología. Es que nadie te ha dicho que ChatGPT viene configurado para sonar a asistente educado, y que se le puede decir, una sola vez, que hable como tú.»**
   *(Base: A35, A36, E38. Reencuadre que valida sin condescender: el defecto es de fábrica, no tuyo.)*

4. **«La mayoría de la gente en tu situación ha probado a pedirle que no suene a IA, a meterle una lista de palabras prohibidas o a pasar el texto por una de esas webs que lo "humanizan". Y si no te funcionó, no es casualidad: quitar palabras no pone tu voz, y las webs reescriben a ciegas un texto que ya salió mal.»**
   *(Base: E12, A29, E9, D19, D34.)*

5. **«Te da vergüenza que se note que usas ChatGPT. Y te da todavía más vergüenza que, después de un año usándolo, sigas sin saber hacer que no se note.»**
   *(Base: E6 «un año usando IA, los mismos clichés ya dan vergüenza», E33, A36. Es el pensamiento que no se dice en voz alta.)*

**Comprobación de calidad:** las cinco suenan a monólogo interno y no contienen jerga. Ninguna promete nada (el looping devuelve, no vende). La n.º 5 es la más arriesgada: debe ir seguida **inmediatamente** de alivio («no es culpa tuya, y se arregla en una tarde») para no abrir la herida.

### Cadena de beneficio adaptada a este mercado (Dimensiones del Beneficio)

> **Nota sobre el prompt:** el bloque original incluye una tabla de «Dimensiones del Beneficio» redactada para un mercado de salud intestinal (es un residuo de otra plantilla) y pide seguir «la estructura de la Cadena de Deseo», que no se define en el prompt. La interpreto como la cadena **dimensión del problema → beneficio deseado → resultado concreto y tangible en la vida del prospecto** y adapto las diez dimensiones a este mercado, aplicando las directrices (lenguaje casual, frases cortas, verbo activo, beneficio real y concreto, sin corchetes en el resultado).

| Dimensión | Beneficio deseado (en este mercado) |
|---|---|
| 1. Psicológico → (alivio) | Dejar de vivir con el «¿se notará?» de fondo cada vez que envías algo. |
| 2. Claridad causal (Baja → Alta) | Saber exactamente qué es lo que delata a la IA, para verlo y quitarlo de raíz. |
| 3. Visibilidad (Alta → Baja) | Que lo que mandas deje de llevar la «marca» que cualquiera reconoce en la primera línea. |
| 4. Urgencia (Alta → Baja) | Que el email de las once de la noche deje de ser una emergencia. |
| 5. Estigma social (Alto → Bajo) | Usar la IA sin sentir que haces trampa ni que te van a señalar. |
| 6. Medibilidad (Baja → Alta) | Notar el cambio en minutos: de media hora a cinco por email. |
| 7. Frecuencia (Alta → Baja) | Pasar de pelearte con la IA en cada texto a configurarla una vez. |
| 8. Locus de control (→ Interno) | Que tu IA haga lo que tú le has enseñado, no lo que trae de fábrica. |
| 9. Intensidad emocional (Alta → Baja) | Que desaparezca ese nudo al darle a enviar. |
| 10. Primera persona (Yo → Otros) | Que tu cliente y tu jefe vuelvan a leerte a ti, no a una máquina. |

**Tres nuevos ejemplos aplicando la cadena** (dimensión → beneficio → resultado tangible, al estilo del ejemplo correcto «Notarás que ese crujido molesto en tus rodillas ha desaparecido»):

1. **Frecuencia (Alta → Baja):** «Abres ChatGPT el lunes. Le pides el email. Lo lees una vez. Lo mandas. Ni lo tocas. Y el martes igual. Ya no le repites "más natural" cada vez.»
2. **Visibilidad (Alta → Baja):** «Tu cliente lee tu email y contesta a lo que le cuentas. No pregunta quién lo ha escrito. Porque ya no lleva el "espero que estés bien" que delata a la máquina.»
3. **Intensidad emocional (Alta → Baja):** «Le das a enviar y cierras el portátil. Sin releerlo tres veces. Sin mirar el móvil a las siete de la mañana a ver qué ha contestado. Duermes. Y punto.»

---

## Jerarquía de Resonancia

> Experiencias ⇒ Creencias ⇒ Valores ⇒ Identidades. Este mercado es un **colectivo de experiencias compartidas** alrededor de un hecho reciente: la llegada masiva de la IA a la escritura cotidiana y el aprendizaje, igual de masivo, de cómo detectarla.

### EXPERIENCIAS

**Pasadas** (las frustraciones que le hicieron reconocer que sí había un problema):
1. La primera vez que pegó un borrador en ChatGPT con un «mejóralo» y lo que volvió **no era él**. Lo mandó igual y alguien lo notó, o no lo notó nadie pero él pasó el día inquieto. **[ANCL F4, A4]**
2. La vez que **recibió** un email de IA de un compañero, de un proveedor o de su jefe y sintió ese rechazo instantáneo de «no se ha molestado ni en leerlo» (C4, C12, C13, E13). Desde entonces sabe lo que piensan los demás. **[ANCL]**
3. La vez que pidió «que suene más natural» y le salió algo más artificial (A20, E12). **[ANCL]**
4. El comentario: «¿esto lo has escrito con ChatGPT?» (F1), «suena a ChatGPT» (F7), «escribes como un robot» (A5). **[ANCL]**
5. La reseña de Trustpilot, o el cargo en su propia tarjeta, de una web «humanizadora» (D8, D14, D25). **[ANCL]**
6. El compañero al que pillaron con la frase meta pegada y del que todos se rieron (B22, C18, E29). **[ANCL]**
7. Las instrucciones que funcionaron un rato y luego dejaron de funcionar (A19). **[ANCL]**

**Presentes** (lo que pierde o deja de disfrutar ahora):
1. **El tiempo**: media hora por cada email que debería costar cinco minutos (F2).
2. **La tranquilidad al enviar**: el «¿se notará?» de fondo (F6).
3. **La confianza en su propio criterio**: ya no sabe si lo que escribe él mismo suena a IA (A13).
4. **El ahorro prometido**: el límite de uso se le va corrigiendo el tono (A28).
5. **La espontaneidad**: ha dejado de usar ciertos signos y ciertas palabras por miedo (A6, B5).
6. **La ayuda en lo importante**: evita la IA justo donde más le serviría (propuestas, cartas delicadas). **[HIP]**
7. **La autoría**: lo que firma no es del todo suyo, y lo sabe (F3).

**Futuras** (lo que teme si no se resuelve):
1. Que **un cliente importante** se vaya o pida descuento al «olerlo» (E19).
2. Que su **jefe deje de confiar** en sus textos y le supervise (A5, C27).
3. Que su **reputación** se erosione en silencio: ser «el de los emails de robot» sin saberlo (C12, C15).
4. **Quedarse atrás** mientras los demás usan la IA «bien» (A36, E35).
5. Que **llegue un momento en que ya no sepa escribir** sin la máquina (A13).
6. Que la empresa le **obligue** a usar IA para todo y el problema se multiplique (C14, E15).

### CREENCIAS (mínimo 5 por categoría)

**Creencias sobre sí mismos:**
1. «Yo no soy técnico.» (A36)
2. «Yo no soy escritor; no tengo "una voz" como los que escriben de verdad.» (A22)
3. «Llego tarde a todo esto.» (E46) **[residual]**
4. «Yo escribo normal, pero ChatGPT me hace sonar raro.» **[ANCL A4]**
5. «Soy honrado: la uso para ayudarme, no para engañar a nadie.» **[ANCL C27, E34]**
6. «Si fuera más listo con esto, ya lo habría arreglado.» **[HIP]**

**Creencias sobre el problema en sí:**
1. «La IA escribe así y no hay manera de cambiarlo del todo.» (A33)
2. «El problema son ciertas palabras.» (E-bloque, creencia insider que se filtra) **[ANCL]**
3. «Se nota porque es demasiado perfecto.» (E45, C4, B4) **[ANCL]**
4. «Cada vez es peor: antes escribía mejor.» (A34) **[ANCL]**
5. «Todo el mundo lo nota, aunque no sepa explicar el qué.» (C23) **[ANCL]**
6. «Es un problema de prompts: si supiera preguntar, saldría bien.» **[HIP con anclaje E24]**

**Creencias sobre su capacidad para resolverlo:**
1. «Si los que saben de esto no lo consiguen con prompts, yo menos.» (A29, A30) **[ANCL]**
2. «Para arreglarlo tendría que aprender cosas técnicas que no me da la vida para aprender.» **[HIP con anclaje A36]**
3. «La única forma segura es reescribirlo yo.» (E36, A31) **[ANCL]**
4. «Ya lo intenté y no me salió.» (A26, A27) **[ANCL]**
5. «Podría, si alguien me lo explicara despacio y sin palabrejas.» **[HIP]**

**Creencias sobre cómo afecta el problema a su autoestima:**
1. «Que se note me hace quedar como un vago.» (E21, C4) **[ANCL]**
2. «Que se note me hace quedar como un falso.» (C19, E42) **[ANCL]**
3. «Si mi texto suena a máquina, ¿qué estoy aportando yo?» (C6, C14) **[ANCL]**
4. «Me da vergüenza no saber hacerlo, después de tanto tiempo usándolo.» (E6) **[ANCL]**
5. «Me siento un poco tramposo aunque no lo sea.» **[HIP con anclaje E19]**

**Creencias sobre el mercado:**
1. «Todo lo que se vende para esto es una estafa.» (D1, D6)
2. «Te enganchan con la prueba gratis y luego te cobran el año.» (D8, D14)
3. «Prometen 100 % humano y no lo cumple ninguno.» (D12, D18, D31)
4. «Los detectores no sirven para nada.» (B18, B20, E9)
5. «Esto lo arreglarán ellos (OpenAI, Anthropic) tarde o temprano.» **[ANCL A19]**
6. «Los que venden cursos de IA no saben escribir.» **[HIP]**

**Creencias sobre las soluciones populares (específicas):**
1. **Humanizadores:** «Te destrozan el texto: palabras que no existen, mayúsculas en medio, el sentido cambiado.» (D23, D30, D33, D40)
2. **Humanizadores:** «Lo que hoy funciona, mañana no, cuando actualizan el detector.» (D28, D29)
3. **Prompts «que suene natural»:** «Funcionan un rato y luego vuelve a lo de siempre.» (A19, A25)
4. **Listas de palabras prohibidas:** «Quitas las palabras y sigue sonando igual.» (A29) / «Si las evitas todas, también suena a IA.» (E9)
5. **Instrucciones personalizadas copiadas de internet:** «Son de otro; no suenan a ti.» **[HIP con anclaje A29]**
6. **Reescribir a mano:** «Funciona, pero entonces no me ahorro nada.» (A31)
7. **Correctores con IA:** «Hasta corregir la gramática te puede hacer sonar a IA.» (B12, B13)

**Creencias sobre «expertos» o autoridades concretas:**
1. «Los gurús de la IA te venden prompts que ellos mismos no usan.» **[HIP]**
2. «Los de LinkedIn que te dicen cómo sonar humano escriben todos igual.» **[HIP con anclaje F6, F2]**
3. «Los de las herramientas te dicen que su detector da 100 % humano, pero claro, es su detector.» (D31) **[ANCL]**
4. «Los profesores y los jefes se creen el detector más que a ti.» (B11, B7) **[ANCL; más del segmento estudiante]**
5. «Los de Reddit que saben mucho hablan de cosas que yo no entiendo (*em dashes*, *tells*…).» **[HIP con anclaje E-bloque]**

**Creencias sobre lo que ocurre después de resolverlo («Si pudiera X, me sentiría Y»):**
1. «Si la IA escribiera como yo, me ahorraría una hora al día.» **[ANCL F2 + cálculo HIP]**
2. «Si dejara de notarse, me atrevería a usarla para las propuestas grandes.» **[HIP]**
3. «Si supiera por qué pasa, dejaría de sentirme tonto.» **[ANCL C23, A35]**
4. «Si lo dejara configurado, me olvidaría del tema para siempre.» **[ANCL E53]**
5. «Si no se notara, me sentiría otra vez dueño de lo que firmo.» **[ANCL F3]**

### VALORES

**Moneda principal:** **AUTENTICIDAD Y HONESTIDAD**, seguida de **EFICIENCIA Y PRODUCTIVIDAD** y **RESPETO Y ADMIRACIÓN**.
- Autenticidad: «que sea mío», «tiene que ser TU trabajo» (C27), «menos perfecto pero auténtico» (C4).
- Eficiencia: la razón por la que usa la IA (A31, E22, «defeats the purpose», A28).
- Respeto: lo que pierde cuando se nota (A17: «no lo toman en serio»).
- Valores secundarios: **Fiabilidad y constancia** (que la solución no se degrade, A19), **Simplicidad** (sin complicaciones técnicas) y **Transparencia** (sin cargos ocultos, D25).

**Estándares personales** (lo que está y no está dispuesto a hacer):
- **Sí:** dedicar **una** tarde a configurarlo bien, revisar el contenido (los datos, las cifras), pagar una vez una cantidad razonable y aprender **por qué** pasa si se lo explican con claridad.
- **No:** programar, pagar cada mes, pasar cada texto por otra web, meter faltas a propósito, fingir que no usa IA si le preguntan directamente **[HIP]** y copiar y pegar sin leer (le parece de vagos, E27, E29).

**Estándares externos** (lo que valora en los demás):
- **Que escriban como hablan** (C12: el salto entre cómo habla el jefe en persona y su «manager-speak» por email le parece falso).
- **Que se tomen la molestia** (C4: prefiere «menos perfecto pero auténtico»; E36: «have it write the email, and then rewrite it in your own words»).
- **Que no le vendan humo** (D-bloque).
- **Que vayan al grano** (E31: «the more efficient way… would be to just be terse»).
- **Reacciones sociales de otras personas** (lo que valoran los demás en él): lo mismo, el reflejo exacto. Sus jueces valoran la autenticidad, el esfuerzo visible y la brevedad. **Por eso lo que delata no es «usar IA», sino lo que la IA comunica sin querer: falta de esfuerzo y falta de persona.**

### IDENTIDAD

**Identidad actual:** «Soy un profesional que hace bien su trabajo, que usa ChatGPT para ir más rápido y que, la verdad, no tiene ni idea de cómo hacer que no se note. Lo arreglo como puedo.» **[ANCL compuesta]**

**Identidad aspiracional:** «Soy de los que usan la IA con cabeza: la tengo a mi medida, escribe como yo y nadie nota la diferencia, porque no la hay. Sigo siendo yo quien escribe.» **[HIP con anclaje E35, E34]**

**Avatares dismórficos (limitaciones de identidad):**
- **«El de los emails de ChatGPT»**: el miedo a ser ese compañero del que todos se ríen (C15, E30, E29). Es la versión temida de sí mismo.
- **«El abuelo de la tecnología»**: el que «tiene mil años» y no sabe (E46). **[residual]**
- **«El impostor»**: el que firma lo que no ha escrito (F3, A9).
- **«El tramposo»**: el que usa IA cuando «tiene que ser TU trabajo» (C27).

**Aliados y enemigos naturales:**
- **Aliados:** los que escriben claro y con voz propia (aunque usen IA), el compañero que «sabe de esto» y le echa una mano, los clientes que valoran el trato personal, quienes dicen que «usar IA responsablemente no debería ser un secreto» (E34).
- **Enemigos:** los humanizadores-estafa (D-bloque), los gurús de la IA que venden prompts mágicos **[HIP]**, los jefes que imponen IA para todo sin entenderla (C14, C23), los que copian y pegan sin leer (C3, E27) y, de forma más difusa, **«la voz por defecto de la IA»**, ese asistente educado y vacío que se cuela en todo (C22, A1).

---

## Polarización y Villanos

### 1. El Villano Sistémico (la Conspiración)

**La industria de los «humanizadores» y de la «IA mágica» que vive de que el problema no se resuelva nunca.**
- Los humanizadores **cobran por cada reescritura** (por palabras, por créditos, por suscripción). Su modelo de negocio **depende** de que vuelvas cada vez con un texto nuevo que «humanizar». Si tu IA escribiera bien desde el principio, no los necesitarías. **[ANCL D23 «consume miles de palabras del plan», D8, D36 + lectura del modelo de negocio]**
- Juegan a un **juego que no se puede ganar**: el del detector contra el humanizador. El detector se actualiza, el humanizador se «actualiza para superarlo» (D18) y tú pagas la carrera. D28 y D29: lo que funcionaba la semana pasada deja de funcionar.
- Y, de fondo, **la voz por defecto de las IAs**: los modelos vienen entrenados para sonar a «asistente servicial y correcto», y nadie te dice que esa voz se puede cambiar. **[HIP sobre el diseño, con anclaje A19, A34]**

**La «Mentira Noble» que se le ha contado y que vamos a destapar:**
**«Para que tu texto de IA no se note, necesitas otra herramienta que lo arregle después.»**
La verdad: el problema no está en el texto ya escrito, sino en **cómo está configurada la IA antes de escribirlo**. Arreglar después es poner tiritas. Configurar antes es no hacerse la herida. Segunda mentira noble, más sutil: **«Para usar bien la IA hay que saber de tecnología.»** La verdad: hay que saber **cómo hablas tú**, y eso lo sabes mejor que nadie.

### 2. El Villano Directo (el Antagonista)

- **«El vendedor de 100 % humano»**: la web que te promete indetectable, te enseña un porcentaje en su propio detector («100 % humano») mientras cualquier otro dice «100 % IA» (D31) y te cobra el año entero cuando el anuncio decía «al mes» (D14).
  - *Frases condescendientes:* «Nuestro modelo avanzado garantiza un texto indistinguible del humano.» «¡Cancela cuando quieras!» «Te ofrecemos créditos como compensación» (D10). **[ANCL + HIP de formulación]**
- **«El gurú del prompt»**: el que te dice que todo es cuestión de saber preguntar y te vende 200 prompts en un PDF.
  - *Frases:* «Si ChatGPT te escribe mal, es que no sabes hacer prompts.» «Copia este prompt mágico.» **[HIP]**
- **«El jefe fanático de la IA»**: el que exige usar la IA para todo y luego se queja de que suena a IA (C14, C23, E15).
  - *Frases:* «¿Por qué no lo hacéis todo con IA?» (C23). «Usa la herramienta, que tardas mucho» (E15). **[ANCL]**
- **(Antagonista secundario) «El experto de foro»**: el que te explica con desdén lo que son los *em dashes* y los *tells* como si fuera obvio. **[HIP con anclaje E-bloque]**

### 3. La «Piedra que tiramos»

**Hacia quién o qué tirar piedras:** hacia **los humanizadores como categoría** (nunca con nombres de marca en el copy público) y hacia **la idea de «arreglar después»**. Secundariamente, hacia **el mito de que hace falta ser técnico**.

**La frase completa:**
> **«Nosotros NO somos como las webs que "humanizan" tu texto, porque nosotros creemos en que lo que escribes sea tuyo desde el principio y para siempre, mientras que ellas solo quieren que vuelvas cada mes a pagar por arreglar lo que tu IA vuelve a escribir mal.»**

Variante contra el gurú:
> «Nosotros no somos como los que te venden 200 prompts, porque nosotros creemos en que tú no tengas que aprender a hablar como una máquina, sino que tu máquina aprenda a hablar como tú. Ellos solo quieren que dependas de su siguiente pack.»

**Objetivo cumplido:** el argumento «nosotros contra ellos» **alivia la culpa** («no es que tú lo hicieras mal, es que te vendieron una solución diseñada para no acabar nunca») y **dirige la ira** hacia afuera (la industria del parche).

**Riesgo:** no tirar piedras **a la IA en sí** ni **a quien la usa**. El prospecto la usa y la quiere seguir usando. Atacar la IA le colocaría en el bando de los «antiIA» (r/NoAiWriting, r/BetterOffline), que no es el suyo. Tampoco tirar piedras a «los que copian y pegan», porque el lector ha sido uno de ellos.

---

## Restricciones de Jerarquía de Resonancia (Bloqueos)

### Bloqueos de IDENTIDAD

**CONSTRAINT 1:** «Yo no soy técnico. Esto de configurar la IA es para gente que sabe.»
**ASSUMPTIONS:** que configurar es una tarea técnica; que hay que entender cómo funciona por dentro; que «los que saben» tienen una habilidad que él no tiene.
**DISSOLUTION FORMULA (Analogía):** «Te entiendo perfectamente. Si nunca has tocado los ajustes de ChatGPT, eso de "configurar" suena a cables y a pantallas negras. Es como cuando creíamos que para tener la tele "bien puesta" había que llamar al técnico. Luego resultó que era darle a un botón del mando y elegir el idioma. Esto es igual: un menú que ya está en tu ChatGPT, en español, donde escribes cómo hablas tú. Si sabes escribir un email, sabes hacer esto.»
**REASONING:** la analogía con un aparato doméstico conocido (la tele, el mando) baja la complejidad percibida sin decirle al lector que lo que siente es una tontería. Encaja con la tarea vital de control y con el subgrupo veterano.

**CONSTRAINT 2:** «Yo no soy escritor. No tengo "una voz" que enseñarle.»
**ASSUMPTIONS:** que la voz es algo de escritores; que hay que escribir bien para tener estilo; que su forma de escribir es «normal», sin rasgos.
**DISSOLUTION FORMULA (Sabiduría contraintuitiva):** «Yo también pensaba así. Que "la voz" era cosa de novelistas. Hasta que leí algo que se escribió en un foro sobre IA: "toda escritura tiene una voz propia de esa persona, e incluso la escritura caótica, pobre o inconsistente tiene coherencia". Tu forma de saludar, las palabras que repites, lo largo o corto que escribes… eso es tu voz. No hace falta que sea bonita. Hace falta que sea tuya. Y tu cliente la reconoce aunque tú no.»
**REASONING:** usa una cita real del corpus (E3) como «sabiduría» de tercero. Rompe la creencia sin elogiar en exceso al lector.

**CONSTRAINT 3:** «A mi edad ya no me pongo con estas cosas.»
**ASSUMPTIONS:** que la edad determina la capacidad de aprender tecnología; que esto exige un aprendizaje largo.
**DISSOLUTION FORMULA (Reencuadre):** «Te entiendo. Llevas años viendo cómo cada cosa nueva viene con un manual más gordo. Pero considera esto: aquí no tienes que aprender la tecnología, tienes que enseñarle a la tecnología cómo eres tú. Y en eso tienes ventaja: llevas más años escribiendo emails, tratando clientes y sabiendo cómo hablas. Lo que significa que lo difícil de esto ya lo tienes hecho.»
**REASONING:** invierte la relación (el que aprende es la IA) y convierte la experiencia en ventaja. **Uso con cautela:** la mención explícita a la edad puede ser un disparador de expulsión. Mejor usarlo en piezas segmentadas que en la landing general.

### Bloqueos de VALORES

**CONSTRAINT 4:** «Si uso algo para que no se note la IA, estoy engañando a mi cliente.»
**ASSUMPTIONS:** que hacer que el texto suene a él es ocultar algo; que la autenticidad depende de no usar herramientas; que «que no se note» equivale a «mentir».
**DISSOLUTION FORMULA (Reencuadre):** «Te entiendo, y dice mucho de ti que te lo plantees. Pero considera esto: lo que molesta a tus clientes no es que uses una herramienta, igual que no les molesta que uses el corrector del Word. Lo que les molesta es recibir algo que no suena a ti, porque parece que no te has molestado. Si tu IA escribe como tú hablas, con tus ideas y tu forma de decirlo, no estás ocultando nada: estás devolviendo al email lo que faltaba, que eras tú.»
**REASONING:** se apoya en E35 y C4 (lo que molesta es la falta de persona, no la herramienta) y alinea el producto con el valor de autenticidad en lugar de chocar con él.

**CONSTRAINT 5:** «No quiero gastar dinero en esto; ya he tirado bastante en herramientas que no funcionan.»
**ASSUMPTIONS:** que este producto pertenece a la misma categoría que los humanizadores; que pagar implica seguir pagando; que la decepción anterior predice la siguiente.
**DISSOLUTION FORMULA (Consecuencias):** «Entiendo perfectamente tu punto. Si ya te cobraron una suscripción por algo que te dejó el texto peor, lo último que quieres es volver a sacar la tarjeta. Pero pensemos en lo que eso implica: si sigues pensando que todo lo de esta categoría es igual, la única opción que te queda es seguir reescribiendo a mano. Media hora por email, cada día, sin final. Eso también cuesta, solo que no lo ves en el banco. Esto se paga una vez. Y, si no te convence, te devuelvo el dinero, no créditos.»
**REASONING:** la fórmula de consecuencias hace visible el coste oculto del statu quo (el tiempo), y la respuesta específica al agravio («no créditos», D10) separa el producto de la categoría.

### Bloqueos de CREENCIAS

**CONSTRAINT 6:** «La IA siempre va a sonar a IA. No tiene arreglo.»
**ASSUMPTIONS:** que el tono de máquina es inherente al modelo; que nadie lo ha conseguido; que las pruebas fallidas demuestran que es imposible.
**DISSOLUTION FORMULA (Experimento mental):** «Te entiendo. Después de tantos intentos, cualquiera lo pensaría. Pero pensemos un segundo: imagina que contratas a la persona que mejor escribe del mundo y el primer día no le dices nada de ti. Ni a quién escribes, ni cómo hablas, ni qué palabras no usarías jamás. ¿Cómo escribiría? Educada, correcta, genérica. Como un manual. ¿Sería culpa de su talento o de que nadie le explicó quién eras? Pues eso es lo que pasa con tu IA. No es que no pueda. Es que nadie se lo ha dicho bien.»
**REASONING:** el experimento mental (el empleado nuevo) desplaza la causa del «es imposible» al «falta información», que es controlable. Coincide con la metáfora recomendada en el Momento Aha.

**CONSTRAINT 7:** «Ya probé a darle instrucciones y no funcionó.»
**ASSUMPTIONS:** que todas las instrucciones son iguales; que si una falla, fallan todas; que el problema es la herramienta y no el contenido de las instrucciones.
**DISSOLUTION FORMULA (Paradoja):** «Entiendo tu punto de vista. Hay gente que lleva semanas probando instrucciones y sigue igual. Pero piensa en esta contradicción: un usuario contaba en un foro que le pidió a ChatGPT "no suenes a IA"… y le metió todos sus clichés de golpe. Cuantas más prohibiciones le das, más piensa en lo prohibido. Las instrucciones normales fallan porque dicen lo que no hacer y nunca dicen cómo eres tú. Es como describirle a alguien tu casa diciéndole que no es azul, que no tiene piscina y que no está en Madrid.»
**REASONING:** la paradoja (E12) es contraintuitiva y verificable. Explica por qué lo que ya probó falló sin culparle y abre la puerta a un enfoque distinto (en positivo, basado en su voz). **Atención: el producto tiene que cumplir esta distinción de verdad.**

**CONSTRAINT 8:** «Si quito las palabras típicas de la IA, ya está.»
**ASSUMPTIONS:** que el problema es léxico; que basta con una lista.
**DISSOLUTION FORMULA (Prueba social, con datos del propio mercado):** «Te entiendo completamente. Es lo que dicen la mitad de los artículos sobre esto. Pero considera esto: en los foros donde más se habla del tema, quienes probaron las listas de "palabras prohibidas" cuentan que les quitaron algunos tics, pero que el texto seguía sin sonar a ellos, y algunos dicen que evitarlas todas también suena a IA. Lo que sugiere que quizás las palabras son solo una de las huellas. ¿Es posible que lo que delata sea también cómo se construyen las frases, el tono de "asistente educado" y ese ritmo en el que todo mide lo mismo?»
**REASONING:** usa A29 y E9 como prueba social de tipo cualitativo. **No hay estadísticas fiables en el corpus**, así que no las invento. Prepara la explicación de las cuatro huellas.

**CONSTRAINT 9:** «Todo lo que se vende para esto es una estafa.»
**ASSUMPTIONS:** que este producto es de la misma categoría; que vender implica engañar.
**DISSOLUTION FORMULA (Reencuadre):** «Te entiendo. Si yo hubiera leído las reseñas que he leído de esas webs (cobros anuales que nadie esperaba, textos con palabras que no existen, devoluciones convertidas en créditos), también lo pensaría. Pero considera esto: todas esas webs tienen algo en común, y es que necesitan que vuelvas. Tú les pagas cada vez que escribes. Esto es justo lo contrario: lo configuras una vez en tu propia IA y no me vuelves a necesitar. Lo que significa que, si fuera una estafa, sería la peor estafa del mundo.»
**REASONING:** el reencuadre usa la lógica del modelo de negocio, que es verificable por el lector, para separar las categorías. El cierre con humor rebaja la tensión.

### Bloqueos de RECURSOS

**CONSTRAINT 10:** «No tengo tiempo para ponerme a configurar nada.»
**ASSUMPTIONS:** que configurar lleva mucho tiempo; que el tiempo invertido no se recupera.
**DISSOLUTION FORMULA (Consecuencias):** «Entiendo perfectamente tu punto. Vas a tope y lo último que quieres es otra tarea. Pero pensemos en lo que eso implica: si cada email importante te lleva media hora en lugar de cinco minutos, y escribes tres o cuatro al día, estás pagando más de una hora diaria en retoques. Cada día. Configurarlo te lleva una tarde, una sola vez. Lo recuperas el primer martes.»
**REASONING:** el cálculo usa F2 como base y hace visible el coste de no tener tiempo. Hay que advertir que el número es ilustrativo, no un dato medido.

**CONSTRAINT 11:** «No tengo ChatGPT de pago / mi empresa no me deja tocar los ajustes.»
**ASSUMPTIONS:** que el producto exige un plan concreto; que no hay alternativa.
**DISSOLUTION FORMULA (Reencuadre, con honestidad):** «Te entiendo, y es una pregunta muy sensata. Te lo digo claro: la configuración permanente funciona en [requisitos reales que tendrá que verificar el creador]. Si tu situación es otra, la guía te enseña además a crear tu "ficha de voz" en un documento propio que pegas al empezar cada conversación. No es tan cómodo como dejarlo puesto, pero suena igual de tuyo.»
**REASONING:** **[HIP de producto]**. Es un bloqueo real que el creador tiene que resolver en el producto. El copy no puede prometer compatibilidad universal sin verificarla. La fórmula modela la honestidad que el mercado premia.

### Bloqueos de EXPERIENCIA (recuerdos)

**CONSTRAINT 12:** «La última vez que pagué por algo así me cobraron el año entero.»
**ASSUMPTIONS:** que todos los vendedores de la categoría usan las mismas prácticas.
**DISSOLUTION FORMULA (Storytelling):** «Yo solía pensar igual. Es muy común creer que cualquier cosa de "IA" que se paga online viene con trampa. Luego leí la historia de una persona que vio un cargo en su cuenta y ni siquiera reconocía el nombre: tuvo que buscarlo en Google para saber que era la herramienta que creía haber cancelado. Por eso esto se paga una vez, con un precio que ves antes de pulsar, y sin nada que cancelar, porque no hay nada que se renueve.»
**REASONING:** la historia real del corpus (D25) valida su recuerdo y el producto se presenta como la respuesta directa a ese agravio.

**CONSTRAINT 13:** «Siempre que me prometen que la IA va a escribir como yo, acabo reescribiéndolo.»
**ASSUMPTIONS:** que la experiencia pasada predice el futuro; que el método anterior y el nuevo son el mismo.
**DISSOLUTION FORMULA (Desafío personal):** «Créeme, he estado ahí. Yo también estaba convencido de que, por mucho que hiciera, acabaría reescribiéndolo. Pero decidí ponerme a prueba: el mismo email, el mismo día, una vez con mi ChatGPT tal cual y otra con la configuración. Los imprimí y se los di a leer a alguien que me conoce sin decirle cuál era cuál. Me señaló el segundo sin dudar: "este eres tú".»
**REASONING:** **[HIP: requiere que el creador haga ese experimento real y lo documente]**. Si no se ha hecho, esta fórmula **no puede usarse** tal cual, porque sería inventar prueba. Se deja como **plantilla para cuando exista la prueba**.

---

## Epifanía — La Escala de Credibilidad

> Para este mercado: personas no técnicas que usan ChatGPT o Claude para escribir en el trabajo y quieren que no se note. Diez ideas por nivel. La credibilidad baja a medida que sube el nivel. **Zona Goldilocks: 6,1-7,9.**

### Nivel 1 — Lo obvio («¿Y a mí qué?»)
1. Los textos de ChatGPT suenan a ChatGPT.
2. Hay que revisar lo que escribe la IA antes de enviarlo.
3. La IA escribe de forma muy formal.
4. A la gente no le gusta recibir mensajes de robot.
5. La IA comete errores.
6. Cada persona escribe de una forma distinta.
7. Hay herramientas que dicen que «humanizan» el texto.
8. Se tarda tiempo en corregir lo que escribe la IA.
9. ChatGPT usa siempre las mismas expresiones.
10. Es mejor que un email suene natural.

### Nivel 2 — Conocido, poco interesante
1. Si le das más contexto a la IA, escribe un poco mejor.
2. Los emails de IA suelen ser demasiado largos.
3. La IA abusa de las listas y las negritas.
4. Las frases de saludo de ChatGPT son muy típicas.
5. Hay palabras que delatan que un texto es de IA.
6. Los detectores de IA no son fiables.
7. Pedirle «más casual» ayuda un poco.
8. Los humanizadores tienen muy malas reseñas.
9. Los jefes notan cuando un email es de IA.
10. Escribir con tus propias palabras es lo más seguro.

### Nivel 3 — Útil pero visto
1. Dar ejemplos de tus textos ayuda a que la IA imite tu estilo.
2. ChatGPT tiene unos ajustes donde puedes decirle cómo quieres que escriba.
3. Los humanizadores muchas veces empeoran el texto.
4. Quitar las frases hechas mejora mucho el resultado.
5. Lo que delata a la IA no es solo el vocabulario.
6. Las instrucciones que le das al principio se le «olvidan» en conversaciones largas.
7. Un texto demasiado perfecto parece menos humano.
8. El mismo texto da resultados distintos en cada detector.
9. Las frases cortas hacen que suene más natural.
10. Hay quien le dice a la IA que el idioma es su segunda lengua para que suene menos formal.

### Nivel 4 — Interesante, empieza a despertar
1. Pedirle a ChatGPT «que no suene a IA» lo hace sonar todavía más a IA.
2. Lo que de verdad delata a la IA es que todas las frases miden más o menos lo mismo.
3. La IA viene programada para sonar a «asistente educado», y por eso todo suena a atención al cliente.
4. Las listas de palabras prohibidas pueden hacer que el texto suene a IA «disfrazada».
5. A nadie le molesta que uses IA: le molesta que se note.
6. Tu cliente detecta un email de IA en la primera línea, aunque no sepa decir por qué.
7. Las herramientas «humanizadoras» ganan más cuanto peor escribe tu IA.
8. Los tics de la IA cambian con cada versión, así que las listas caducan.
9. Un email «humanizado» por una web puede cambiar lo que querías decir.
10. Corregir la gramática con IA puede hacer que tu propio texto suene a IA.

### Nivel 5 — Sorprendente, todavía «normal»
1. Hay cuatro huellas concretas que delatan cualquier texto de IA, y las palabras son solo una de ellas.
2. Tu IA no escribe mal: escribe como alguien a quien nadie le ha dicho quién eres.
3. Puedes ver las cuatro huellas en cualquier email de IA en menos de un minuto, una vez sabes dónde mirar.
4. Las mismas palabras que te ponen nervioso en un email de IA las tienes que buscar también en los tuyos.
5. La forma en que saludas y te despides dice más de tu voz que cualquier palabra «bonita».
6. Para que la IA suene a ti, es más útil decirle cómo hablas que decirle lo que no debe hacer.
7. Un email con alguna frase un poco torcida convence más que uno perfecto.
8. Pasar el texto por una web después de escribirlo es arreglar el síntoma; la causa está antes.
9. Lo que la gente llama «tono de ChatGPT» es, en realidad, el tono de un manual de atención al cliente.
10. Si te pasas media hora retocando cada email, la IA te está costando tiempo en lugar de ahorrártelo.

### Nivel 6 — En el borde (6,1-6,9) ✦ Zona Goldilocks baja
1. **Puedes dejar configurado tu ChatGPT en una tarde para que escriba con tu forma de hablar desde el primer mensaje, sin saber nada de programación.**
2. **No necesitas otra herramienta: la solución está dentro del ChatGPT que ya usas, en un menú que casi nadie toca.**
3. **El motivo por el que «suena a IA» tiene nombre y cuatro partes, y cuando lo ves ya no puedes dejar de verlo.**
4. **Si sabes escribir un email, sabes enseñarle a tu IA a escribir como tú.**
5. **Configurarlo una vez te ahorra el «más natural, por favor» de cada día.**
6. **Lo que hacen los humanizadores después, tú lo puedes evitar antes, y gratis a partir de entonces.**
7. **Tu IA puede aprender a no meter nunca más el «Espero que este mensaje te encuentre bien».**
8. **Tus textos con IA pueden llegar a sonar más a ti que los que escribes con prisas a mano.**
9. **El email de cinco minutos puede volver a durar cinco minutos.**
10. **La forma de que no se note la IA no es quitar cosas, sino darle una cosa: tu voz.**

### Nivel 7 — Casi demasiado bueno (7,0-7,9) ✦ Zona Goldilocks alta
1. **Le pides el email, lo lees una vez y lo envías. Ni lo tocas.**
2. **Tu cliente de toda la vida no distinguiría un email tuyo escrito con tu IA de uno que hayas escrito tú.**
3. **En una tarde dejas tu IA ajustada a ti para siempre, y no vuelves a pagar nada.**
4. **Después de configurarla, el que va a tener que preguntarte «¿cómo lo haces?» va a ser tu compañero.**
5. **Tu ChatGPT puede escribir tu propuesta importante con tu voz, la que antes no te atrevías a pedirle.**
6. **Dejas de releer tres veces antes de enviar.**
7. **La misma configuración sirve para emails, mensajes, posts y propuestas, cada una en su tono, sin que dejes de sonar a ti.**
8. **Recuperas una hora al día que se te iba en retocar lo que escribía la máquina.**
9. **Puedes coger cualquier email de IA y decir exactamente qué lo delata, y arreglarlo en un minuto si hiciera falta.**
10. **Tu IA puede escribir como tú incluso cuando tú estás cansado y escribirías peor.**

### Nivel 8 — Límite del BS (empieza a costar creerlo)
1. Nadie, nunca, volverá a notar que usas IA.
2. Tu IA escribirá exactamente igual que tú, palabra por palabra.
3. En diez minutos tendrás una IA que escribe mejor que tú.
4. No tendrás que revisar ningún texto nunca más.
5. Tus emails pasarán todos los detectores de IA del mundo.
6. Tus clientes te darán más trabajo porque escribirás mejor.
7. Tu jefe te ascenderá por cómo escribes.
8. Funciona igual en cualquier IA, versión e idioma, para siempre.
9. Te convertirás en «el que mejor escribe» de tu empresa.
10. Ahorrarás 20 horas a la semana.

### Nivel 9 — Exagerado
1. Tu IA leerá tu mente y escribirá lo que piensas sin que se lo pidas.
2. Escribirás un libro con tu voz en un fin de semana.
3. Con esto podrás despedir a tu redactor, a tu agencia y a tu secretaria.
4. Tus emails convertirán el triple.
5. Ganarás más dinero solo por cambiar el tono de tus correos.
6. Nunca más tendrás que escribir nada tú.
7. Es imposible que nadie detecte jamás tu IA, ni humano ni máquina.
8. Tus clientes se enamorarán de tus emails.
9. Te convertirás en un escritor profesional sin esfuerzo.
10. Tu IA escribirá mejor que los mejores copywriters del mundo.

### Nivel 10 — «Ni de broma»
1. Tu IA escribirá premios literarios en tu nombre.
2. Podrás jubilarte gracias a tus emails.
3. Tu ChatGPT tomará decisiones de negocio por ti con tu voz y nadie lo sabrá.
4. Una configuración de cinco minutos te convertirá en millonario.
5. Tu IA será indistinguible de ti incluso para tu familia por teléfono.
6. No volverás a trabajar más de una hora al día.
7. Tus correos harán que tus clientes te paguen el doble.
8. Tu IA te sustituirá en las reuniones y nadie se dará cuenta.
9. Escribirás en cualquier idioma como un nativo de ese país sin saberlo.
10. Esta guía hará que la IA no vuelva a cometer ningún error jamás.

**Selección para copy (Zona Goldilocks):** las ideas **6.1**, **6.3**, **6.10**, **7.1**, **7.2** y **7.6** son las más potentes. La **7.1** («Le pides el email, lo lees una vez y lo envías») es la candidata a promesa central, porque es concreta, visualizable y está «casi demasiado bien», pero es plausible si se demuestra. La **6.3** es el gancho del PDF. La **6.10** es la Big Idea en versión explicativa. **Cuidado con la 7.2 y la 7.8**: hay que formularlas como posibilidad, no como garantía, y la 7.8 solo con el cálculo explicado.

---

## Mecanismos Interoceptivos

> Producto no físico, adaptado según indica el prompt. Base corporal real en el corpus: «my soul left my body» (C1), «my brain just turns off» (E48), «bad taste in my mouth» (E27), «ganas de vomitar» (E39), «Ouch my heart» (A15), «keeps me awake» (B4), «freaking out» (B7, B15), «cringe» (A27), «tirar el MacBook al río» (C7). Hay pocas sensaciones corporales literales y casi todas son de jueces o de estudiantes, así que **las localizaciones corporales concretas del emisor adulto son [HIP]**. Habrá que validarlas en entrevistas.

### Las 5 sensaciones dominantes del Estado A (el problema)

1. **El nudo en el estómago al darle a «enviar».** Aparece justo antes del clic en el email importante. Intensidad media y cotidiana. **[HIP con anclaje F6, F2]**
2. **El calor en la cara y las orejas cuando alguien pregunta «¿esto lo has escrito tú?».** Llega en el momento del comentario. Intensidad alta y puntual. **[HIP con anclaje F1, E33 «embarrassing»]**
3. **La pesadez en los ojos y la frente de releer el mismo texto por cuarta vez.** Aparece al final del día, de noche. Intensidad media y acumulativa. **[HIP con anclaje F2, A1]**
4. **La sensación de «grima» (vergüenza ajena física, un escalofrío en la nuca) al leer lo que ChatGPT ha escrito en su nombre.** Aparece cuando lee la respuesta de la IA. Intensidad media. **[ANCL A27 «cringe», E27 «yuck»]**
5. **La mandíbula apretada y los hombros subidos mientras hace el ciclo de pestañas** (copiar, pegar, corregir, volver). Se da en plena tarea, al mediodía. Intensidad media-baja y sostenida. **[HIP con anclaje A21]**

### Las 5 sensaciones del Estado B (la solución)

1. **El clic de «enviar» sin respiración contenida**: soltar el aire con normalidad.
2. **La cara a temperatura normal** al leer la respuesta del cliente: contesta al contenido.
3. **Los ojos descansados**: una sola lectura y la pantalla cerrada antes.
4. **El reconocimiento cálido**, la sensación de «sí, este soy yo» al leer el texto de la IA.
5. **Los hombros que bajan**: una sola pestaña, una sola ventana, el trabajo fluye.

### 10 pares interoceptivos A → B con lenguaje para copy

| # | Estado A (cuerpo) | Estado B (cuerpo) | Lenguaje interoceptivo para copy | Razonamiento |
|---|---|---|---|---|
| 1 | Nudo en el estómago antes de enviar | Soltar el aire al pulsar «enviar» | «Ese nudo que se te hace justo antes de darle a enviar» → «Le das a enviar y sueltas el aire. Ya está.» | Es el momento de mayor ansiedad cotidiana (F6, casi a diario). Encaja con el cuadrante de ansiedad y baja energía. |
| 2 | Calor en la cara ante el «¿lo has escrito tú?» | Cara fresca al leer «perfecto, adelante» | «Ese calor que te sube a las orejas cuando el cliente pregunta…» → «…y esta vez contesta "perfecto, adelante".» | Es el pico de vergüenza del disparador situacional (F1). Úsese una sola vez en la carta, porque toca la herida. |
| 3 | Ojos pesados de releer a las once de la noche | Cerrar el portátil a las nueve y cinco | «Cuando los ojos ya te pican de leer el mismo email por cuarta vez» → «Lo lees una vez. Cierras el portátil.» | Es el contraste central temporal (las once de la noche frente a las nueve y cinco). Da imagen y sensación a la vez. |
| 4 | Grima o escalofrío al leer el «Espero que este mensaje…» | Reconocerse: «sí, así hablo yo» | «Ese escalofrío de vergüenza ajena, pero con tu firma debajo» → «Lo lees y te oyes a ti.» | Corpus: «cringe» (A27), «yuck» (E27). Activa al lector como juez de sí mismo. |
| 5 | Mandíbula apretada en el ciclo de pestañas | Hombros que bajan con una sola ventana | «Pestaña, copiar, pegar, corregir… con la mandíbula apretada» → «Una ventana. La tuya. Escribes y ya.» | A21: el ciclo de pestañas que rompe el ritmo. Al ser un gesto repetitivo, el cuerpo lo reconoce. |
| 6 | «Se me apaga el cerebro» al leer texto de IA (del juez) | El cliente «se engancha» y lee hasta el final | «Tu cliente lee la primera línea y se le apaga el cerebro: "otro de IA"» → «Lee la primera línea y sigue leyendo, porque eres tú.» | E48 (literal). Sirve para trasladar la sensación del juez al lector, que la conoce bien porque también la ha sentido. |
| 7 | Mirar el móvil a las siete de la mañana con el corazón acelerado («¿ha contestado?») | Despertarse sin abrir el correo primero | «Esa mirada al móvil antes de levantarte, a ver qué ha contestado» → «Te levantas, te haces el café y ya mirarás el correo.» | Prolonga la vigilancia nocturna (Un Día en la Vida, escena 1). Es una sensación de alerta temprana. |
| 8 | El estómago revuelto al ver un cargo desconocido en el banco (humanizadores) | La calma de «pago una vez y ya» | «Ese vuelco cuando ves en la cuenta un cargo que no reconoces» → «Un pago. Uno. Y nada más que cancelar.» | D25 y D14 (literales, BCT). Activa el recuerdo corporal del engaño para diferenciarse. |
| 9 | La tensión del pulgar suspendido sobre «enviar» (duda) | El pulgar que pulsa sin pararse | «Ese segundo con el dedo encima del botón, dudando» → «Pulsas sin pararte a pensarlo.» | Es una microescena física y cotidiana, sobre todo en el móvil. Muy visual para un anuncio en vídeo. **[HIP]** |
| 10 | La rabia sorda al ver «¡Claro! Aquí tienes…» por enésima vez | La sonrisa de complicidad («esto me pasaba a mí») al ver el email de IA de otro | «Esa rabia sorda cuando vuelve a salir el "¡Claro!" que le has dicho mil veces que quite» → «Ahora el que sonríe cuando le llega un email de robot eres tú.» | A19 (degradación) y el momento de superioridad de «Impacto de la transformación». Pasa de la impotencia al control. |

---

## Círculos Concéntricos de Preocupación (CCC)

### 1. Objetivo Principal (Primary Goal)

**«Usar la IA para escribir sin que se note»**, es decir, que lo que firma suene a él y le ahorre tiempo de verdad.
Ejemplos específicos:
- Mandar el email al cliente en cinco minutos y sin releerlo tres veces (F2).
- Que el jefe deje de comentar que «suena a ChatGPT» (A5).
- Atreverse a usar la IA para la propuesta importante. **[HIP]**
- Publicar un post en LinkedIn sin que nadie comente «esto es IA» (F4). **[ANCL]**
- Que el límite de uso diario no se le vaya corrigiendo el tono (A28).

**Puntos de referencia** (memes, frases o referencias que ya circulan):
- «Sent from my iPhone» → «Written by ChatGPT and I forgot to edit it» (E29).
- «AI slop» (C5, C9, C16, C22).
- «Usa la IA, pero que sea TU trabajo» (C27).
- «Que la IA escriba y luego lo reescribes con tus palabras» (E36).
- «Delve» y «tapestry» como memes de la IA (E1, E2; **anglosajones**).
- **[HIP en español]**: «Espero que este mensaje te encuentre bien» como meme de email de IA; «¡Claro! Aquí tienes…»; «En el vertiginoso mundo actual…».

### 2. Factores Críticos (Critical Factors)

Lo que el mercado considera esencial para lograrlo:
- **Saber qué delata a la IA** (conocimiento). **[ANCL C23, E38]**
- **Tener su IA «a su medida»** (configuración). **[ANCL E53]**
- **Saber explicar cómo escribe uno** (autoconocimiento de la propia voz). **[ANCL A22, E3]**
- **Mantener la configuración** en el tiempo (persistencia). **[ANCL A19]**
- **No depender de terceros** (autonomía). **[ANCL D-bloque]**
- **Confianza** para tocar los ajustes (autoeficacia). **[HIP con anclaje A36]**

**Puntos de referencia:**
- «Prompt engineering» (lenguaje insider; el recién llegado lo conoce de oídas). **[HIP]**
- «Instrucciones personalizadas» / «Custom Instructions» (nombre del menú). **[HIP del nombre en español]**
- «Dale contexto a la IA» (consejo omnipresente). **[HIP]**
- «Basura entra, basura sale» (*garbage in, garbage out*). **[HIP]**
- «Escribe como hablas» (consejo clásico de escritura). **[HIP]**

### 3. Factores de Campo (Field Factors)

Condiciones externas:
- **Saturación de texto de IA** en bandejas, redes y webs (C7, C22, A1: «everything sounds like AI now»).
- **Sospecha generalizada**: se acusa incluso a quien escribe a mano (bloque B, F1, F5). El listón de lo «humano» ha subido.
- **Presión corporativa para usar IA** (C14, C23, E15).
- **Políticas de «no IA»** en algunas empresas y con algunos clientes (E19).
- **Detectores poco fiables pero creídos** (B11, B18).
- **Industria de humanizadores** desacreditada (D-bloque).
- **Evolución constante de los modelos**: cambian la voz y cambian los tics (A34, D28, D29).
- **[HIP]**: la normativa de transparencia sobre IA en Europa (el AI Act) puede aumentar la sensibilidad a «ocultar» el uso de IA en ciertos contextos profesionales. No aparece en el corpus. Hay que investigarlo antes de usarlo.

**Puntos de referencia:**
- «La IA no va a quitarte el trabajo; te lo quitará alguien que use la IA.» **[HIP: frase muy difundida en el sector]**
- «Si es gratis, el producto eres tú.» **[HIP, aplicado a las herramientas de IA]**
- «People aren't stupid, they know when something feels off» (C23).
- «Managers who use AI to write emails seen as less sincere» (E16).

### 4. Consideraciones Contextuales (Contextual Considerations)

- **Brecha generacional**: los más jóvenes parecen manejar la IA con soltura; el veterano siente que va por detrás. **[HIP con anclaje A36, E46]**
- **Pudor**: no quiere que se sepa que necesita ayuda con algo «que todo el mundo usa». **[HIP]**
- **Relaciones comerciales largas** que dependen de la confianza personal (C11). **[ANCL]**
- **Ética del trabajo propio** («tiene que ser TU trabajo», C27).
- **Uso personal** en la familia y los amigos (C18, C19), con el riesgo de parecer frío. **[ANCL indirecto]**
- **[HIP cultural hispana]**: en España y Latinoamérica el trato personal en el email (el «un abrazo», el tuteo con el cliente, la broma) pesa mucho. Un email de IA con registro neutro-corporativo **chirría más** que en la cultura anglosajona del email.

**Puntos de referencia:**
- «A estas alturas…» (resistencia a aprender cosas nuevas). **[HIP]**
- «Esto es cosa de los jóvenes.» **[HIP]**
- «El trato es lo primero.» **[HIP]**
- «Más vale caer en gracia que ser gracioso» (aplicado a que el cliente «te lea bien»). **[HIP]**

### 5. Necesidades Humanas Fundamentales (Fundamental Human Needs)

- **Seguridad**: no ser descubierto, no ser estafado, no romper nada.
- **Autoestima / estima de los demás**: seguir siendo valorado y respetado.
- **Pertenencia**: ser de los que usan la IA bien, no de los que dan vergüenza.
- **Autonomía / control**: que la herramienta haga lo que él quiere.
- **Competencia**: sentirse capaz con la tecnología.
- **Autenticidad**: que lo que firma sea suyo.

**Puntos de referencia:**
- Pirámide de Maslow: **estima** (reconocimiento) y **seguridad**.
- Teoría de la autodeterminación: **autonomía, competencia y relación**. **[HIP como marco]**
- «Sé tú mismo.» «La autenticidad no se finge.» **[HIP]**
- «Más vale maña que fuerza» (la configuración inteligente frente a la reescritura bruta). **[HIP]**

---

## Dieta Informativa y Fuentes de Influencia

### 1. Los Héroes y Gurús

**[DATO INSUFICIENTE]**: el corpus no nombra figuras de autoridad seguidas por este mercado. Lo que sigue es **[HIP arquetípica]**:
- **El divulgador de IA «para todos»** (YouTube o Instagram en español): explica herramientas sin jerga, en vídeos cortos, con tono de «te lo enseño en un minuto». Le gusta porque **le hace sentir capaz**.
- **El creador de LinkedIn que habla de «sonar humano» y de marca personal** (F2, F4, F6, en inglés). Le gusta porque **habla de su problema profesional** con su lenguaje.
- **El comunicador o copywriter que critica la «escritura de IA»** con humor. Le gusta porque **pone palabras** a lo que él nota.
- **El periodista o escritor «de toda la vida»** que defiende la escritura humana (F5). Le gusta por la **autoridad del oficio**.
- **El compañero de trabajo o el hijo que «sabe de esto»**: es el gurú doméstico. Le gusta porque **es de confianza**.

**Investigación necesaria:** listar los cinco divulgadores de IA en español con más audiencia de 35-60 años (por demografía de seguidores en YouTube, Instagram y LinkedIn) y mirar en sus comentarios qué preguntan sobre «que suene natural».

### 2. Los «Campos de Batalla» Digitales

- **En el corpus (anglosajón):** Reddit (r/ChatGPT, r/ClaudeAI, r/claude, r/OpenAI, r/WritingWithAI, r/copywriting, r/managers, r/antiwork, r/mildlyinfuriating, r/smallbusiness, r/AITAH), Trustpilot y LinkedIn.
- **Para el target hispano [HIP]:** grupos de Facebook («ChatGPT en español», «IA para negocios»), comentarios de YouTube, LinkedIn en español, Instagram (reels de trucos de IA), grupos de WhatsApp o Telegram de su sector y, en menor medida, foros generalistas (Forocoches en España, menos para el target femenino de más edad).
- **Contenido que consume vorazmente [HIP]:** **reels y shorts** con un truco de IA, **carruseles de LinkedIn** («10 frases que delatan a ChatGPT»), **tutoriales paso a paso de 5-10 minutos** y **newsletters** de productividad. **No** consume podcasts largos ni papers.

### 3. Jerga Tribal (Insider Language)

> Atención: el target recién llegado **no** usa la mayoría de estas palabras. Sirven para **entender** el mercado y para que el PDF tenga autoridad, pero en el copy de entrada deben **traducirse** a lenguaje llano.

1. **Prompt** («el prompt», «hacer buenos prompts»).
2. **Instrucciones personalizadas** / *Custom Instructions*.
3. **Proyectos** (en ChatGPT y en Claude).
4. **Humanizador** / *humanizer*.
5. **Detector** (GPTZero, Turnitin, ZeroGPT, Pangram).
6. ***Slop*** / *AI slop*.
7. ***Tells*** (las «señales» o «huellas» que delatan a la IA).
8. ***Em dash*** (la raya larga).
9. ***Delve*** / ***tapestry*** (palabras meme).
10. **Límite de uso** / **tokens** / **contexto** («se le olvida porque se acaba el contexto»).
11. **Plantilla** / *rulebook*.
12. **Alucinación** (E50).

### 4. Creencias de Autoridad

**«Verdad aceptada» que hay que desafiar:** **«Para que la IA escriba bien, tienes que aprender a hacer buenos prompts.»**
La nueva oportunidad: **«No necesitas aprender a hablarle a la IA. Necesitas que la IA aprenda a hablar como tú, y eso se le enseña una vez.»** La responsabilidad pasa del usuario (que tiene que convertirse en experto) a la configuración (que se hace una vez).

Segunda verdad aceptada que hay que desafiar: **«Lo que delata a la IA son ciertas palabras.»** La nueva oportunidad: **«Las palabras son solo una de las cuatro huellas. Las otras tres (cómo se construyen las frases, el tono de asistente educado y el ritmo en el que todo mide lo mismo) son las que de verdad se notan.»** Base: E38, A29, A33, E9.

---

## MAPA DE TRIGGERS PSICOLÓGICOS — AUDITORÍA DE MOTIVADORES

> Reutilizo las objeciones del bloque OBJECIONES (más abajo), los bloqueos de las Restricciones, la Escala de Credibilidad y los Disparadores de Expulsión (bloque Gatillos de Abandono). No los regenero: los referencio.

| # | Trigger | Relevancia | Manifestación (voz del buyer) | Palanca (qué lo activa) | Micro-ángulo (1 línea) | Riesgo (anti-ejection) |
|---|---|---|---|---|---|---|
| 1 | Consistency | **Alta** | «Yo siempre he dicho que la IA hay que usarla con cabeza, revisando.» | Recordarle su propia norma («usar la IA está bien; que se note, no») y alinear la compra con ella | «Si ya revisas lo que escribe la IA, el siguiente paso lógico es que no tengas que revisarlo tanto.» | No acusarle de haber sido «de los que copian y pegan» (Gatillo 6) |
| 2 | Product Nature | **Alta** | «¿Esto es otra web? ¿Un curso? ¿Se instala?» | Explicar pronto qué es: «una guía y una configuración dentro de tu ChatGPT» | «No es otra herramienta. Es tu ChatGPT, ajustado a ti.» | No decir «plugin» ni «skill» sin contexto en el primer pantallazo (Gatillo 2) |
| 3 | Prospect Nature | **Alta** | «Esto será para gente que sabe de tecnología.» | Hablarle como a un no técnico desde la primera línea | «Para gente que usa ChatGPT como usa el WhatsApp.» | No infantilizar ni mencionar la edad (Gatillo 8) |
| 4 | Objection Raising | **Alta** | «Ya, ya, eso me dijeron los de la web de humanizar.» | Plantear la objeción antes que él (Objeciones 1, 6, 11) | «Seguro que estás pensando: "otro que me promete que no se notará".» | No plantear objeciones que no tiene (por ejemplo, de detectores académicos) |
| 5 | Objection Resolution | **Alta** | «Si me explicas por qué esto es distinto, te escucho.» | Disolución con fórmulas (Restricciones 6, 7, 9) | «Lo que probaste falló por tres motivos. Esto ataca los tres.» | No ridiculizar lo que probó (Gatillo 5) |
| 6 | Involvement and Ownership | **Alta** | «Si lo configuro yo, es mío.» | Hacerle imaginar su configuración: «tu forma de saludar, tus palabras» | «Escribe tres frases como las dirías tú. Eso ya es el principio de tu configuración.» | No prometer que «lo hace todo solo» (resta propiedad) |
| 7 | Integrity | **Alta** | «Que me digan la verdad: qué hace y qué no.» | Declarar los límites (no es indetectable; requisitos de plan) | «No te prometo que nadie vaya a notarlo nunca. Te prometo que va a sonar a ti.» | No usar «100 % humano» (Gatillo 1) |
| 8 | Storytelling | **Alta** | «Cuéntame de alguien a quien le pasó lo mismo.» | La micro-historia del email de las once de la noche y la pregunta del cliente | «Era martes, eran las once, y el email seguía sonando a robot…» | No inventar testimonios (no hay prueba propia todavía) |
| 9 | Authority | **Media** | «¿Quién eres tú para enseñarme esto?» | Autoridad **de oficio** (alguien que escribe bien y lo demuestra en la propia página) | «La prueba de que funciona es que estás leyendo esto.» | No inflar credenciales ni usar «experto en IA» (suena a gurú, Gatillo 4) |
| 10 | Proof of Value | **Alta** | «Enséñame el antes y el después.» | Demostración comparativa del mismo email | «El mismo email, dos versiones. Tú decides cuál mandarías.» | No usar porcentajes de detectores como prueba (Gatillo 3) |
| 11 | Emotion | **Alta** | «Lo que no quiero es volver a sentir eso cuando me preguntan si lo escribí yo.» | Escena del calor en la cara (Interoceptivo 2) | «Ese calor en las orejas cuando el cliente pregunta…» | No revivir la humillación con detalle morboso (Herida) |
| 12 | Justify with Logic | **Media** | «Si me ahorra media hora al día, se paga solo.» | Coste de la inacción por unidad de tiempo (Lógica Transaccional) | «Media hora por email, cuatro al día. Haz la cuenta.» | No abrir con números, solo justificar después |
| 13 | Greed | **Baja** | «¿Me hará ganar más clientes?» | Beneficio indirecto (no perder clientes, E19) | «Que tu cliente no te pida descuento por sospechar.» | No prometer más ventas ni conversiones (Escala nivel 9) |
| 14 | Credibility | **Alta** | «¿Por qué me voy a fiar de ti si todos mienten?» | Honestidad, garantía en dinero, pago único y la página humana | «Pago único. Si no te convence, te devuelvo el dinero, no créditos.» | No usar pruebas inexistentes |
| 15 | Satisfaction Conviction | **Alta** | «¿Y si no me sirve?» | Garantía sin preguntas, reversibilidad | «Si no te gusta, borras dos párrafos y tu ChatGPT vuelve a ser el de antes.» | No poner condiciones a la devolución |
| 16 | Linking | **Alta** | «Es como cuando…» | Metáfora del empleado nuevo o del asiento del coche | «Es como un empleado nuevo al que nadie le dijo cómo hablas con tus clientes.» | No usar metáforas técnicas (programación, código) |
| 17 | Desire to Belong | **Media** | «Quiero ser de los que la usan bien.» | Norma del grupo: «usar la IA está bien; que se note, no» | «Únete a los que usan la IA y no se les nota.» | No crear «comunidad» visible que exponga al comprador (estigma) |
| 18 | Desire to Collect | **Baja** | «¿Trae más cosas?» | Configuraciones por tipo de texto (email, LinkedIn, WhatsApp), si existen | «Una voz, varios tonos: para el cliente, para el jefe, para LinkedIn.» | No inflar bonus ni hacer de «pack» (suena a gurú) |
| 19 | Sense of Urgency | **Baja-Media** | «Lo miraré cuando tenga tiempo.» | Urgencia **natural**: el próximo email importante | «El próximo email que escribas va a sonar igual. A menos que…» | **Nunca** cuentas atrás ni escasez artificial (Gatillo 7) |
| 20 | Exclusivity | **Baja** | — | No aplica bien: el mercado quiere seguridad, no exclusividad | (Si acaso) «Lo que casi nadie sabe que su ChatGPT puede hacer.» | No hacer «solo para elegidos» |
| 21 | Simplicity | **Alta** | «Dímelo fácil.» | Pasos numerados, capturas, «una tarde» | «Una tarde. Una vez. En tu ChatGPT.» | No simplificar hasta la falsedad («en 2 minutos y para siempre») |
| 22 | Guilt | **Baja** | «Ya sé que debería haberlo arreglado antes…» | Quitar culpa, no ponerla | «No es culpa tuya: viene así de fábrica.» | No culpabilizar («llevas meses mandando emails de robot») |
| 23 | Specificity | **Alta** | «¿Qué es lo que se nota exactamente?» | Las cuatro huellas nombradas, ejemplos concretos y cifras de tiempo | «Cuatro huellas. Esta es la primera: todas tus frases miden lo mismo.» | No dar listas eternas de palabras (insider) |
| 24 | Familiarity | **Alta** | «Si es en mi ChatGPT, lo conozco.» | Capturas de la interfaz que ya usa, en español | «La misma pantalla de siempre. Un menú que ya tienes.» | No enseñar interfaces desconocidas (terminal, API) |
| 25 | Patterning | **Media** | «¿Cómo lo hacen los que lo hacen bien?» | Mostrar el patrón: la IA bien configurada frente a la IA por defecto | «Los que no se les nota no tienen un truco. Tienen la IA configurada.» | No basarse en «lo que hacen los expertos» (excluye al no técnico) |
| 26 | Hope | **Alta** | «Ojalá hubiera una forma de que dejara de pasarme.» | La promesa de nivel 6-7 de la Escala | «Le pides el email, lo lees una vez y lo envías.» | No prometer el nivel 8 («nadie lo notará jamás») |
| 27 | Curiosity | **Alta** | «¿Por qué pasa eso?» | La paradoja de E12 y las cuatro huellas | «Si le pides que no suene a IA, suena más a IA. Te explico por qué.» | No hacer clickbait vacío |
| 28 | Harmonize | **Alta** | «Sí, eso es verdad… y eso también…» | Cadena de síes: reconocimiento de síntomas | «¿Relees tres veces antes de enviar? ¿Le has pedido "más natural"? ¿Has sentido grima al leerlo?» | No hacer preguntas que no se apliquen al target (académicas) |
| 29 | Mental Engagement | **Alta** | «A ver si lo veo…» | Ejercicio: «encuentra las cuatro huellas en este email» | «Mira este email. ¿Ves lo que tienen en común las tres primeras frases?» | No hacerlo difícil ni técnico |
| 30 | Honesty | **Alta** | «Por fin alguien que no me vende humo.» | Admitir límites y decir lo que no es | «No te voy a decir que es indetectable. Te voy a decir que suena a ti.» | No mezclar honestidad con exageración en la misma página |

### A) TOP 10 triggers en este mercado

1. **Proof of Value (10):** el mercado ya no se cree claims, solo lo que ve con sus ojos. El antes y después del mismo email es la prueba reina.
2. **Credibility (14):** sale de una categoría desacreditada, así que sin credibilidad nada más funciona.
3. **Simplicity (21):** es la palanca crítica (ansiedad del no técnico). Si no parece simple, no hay compra.
4. **Specificity (23):** las cuatro huellas convierten el «algo chirría» en algo concreto y controlable.
5. **Curiosity (27):** la paradoja de E12 rompe la predicción del lector.
6. **Integrity / Honesty (7, 30):** el mercado premia a quien admite límites, frente al «100 % humano» desacreditado.
7. **Satisfaction Conviction (15):** la garantía en dinero y la reversibilidad bajan la ansiedad dominante.
8. **Familiarity (24):** «en tu ChatGPT, la pantalla de siempre» supera el filtro de preselección.
9. **Objection Raising (4):** anticipar el «otro humanizador más» desactiva el sesgo de disponibilidad.
10. **Involvement and Ownership (6):** el «es tuyo» encaja con la tarea vital de control y con el diferencial frente a la suscripción.

### B) 3 combos de triggers

**Combo 1 — «La paradoja que se puede ver»: Curiosity + Specificity + Proof of Value**
→ Estructura de **lead de Secreto**. Se abre con la paradoja («pedirle que no suene a IA lo empeora»), se explica la causa con las cuatro huellas nombradas y se demuestra con el mismo email antes y después. Es la estructura de la parte educativa (PDF y landing) y del anuncio en formato «mira esto».

**Combo 2 — «Seguro, sencillo, tuyo»: Simplicity + Familiarity + Satisfaction Conviction + Ownership**
→ Estructura del **giro de seguridad y la oferta**: «se hace en tu ChatGPT, en una tarde, paso a paso, y si no te gusta lo borras y te devuelvo el dinero». Es la estructura del bloque central de la carta (justo después del mecanismo) y de los emails de objeciones.

**Combo 3 — «Por fin alguien honesto»: Honesty + Objection Raising + Credibility + Storytelling**
→ Estructura de **carta de tono confesional y anti-industria**: «Seguro que has visto las webs que prometen 100 % humano. Yo también. Esto es lo que encontré en sus reseñas… Por eso hice algo distinto, y te digo también lo que NO hace». Es la estructura para el segmento quemado por los humanizadores y para el retargeting.

---

## Eventos Disparadores y Timeline de Compra

### 1. Los 10 eventos disparadores más probables, por frecuencia e impacto

| # | Evento | Categoría | Frecuencia | Impacto | Base |
|---|---|---|---|---|---|
| 1 | El cliente o el jefe dice o pregunta «¿esto lo ha escrito ChatGPT?» / «suena a ChatGPT» | Comparación / comentario hiriente | Media | **Muy alto** | F1, F7, A5, C27 |
| 2 | La enésima reescritura del mismo texto (el «hasta aquí» del propio emisor) | Vida laboral cotidiana | **Alta** | Medio | F2, F3, A27, A28 |
| 3 | Mandar sin querer la frase meta del asistente | Vergüenza pública | Baja | **Muy alto** | B22, E33 |
| 4 | Un texto de alto riesgo inminente (propuesta grande, candidatura, presentación ante dirección, reclamación importante) | Vida laboral / fecha límite | Media | Alto | **[HIP]** |
| 5 | La empresa impone usar IA para todo | Vida laboral / cambio de normas | Media (creciente) | Alto | C14, C23, E15 |
| 6 | Recibir el email de IA de otro y verse reflejado | Comparación | **Alta** | Medio | Bloque C + **[HIP del giro]** |
| 7 | Un cargo inesperado o un fracaso con un humanizador (pasa a buscar alternativa) | Experiencia negativa | Baja-media | Alto | D8, D14, D25 |
| 8 | Ver a otro (compañero, proveedor) usar la IA «sin que se note» | Comparación / envidia | Media | Medio | E35 + **[HIP]** |
| 9 | Cambio de trabajo o de rol que exige escribir más (nuevo puesto, hacerse autónomo, empezar en LinkedIn) | Evento de vida | Baja | Alto | **[HIP]** |
| 10 | Vuelta de vacaciones / inicio de trimestre / Año Nuevo («este año me pongo con esto») | Calendario | Estacional | Medio | **[HIP]** |

### 2. Ciclo de decisión

- **Tiempo entre reconocer el problema y comprar:** **largo en la fase latente** (meses de reescritura silenciosa) y **corto tras un evento disparador** (de horas a días). **[HIP con anclaje en la naturaleza crónica de A1, F6 frente a la reacción a un incidente de F1]**
- **Tipo de compra:** a 29 € y con pago único, **semi-impulsiva**: se decide en minutos u horas **si** se supera el filtro de confianza. No es deliberada como un curso de 300 €. **[HIP basada en mercados similares]**
- **¿Investiga mucho antes de comprar?** Lo justo para descartar estafa: busca «nombre + opiniones / estafa». No compara diez opciones. La desconfianza hacia la categoría hace que **investigue la honestidad, no las funcionalidades**. **[ANCL D3-D6: «is it legit?»]**

### 3. Estacionalidad

**[DATO INSUFICIENTE]**: el corpus no tiene fechas por cita. **Hipótesis basada en mercados similares (productividad y formación para profesionales):**
- **Picos:** **septiembre** (vuelta al trabajo, «este curso me organizo»), **enero** (propósitos), **inicio de trimestre** (abril, octubre) y las semanas posteriores a **anuncios de nuevas versiones de ChatGPT** (vuelve el tema a la conversación pública).
- **Valles:** **agosto** y **la segunda quincena de diciembre** (menos trabajo escrito, menos fricción); **Semana Santa** en España.
- **Contraestacional:** el **cierre de trimestre o de año** (alta carga de trabajo) reduce la disponibilidad para configurar, pero aumenta el dolor.

### 4. Ventana de oportunidad

- **Duración de la urgencia tras el evento:** **de 24 a 72 horas** en el caso del comentario hiriente (la vergüenza se enfría rápido y vuelve el «tampoco es para tanto»). **Una o dos semanas** si hay un texto de alto riesgo en el horizonte. **[HIP]**
- **Qué pasa si no actúa en esa ventana:** vuelve al statu quo (reescribir a mano y revisar tres veces), **con un nivel de vigilancia algo más alto**. El problema se cronifica y sube un escalón de ansiedad. Si en ese intervalo encuentra un humanizador, puede caer en él, decepcionarse y aumentar su desconfianza hacia toda la categoría. **[ANCL D-bloque]**

### Implicaciones para el copy

- **Eventos que hay que mencionar para activar la urgencia:** el n.º 1 (la pregunta del cliente o del jefe), el n.º 2 (la cuarta reescritura) y el n.º 4 (el próximo email importante). El n.º 3 (la frase meta) funciona como **humor reconocible**, no como amenaza.
- **Momentos del año para intensificar la publicidad:** septiembre, enero y las semanas siguientes a cada lanzamiento de un modelo nuevo de IA. **[HIP]**
- **¿Urgencia artificial o natural?** **Natural**, sin duda. La urgencia artificial es un disparador de expulsión para el cuadrante de ansiedad. La urgencia natural es suficiente y más creíble: **«tu próximo email va a sonar igual que el anterior»**. Si se quiere un incentivo temporal, que sea honesto (por ejemplo, un precio de lanzamiento real, si existe) y comunicado sin presión.

---

## Arquetipos y Subsegmentos

| Arquetipo | Motivador principal | Objeción principal | Ángulo clave |
|---|---|---|---|
| **«La que firma con su nombre»** (núcleo) | Que no se note ante el cliente o el jefe | «Yo no soy técnica» | «Tu ChatGPT, ajustado a ti, en una tarde.» |
| **«El quemado por los humanizadores»** | No volver a tirar dinero; encontrar algo que por fin funcione | «Todo esto es una estafa» | «No es otro humanizador. Es lo contrario.» |
| **«El veterano desbordado»** | No quedarse atrás; demostrarse que todavía puede | «A mi edad ya no me pongo con esto» | «No tienes que aprender la IA. La IA tiene que aprender de ti.» |
| **«El que ya probó las instrucciones»** (semi-técnico) | Entender por qué no le funcionó y arreglarlo de verdad | «Ya lo intenté y no funcionó» | «Lo que probaste falló por tres motivos. Esto ataca los tres.» |

### Detalle por arquetipo

**1. «La que firma con su nombre»** (núcleo, ≈ 50-55 % del segmento principal **[HIP]**)
- **Perfil diferencial:** 38-55 años, empleada de oficina, comercial, administrativa, gestora o autónoma de servicios. Usa ChatGPT a diario para emails y mensajes. No ha tocado nunca los ajustes.
- **Motivador:** que el cliente o el jefe no note la IA; dejar de reescribir.
- **Objeción:** «No sé si voy a saber hacerlo.»
- **Disparador:** un comentario del cliente o del jefe; la cuarta reescritura.
- **Mensaje que resonaría:** «A nadie le molesta que uses ChatGPT. Le molesta que se note. Y se arregla una vez, en tu propio ChatGPT, sin saber nada técnico.»
- **Mensaje que le alejaría:** «Domina la IA como un profesional», «prompt engineering», «automatiza tu escritura con agentes».

**2. «El quemado por los humanizadores»** (≈ 15-20 % **[HIP]**; con mucha base en el corpus: D-bloque)
- **Perfil diferencial:** cualquier edad, ha pagado por Undetectable, StealthGPT u otra herramienta similar, o ha leído las reseñas. Puede ser autónomo o profesional de contenidos.
- **Motivador:** encontrar algo que funcione y que no le estafe.
- **Objeción:** «Todo lo que se vende para esto es una estafa.»
- **Disparador:** el último fracaso o cargo inesperado.
- **Mensaje que resonaría:** «Si alguna vez te cobraron el año entero cuando decía "al mes", esto es para ti: se paga una vez, funciona dentro de tu propia IA y no vuelves a depender de nadie.»
- **Mensaje que le alejaría:** cualquier porcentaje de «humano», la palabra «humanizar», las pruebas gratuitas con tarjeta y «modelo avanzado».

**3. «El veterano desbordado»** (≈ 15 % **[HIP]**; base residual: A36, E46)
- **Perfil diferencial:** 52-62 años. Usa ChatGPT porque «hay que usarlo», con cierta inseguridad. Puede que lo use más en el móvil que en el ordenador.
- **Motivador:** no quedarse atrás; sentirse capaz; no hacer el ridículo.
- **Objeción:** «Esto es para gente joven / que sabe.»
- **Disparador:** ver que otros (más jóvenes) lo hacen sin que se note; el comentario del jefe.
- **Mensaje que resonaría:** «Si sabes escribir un email, sabes hacer esto. Te lo enseño paso a paso, con capturas, en tu pantalla de siempre.»
- **Mensaje que le alejaría:** cualquier referencia explícita a la edad («aunque seas mayor»), la jerga, la velocidad («en 2 minutos») y los vídeos con montaje frenético.

**4. «El que ya probó las instrucciones»** (≈ 10-15 % **[HIP]**; base: A19, A26, A27, A29)
- **Perfil diferencial:** 30-50 años, semi-técnico. Sabe que existen las Instrucciones personalizadas, ha copiado alguna plantilla y le ha fallado.
- **Motivador:** entender **por qué** falló y tener algo que funcione de verdad.
- **Objeción:** «Esto ya lo hice y no sirve.»
- **Disparador:** la degradación (vuelven los tics) o un texto importante que le sale mal.
- **Mensaje que resonaría:** «Las instrucciones normales fallan porque dicen lo que no hacer, son de otro y se olvidan a mitad de conversación. Esta configuración está hecha con tu voz y resiste.»
- **Mensaje que le alejaría:** la simplificación excesiva («es solo pegar un texto») o no reconocer que ya lo ha intentado.

**Arquetipo excluido (ver Segmentación y Anti-Persona):** «El que tiene que pasar el detector» (estudiante o candidato). Tiene otro motivador, otro juez, otro criterio de éxito y otro riesgo ético.

---

## Anti-Persona (el cliente a rechazar)

### 1. Perfil del Anti-Persona

- **El evasor de detectores académicos:** el estudiante que busca entregar como propio un trabajo de IA y que no lo marque Turnitin. Su criterio de éxito es **un porcentaje** en un detector, no un lector humano (B-bloque, D28, D29, D32, D36).
- **El que busca la caja mágica:** quiere pegar un texto y que salga «humano» sin hacer nada.
- **El que quiere «clonar» a otro:** quiere que la IA escriba como su jefe, un autor o un competidor para hacerse pasar por él. **[ANCL E18 como caso límite]**
- **El experto que quiere un juguete:** el usuario avanzado que construye sus propias configuraciones y busca algo que ya sabe hacer. Comprará, encontrará «nada nuevo» y lo dirá.
- **El productor de contenido masivo:** quiere generar 70 artículos al mes (E44) o cientos de cold emails sin que se detecten. Busca volumen, no voz.

**Mentalidad:** **atajo y garantía**. Quieren certeza absoluta de resultado sin implicarse y miden el éxito con una métrica externa (detector, volumen) en lugar de con la lectura de una persona.

### 2. Señales de alerta

- Frases: «¿Pasa Turnitin?», «¿Garantizas 0 % IA en GPTZero?», «¿Sirve para la tesis?», «Necesito que no se detecte», «¿Puedo generar 100 artículos al día?», «¿Me lo hace todo sin que yo tenga que escribir nada?».
- Comportamientos: preguntar por porcentajes, comparar con humanizadores **por precio**, pedir pruebas en detectores, querer usarlo para textos ajenos.
- **Lo que esperan y no podemos o no queremos dar:** garantía de indetectabilidad algorítmica; ayuda para hacer pasar trabajos académicos como propios; volumen industrial; resultados sin aportar nada de sí mismos.

### 3. Por qué son problemáticos

- **Devoluciones y malas reseñas:** el detector puede marcar igualmente cualquier texto (B18: 0 %, 40 % y 100 % para el mismo texto), así que el evasor **siempre** tendrá un «fallo» que reclamar.
- **Riesgo reputacional y ético:** asociar el producto a hacer trampas académicas lo pone en la categoría de los humanizadores.
- **No obtendrán resultados** porque el producto requiere **la voz del usuario**: sin implicación, no hay voz que configurar.
- **Ruido en el posicionamiento:** si el copy les atrae, se diluye el mensaje para el comprador principal (que es honrado y quiere sonar a sí mismo).

### 4. Ejemplos concretos (5 tipos que NO queremos)

1. **«El que quiere pasar Turnitin»**: «Solo necesito que el ensayo salga humano en el detector.»
2. **«El que busca el botón mágico»**: «¿No hay algo que pegue el texto y ya?»
3. **«El que no quiere poner nada de sí mismo»**: «Yo no tengo tiempo de explicarle cómo hablo; que lo adivine.»
4. **«El fabricante de contenido al peso»**: «Necesito 200 posts al mes que no parezcan de IA.»
5. **«El experto escéptico profesional»**: «Esto me lo hago yo en diez minutos con un system prompt.»
6. (Extra) **«El suplantador»**: «Quiero que escriba como mi jefe / como tal autor, para que parezca suyo.»

### 5. Filtros en el copy

**Frases para que se autoexcluyan:**
- «Esto **no** es para engañar a un detector. Si lo que necesitas es que un trabajo pase Turnitin, este producto no es para ti.»
- «Esto **no** es una caja donde pegas un texto y sale otro. Es enseñarle a tu IA cómo hablas tú, y para eso hace falta que tú pongas tu forma de hablar.»
- «No te prometo que ningún detector lo vaya a marcar. Los detectores dan lo que les da la gana. Te prometo que va a sonar a ti cuando lo lea una persona.»
- «Si ya configuras tu IA con system prompts y sabes lo que es un token, probablemente esto te quede corto. Está hecho para quien usa ChatGPT en modo chat y no quiere complicarse.»

**Requisitos o compromisos que los ahuyentan:**
- «Necesitas una tarde (unos 60-90 minutos) y tres o cuatro textos tuyos.» **[HIP de producto: verificar la duración real]**
- «Funciona con tu voz. Si no quieres poner tu voz, no funciona.»

---

## Gatillos de Abandono (Disparadores de Expulsión)

1. **«100 % humano» / «indetectable» / «pasa todos los detectores».** El lector lo asocia al instante con los humanizadores-estafa (D12, D18, D31). Para el adulto honrado, además, suena a trampa. Expulsión inmediata por desconfianza y por choque de valores.

2. **Jerga técnica en la entrada: «plugin», «skill», «API», «system prompt», «tokens», «Claude Code», «instalar».** Confirma el «esto no es para mí» (A36). El lector se ve a sí mismo fracasando antes de empezar. **Atención: «plugin» y «skill» forman parte del formato real del producto**, así que hay que presentarlos tarde, explicados y con capturas.

3. **Porcentajes de detectores como prueba («0 % IA en GPTZero»).** El mercado sabe que los detectores se contradicen (B18, B20). Usarlos como prueba demuestra que el vendedor juega al juego equivocado y le coloca en la categoría de los humanizadores.

4. **El tono de gurú de la IA (euforia, mayúsculas, emojis, «revoluciona», «domina la IA»).** Es la contaminación de predicción por excelencia («otro vendedor de prompts»). En el cuadrante de ansiedad, la euforia suena a falsedad.

5. **Ridiculizar a quien copia y pega sin editar.** El lector **ha sido** esa persona (E33, B22). Burlarse de «los que se les nota» le hace sentir señalado, no cómplice. El humor sobre la frase meta solo funciona si es **autoinclusivo** («a todos nos ha pasado»).

6. **Insinuar que usar IA es hacer trampa / que está engañando a sus clientes.** Choca con su autoimagen de persona honrada que usa una herramienta (E34, C27). Si el copy moraliza («deberías escribir tú»), le expulsa al bando antiIA, que no es el suyo.

7. **Urgencia artificial (cuentas atrás, «solo hoy», «últimas plazas»).** Activa el recuerdo de las webs con trampas de facturación (D14: «It said cancel anytime…») y dispara la ansiedad, que es justo la fuerza que hay que bajar.

8. **Referencias explícitas a la edad («aunque tengas 50 años», «para los que no son nativos digitales»).** Incluso dirigidas al veterano, le etiquetan y le humillan. La edad debe estar implícita en el tono (calma, claridad), nunca nombrada.

9. **Una landing o un anuncio que suene a IA.** Es la contradicción fatal: el lector es juez experto y se le «apaga el cerebro» (E48) en la primera línea. Basta un «En el vertiginoso mundo actual», un «¡Descubre cómo…!» o tres beneficios con viñetas simétricas para que abandone y además se ría.

10. **Prometer que «escribirá exactamente como tú» o que «clona tu voz».** El mercado ha probado los clonadores (A30) y sabe que no es cierto. Al cruzar el límite de credibilidad (nivel 8+), invalida también las promesas razonables que vienen después.

---

## OBJECIONES

> **Público objetivo:** profesionales no técnicos de 35 a 60 años que usan ChatGPT o Claude en modo chat para escribir emails, mensajes y textos de trabajo, y que **quieren que lo que escriben con IA suene a ellos y no se note la máquina**.
> **Ejercicio:** 15 razones por las que no creen poder conseguirlo con **una guía en PDF más una configuración guiada (skill/plugin) para su propia IA**, y por tanto no lo comprarían.
> **Procedencia:** las citas escépticas son **[HIP]** construidas en primera persona, cada una anclada en entradas concretas del corpus (se indican). La popularidad (1-10) se estima a partir de la frecuencia de cada patrón en el corpus y de su peso en el segmento principal.

### A. OBJECIONES INTERNAS

#### I-1. «No soy técnico: no voy a saber hacerlo» — Popularidad: 9/10
*Anclaje: A35, A36, E46, A21; criterio eliminatorio n.º 2; sesgo de autoeficacia baja.*

**Cita escéptica:**
«Mira, yo uso ChatGPT como uso el WhatsApp: escribo, me contesta, copio y pego. Ya está. No he tocado un ajuste en mi vida y, cuando veo la palabra "plugin", me imagino algo que se instala y que a la semana me está pidiendo actualizaciones. Mi hijo me dice que es muy fácil, pero a mi hijo todo le parece muy fácil. La última vez que intenté seguir un tutorial de esos, el chico iba a toda velocidad, su pantalla no se parecía a la mía y al minuto tres yo ya estaba perdido. Me da miedo ponerme a tocar cosas un martes por la noche y que el miércoles, cuando tenga que mandar los presupuestos, no me funcione nada. Prefiero seguir como estoy, que por lo menos sé hacerlo. Esto será para la gente que sabe de estas cosas, no para mí. Y no me apetece sentirme torpe otra vez delante de una pantalla.»

**Validación (≈ 50 palabras):** Es completamente lógico. Has visto cómo cada herramienta nueva viene con un manual más gordo y tutoriales a toda prisa en pantallas que no son la tuya. Sentirse torpe delante de un ordenador desgasta, y nadie quiere arriesgar la herramienta con la que trabaja cada día por un experimento.

**Contraargumento 1 (reformulación como ventaja, ≈ 150 palabras):** Pero fíjate en una cosa: lo difícil de que tu IA suene a ti **no es técnico**. Es saber cómo hablas tú: cómo saludas a un cliente, qué palabras no usarías nunca, si escribes corto o largo. Y eso lo sabes tú mejor que cualquier ingeniero. El usuario técnico que se monta configuraciones complicadas suele hacer listas de «prohibido decir esto», y por eso en los foros se queja de que su IA sigue sin sonar a él. Tú partes de otro sitio: no vas a intentar programar a la máquina, vas a **describirte**. Quien no sabe de tecnología no tiene la tentación de complicarlo. La guía está pensada exactamente para ti: la pantalla de ChatGPT que ya conoces, en español, con capturas, un paso cada vez. Si sabes copiar, pegar y escribir un email, tienes todo lo que hace falta. Lo técnico ya está resuelto. Lo que falta es lo tuyo.

**Contraargumento 2 (celebración, ≈ 150 palabras):** Hay algo que dice mucho de ti en esa prudencia. No te lanzas a instalar cualquier cosa, no te crees al primero que te dice «es facilísimo» y proteges la herramienta con la que trabajas. Eso no es torpeza: es criterio. Es el mismo criterio que hace que tus clientes se fíen de ti. Y es justo el que hace falta aquí, porque esta configuración funciona mejor en manos de alguien que se toma el tiempo de pensar cómo escribe que en las de alguien que pega una plantilla de internet sin mirarla. Tú vas a ir despacio, vas a comprobar cada paso y vas a ver el cambio en tu propio email antes de seguir. Además, si algo no te convence, borrarlo es tan sencillo como borrar un párrafo, y tu ChatGPT vuelve a estar como antes. La gente prudente es la que mejor resultado saca de esto.

#### I-2. «Para lo que tardo en arreglarlo, lo escribo yo» — Popularidad: 7/10
*Anclaje: E22, A31, A30, F2.*

**Cita escéptica:**
«Lo he pensado mil veces. Para cuando consigo explicarle a la máquina lo que quiero, cómo lo quiero y en qué tono, ya lo habría escrito yo. Me pasó la semana pasada: un correo para un proveedor, cosa de cinco líneas. Entre que se lo pedí, me lo devolvió con un "Espero que este mensaje le encuentre bien", se lo corregí, me lo volvió a poner y lo acabé rehaciendo a mano, se me fueron veinte minutos. Veinte minutos para cinco líneas. Así que ahora, para lo importante, lo escribo yo y punto, y la IA la dejo para cosas tontas. Si encima ahora tengo que dedicar una tarde entera a configurarla, eso es todavía más tiempo. No me salen las cuentas. Prefiero lo malo conocido.»

**Validación:** Tienes toda la razón en la cuenta que haces. Si cada texto te obliga a explicarle todo desde cero y luego a corregirlo, la IA no te ahorra tiempo: te lo quita. Mucha gente ha llegado a la misma conclusión que tú y ha dejado la IA para lo que no importa.

**Contraargumento 1:** Precisamente porque has hecho esa cuenta, eres de las pocas personas que ven el problema de verdad. La mayoría sigue usando la IA «como viene», pierde esos veinte minutos cada vez y ni se da cuenta. Tú has detectado que el coste está en **explicárselo cada vez**. Y esa es exactamente la parte que desaparece: si se lo explicas una sola vez, bien explicado, deja de haber «cada vez». Es la diferencia entre darle las indicaciones a un taxista en cada trayecto o tener tu propio coche con el GPS ya programado. Una tarde de configuración frente a veinte minutos multiplicados por cada email del año. Quien escribe a mano «para lo importante» se está privando de la ayuda justo donde más la necesita. Tú vas a poder usarla también para lo importante, porque saldrá con tu voz desde el principio.

**Contraargumento 2:** Que prefieras escribirlo tú antes que mandar algo que no suena a ti dice mucho de tu forma de trabajar. No te conformas con «lo que salga», y eso es lo que te distingue del compañero que pega lo primero que le da ChatGPT. Ese estándar es tu mayor activo. Lo único que cambia aquí es que tu estándar, el de «esto tiene que sonar a mí», deja de depender de tu tiempo y pasa a estar escrito dentro de tu IA. Sigues siendo tú quien decide cómo suena. La diferencia es que ya no tienes que demostrarlo a mano en cada correo. Es la exigencia de siempre, pero sin el coste de siempre.

#### I-3. «Yo no tengo una "voz". No soy escritor» — Popularidad: 6/10
*Anclaje: A22 («no es copywriter profesional»), E3.*

**Cita escéptica:**
«Esto de "enseñarle tu voz a la IA" estará muy bien para escritores, periodistas o esa gente de LinkedIn que escribe posts bonitos. Yo no tengo voz. Yo escribo emails normales: "Hola, Pedro, te adjunto el presupuesto, cualquier cosa me dices, un saludo". Eso no es un estilo, es lo que escribe todo el mundo. Si le enseño eso a la IA, me va a escribir igual de soso, solo que con más palabras. El problema no es que la IA no suene a mí, es que yo tampoco sueno a nada en especial. No creo que haya mucho que "configurar" en mi forma de escribir. Me parece que esto está pensado para otro tipo de persona, alguien que escribe con gracia, no para alguien como yo, que escribe para quitarse el correo de encima.»

**Validación:** Es muy normal pensarlo. Casi nadie fuera del mundo de la escritura se considera alguien «con voz», y la palabra suena a novelista. Es fácil sentir que un producto así está hecho para gente que escribe con gracia, no para quien solo quiere despachar el correo.

**Contraargumento 1:** Pero mira lo que acabas de escribir: «Hola, Pedro, te adjunto el presupuesto, cualquier cosa me dices, un saludo». Eso **es** una voz. Corta, directa, cercana, sin adornos. Y es justo la que ChatGPT destroza cuando lo convierte en «Estimado Pedro: Espero que este mensaje le encuentre bien. Me complace adjuntarle…». Tu cliente reconoce tu «cualquier cosa me dices» igual que reconoce tu letra. Quien escribe «con gracia» tiene un problema distinto: su voz es más difícil de describir. La tuya es clarísima. En un foro sobre esto alguien lo explicaba muy bien: toda escritura tiene una voz propia, incluso la más sencilla o desordenada, porque tiene coherencia. La sencillez es tu ventaja: es la voz más fácil de enseñarle a una IA y la que más se nota cuando la pierde.

**Contraargumento 2:** Ir al grano, no adornar y escribir «para quitarte el correo de encima» es exactamente lo que la gente valora en un email. En los foros, los managers se quejan de los emails de IA larguísimos y llenos de relleno, y dicen que preferirían mensajes más cortos y auténticos. Tu forma de escribir es la que todos echan de menos. No necesitas «tener gracia». Necesitas que la máquina deje de estropear lo que ya haces bien. Lo extraordinario no es escribir bonito: es escribir como habla una persona de verdad. Y eso, tú ya lo haces.

#### I-4. «No tengo tiempo para ponerme a configurar nada» — Popularidad: 6/10
*Anclaje: Capacidad real (energía baja, compra de alivio); Restricción 10.*

**Cita escéptica:**
«Voy a tope. Entre el trabajo, la casa y todo lo demás, no tengo una tarde libre para sentarme a configurar la IA. Ya me cuesta encontrar media hora para contestar los correos que tengo pendientes. Y sé cómo acaban estas cosas: compras la guía, la abres, ves que son cuarenta páginas, dices "ya me pondré el fin de semana" y ahí se queda, en la carpeta de descargas, con el resto de cosas que compré y nunca miré. No quiero otra tarea más en la lista. Si fuera algo que funcionase al momento, vale, pero si me tengo que sentar una tarde a pensar cómo escribo y a hacer pasos, no lo voy a hacer. Me conozco. Y entonces habré tirado el dinero.»

**Validación:** Es muy sensato conocerse así. Todos tenemos esa carpeta de cosas compradas con buena intención y nunca abiertas, y cuando vas al límite cualquier tarea nueva pesa el doble. No quieres sumar otra promesa incumplida contigo mismo.

**Contraargumento 1:** Justamente porque vas a tope, eres quien más tiempo pierde con el sistema actual. Si cada email importante te lleva media hora en lugar de cinco minutos, eso no es «una tarde», son varias horas a la semana que se te escapan sin darte cuenta, cada semana. La persona que tiene tiempo de sobra puede permitirse reescribir. Tú no. Por eso la guía está pensada para hacerse **en una sola sesión**, con un primer cambio visible en los primeros minutos, para que no se quede en la carpeta de descargas. No son cuarenta páginas de teoría que leer antes de empezar: es un paso a paso que vas haciendo mientras lees. Y la recompensa es inmediata. El primer email que te ahorres reescribir ya te ha devuelto una parte de esa tarde.

**Contraargumento 2:** Que te conozcas tan bien es una virtud muy poco común. La mayoría compra y se engaña. Tú sabes que, si no es práctico y rápido, no lo vas a hacer, y eso es exactamente lo que hay que exigirle a cualquier cosa que compres. Es la mentalidad de alguien que valora su tiempo, que es lo que más vale en tu situación. Esta guía está hecha para gente como tú: los que no tienen tiempo que perder y por eso necesitan dejar resuelto algo **una vez** en lugar de pelearse con ello todos los días. Los que van sobrados de tiempo pueden seguir peleándose. Tú no tienes por qué.

#### I-5. «Me da cosa: usar algo para que no se note la IA es como hacer trampa» — Popularidad: 5/10
*Anclaje: C27, E19, E34, E36; Restricción 4.*

**Cita escéptica:**
«No sé, me genera un poco de conflicto. Una cosa es usar ChatGPT para ayudarme, y otra es comprar algo para que no se note que lo uso. Suena a esconder algo. ¿Y si un día el cliente se entera de que mis emails los escribe una máquina configurada para sonar como yo? Se sentiría engañado, y con razón. Mi jefe ya dijo una vez que está bien usar la IA, pero que tiene que ser mi trabajo. Si ahora hago que la IA se haga pasar por mí, ¿no es peor? Prefiero que se note un poco y que quede claro que no engaño a nadie, a que parezca que soy yo cuando no lo soy. Yo siempre he ido de frente con mis clientes y no quiero empezar ahora con estas cosas.»

**Validación:** Que te plantees esto dice mucho de ti. La honestidad con los clientes es lo que sostiene una relación de años, y es normal desconfiar de cualquier cosa que suene a «disimular». Nadie quiere ganar comodidad a cambio de sentir que oculta algo.

**Contraargumento 1:** Fíjate en lo que dicen los propios clientes y jefes en los foros: lo que les molesta **no es que uses IA**, igual que no les molesta que uses el corrector del Word. Les molesta recibir algo que no suena a ti, porque parece que no te has molestado. Y fíjate en la frase de tu jefe: «tiene que ser tu trabajo». Con esta configuración, el contenido, las ideas y las decisiones siguen siendo tuyas. Lo que cambia es que la herramienta deja de disfrazarte de asistente de atención al cliente. No es la IA haciéndose pasar por ti. Es la IA dejando de hacerse pasar por otro. El compañero que pega lo primero que sale sin leerlo sí está dando gato por liebre. Tú vas a mandar algo que dice lo que piensas, como lo dirías tú.

**Contraargumento 2:** Ese escrúpulo es lo que hace que tus clientes se fíen de ti, y es exactamente la persona para la que está hecha esta guía: alguien que quiere usar la herramienta **con honestidad**, que no busca engañar a un detector ni hacer pasar por suyo algo ajeno, sino que lo que firma le represente. Quien solo quiere esquivar un control no se hace esta pregunta. Tú sí te la haces, y por eso vas a usar la IA mejor que casi nadie: como una ayuda que respeta tu forma de ser, no como una máscara. Si algún día un cliente te pregunta, podrás decirle con toda tranquilidad que usas una herramienta que has ajustado para que escriba como tú, y que todo lo que te dice lo piensas tú.

### B. OBJECIONES EXTERNAS

#### E-1. «La IA siempre va a sonar a IA. No tiene arreglo» — Popularidad: 8/10
*Anclaje: A33, A29, A30, A34; Restricción 6.*

**Cita escéptica:**
«Llevo más de un año con esto y he llegado a una conclusión: la IA suena a IA y punto. Puedes cambiarle cuatro palabras, pedirle que sea más casual o que suene a persona, y al final siempre se le ve el plumero. Hay algo en cómo construye las frases que no se quita. En los foros en inglés hay gente que sabe muchísimo, que lleva semanas probando de todo, y dice lo mismo: que es casi imposible quitarle ciertos tics solo con instrucciones. Si ellos, que saben, no lo consiguen, ¿cómo lo voy a conseguir yo con una guía? Además, cada vez que sale una versión nueva parece que escribe peor, no mejor. Creo que hay que aceptar que es una herramienta para borradores y que lo que mandas, lo tienes que escribir tú.»

**Validación:** Después de un año de intentos, es una conclusión razonable. Has visto cómo los tics vuelven una y otra vez, y has leído a gente muy experimentada que dice lo mismo. Cuando lo intentas todo y sigue saliendo igual, aceptar el límite parece lo más sensato.

**Contraargumento 1:** Que hayas notado que «hay algo en cómo construye las frases» te pone por delante de la mayoría. Quien cree que el problema son cuatro palabras lleva meses quitando palabras y sigue igual. Tú has intuido lo que de verdad pasa: lo que delata a la IA no son solo las palabras, sino **cuatro huellas**: cómo se construyen las frases, el tono de asistente educado, el vocabulario y el ritmo en el que todo mide lo mismo. Los expertos de los foros fallan porque atacan una huella cada vez, casi siempre con listas de prohibiciones. Esta guía parte de lo que tú ya has visto y lo convierte en algo que se puede corregir de raíz. No es que no tenga arreglo. Es que se estaba intentando arreglar por el lado equivocado.

**Contraargumento 2:** Tu escepticismo es una señal de que tienes buen oído. Quien no distingue un texto de IA no se plantea nada de esto y manda sus emails «de folleto» tan tranquilo. Tú detectas la diferencia al instante, y precisamente por eso vas a notar enseguida cuándo tu IA empieza a sonar a ti. Ese oído es lo que hace que tus textos sean mejores que la media, con o sin IA. Una persona que ha probado mucho y ha mirado con atención es la que mejor sabe juzgar si algo funciona. Esta vez no tienes que creértelo: lo vas a comprobar en tu propio email, con tu propio oído.

#### E-2. «Hoy todo el mundo sospecha: aunque lo escriba yo, dirán que es IA» — Popularidad: 6/10
*Anclaje: F1, F5, A5, B-bloque (acusados sin culpa), E46.*

**Cita escéptica:**
«El problema ya no es la IA, es la gente. Hoy en día cualquier cosa bien escrita parece IA. Hay una periodista con no sé cuántos años de experiencia a la que acusaron de escribir "slop". A un chico le preguntó un cliente si lo había escrito ChatGPT después de pasarse veinte minutos escribiéndolo a mano. A mí mi jefe me dijo que un informe "sonaba a ChatGPT" y lo había hecho yo. Así que da igual: aunque la IA escriba como yo, alguien dirá que suena a IA, porque ahora lo dicen de todo. No veo por qué gastar dinero en que suene "humano" si al final la sospecha es la misma. Esto no lo arregla ninguna guía. Es una paranoia colectiva.»

**Validación:** Es verdad, y es injusto. La sospecha se ha disparado, y cualquier texto correcto puede recibir el «esto es de IA». Tiene que ser frustrante esforzarse y que te despachen con esa frase. Tiene sentido que pienses que el problema está fuera de ti.

**Contraargumento 1:** Precisamente porque la sospecha está por todas partes, sonar a ti se ha vuelto más valioso que nunca. Lo que dispara el «esto es de IA» no es escribir bien: es escribir **como escribe la IA**, con frases simétricas, fórmulas de cortesía de manual y un ritmo plano. Muchos de los acusados injustamente escribían con hábitos que la IA ha convertido en sospechosos. La guía te enseña a reconocer esas cuatro huellas, también en lo que escribes tú a mano. Quien no las conoce queda a merced de la paranoia. Tú vas a saber exactamente qué evita la sospecha. Con o sin IA, tus textos van a llevar tu marca, no la de la máquina, y eso es lo único que desactiva el «¿lo has escrito con ChatGPT?».

**Contraargumento 2:** Que te haya dolido que te acusaran de algo que no hiciste dice que te importa tu trabajo y tu nombre. Mucha gente se encoge de hombros. Tú no, y esa sensibilidad es lo que te hace ver un problema que otros todavía no ven. En un mundo donde todo empieza a sonar igual, la persona cuyos textos se reconocen a la primera es la que destaca, y tú ya tienes ese instinto. Esta guía no te pide que cambies quién eres para evitar la sospecha. Te ayuda a que se te reconozca aún más fácilmente, escribas como escribas. En lugar de defenderte de la paranoia, la dejas atrás.

#### E-3. «Esto lo arreglarán en la próxima versión, o cambiará y la configuración no servirá» — Popularidad: 6/10
*Anclaje: A19 («I hope someone from OpenAI sees this»), A34, D28, D29.*

**Cita escéptica:**
«Con la velocidad a la que va todo esto, cualquier cosa que compre hoy estará obsoleta en tres meses. O bien OpenAI se da cuenta de que la gente odia que escriba así y lo arregla en la siguiente versión, y entonces habré pagado por algo que viene de serie, o bien cambian los menús, la forma de configurarlo o el propio modelo, y la guía deja de servir. Ya pasó con esas webs que "humanizaban": funcionaban una semana y luego, con una actualización, dejaban de funcionar. Prefiero esperar a ver qué pasa. Si de verdad es un problema tan grande, ya lo arreglarán ellos. No tiene sentido que lo arregle yo por mi cuenta pagando.»

**Validación:** Es una preocupación muy razonable. Todo cambia a una velocidad absurda, has visto herramientas dejar de funcionar de una semana a otra y no quieres pagar por algo que se queda viejo enseguida ni por algo que quizá te regalen mañana.

**Contraargumento 1:** Mira qué es lo que caducó en esas webs: el truco, porque dependían de engañar a un detector que cambiaba cada semana. Esto no depende de ningún truco. Depende de algo que no cambia con las versiones: **cómo hablas tú**. Esa descripción de tu voz es tuya, la puedes copiar a cualquier versión nueva, a otra IA o al menú que inventen mañana. Y las empresas no van a «arreglar» que la IA suene a ti, porque no saben cómo hablas tú: la harán sonar mejor en general, a una persona genérica. Quien espera a que lo arreglen seguirá sonando como todos los demás que esperan. Tú tendrás algo propio que se lleva a cualquier herramienta. Y el PDF que explica por qué suena a IA no caduca: te sirve para juzgar cualquier texto, de la versión que sea.

**Contraargumento 2:** Que no te dejes arrastrar por la novedad y te preguntes cuánto va a durar algo antes de comprarlo es exactamente la actitud de quien toma buenas decisiones a largo plazo. Es la que tienen tus mejores clientes, y probablemente la que te ha mantenido a flote en un sector que cambia. Esa forma de pensar es la que hace que esta guía tenga más valor para ti que para nadie: no te vende una herramienta que hay que renovar, sino un conocimiento y una configuración que son tuyos. Lo que construyes una vez se queda. Eso es lo que buscas, y es lo que encaja con alguien que piensa como tú.

#### E-4. «Uso la cuenta del trabajo, o la gratuita, y no puedo tocar esas cosas» — Popularidad: 5/10
*Anclaje: C21 (controles corporativos), Capacidad real (restricciones logísticas); Restricción 11. Debe resolverse en el producto.*

**Cita escéptica:**
«Esto estará muy bien para quien tiene su ChatGPT de pago y lo controla, pero yo uso el del trabajo, que nos lo puso la empresa, y no sé si me dejan tocar los ajustes. Igual hasta queda registrado y me preguntan qué he hecho. Una compañera tuvo un lío con el departamento de informática por pegar cosas que no debía. Y en casa uso la versión gratuita, que no sé si tiene todas esas opciones de personalizar. No me apetece pagar 29 euros para descubrir luego que en mi caso no sirve porque mi cuenta no tiene esa función, o que la empresa no deja. Necesito saber antes, con claridad, si esto funciona en mi situación, porque si no, es tirar el dinero.»

**Validación:** Es una pregunta muy sensata, y mucha gente no se la hace hasta que ya ha pagado. Que te preocupe no meterte en líos en el trabajo y saber de antemano si funciona en tu caso es pura responsabilidad. Nadie quiere descubrir después que no le servía.

**Contraargumento 1:** Que pienses en esto antes de comprar te coloca por delante de los que compran a ciegas y luego piden la devolución. Por eso la página tiene que decirte con claridad, antes de pagar, **en qué planes y cuentas funciona cada parte** [**el creador debe verificar y declarar los requisitos reales**]. Y para los casos en los que no puedes dejarlo configurado (una cuenta de empresa bloqueada, por ejemplo), la guía te enseña a crear tu propia «ficha de voz» en un documento que pegas al empezar. No es tan cómodo como dejarlo fijo, pero es igual de tuyo y no toca ningún ajuste que no puedas tocar. Quien no se informa se queda sin nada. Tú vas a saber exactamente qué opción es la tuya antes de gastar un euro.

**Contraargumento 2:** La prudencia con las herramientas de la empresa y con lo que pegas en ellas dice mucho de tu profesionalidad. En los foros hay gente que se ha metido en problemas serios por no pensarlo. Tú lo piensas, y eso es lo que te convierte en el tipo de persona que usa la IA bien: con cabeza, respetando las normas y sin exponerse. Esta guía está hecha para esa forma de trabajar. No te pide subir documentos a ningún sitio raro ni instalar nada en el ordenador de la empresa, y te ofrece una alternativa limpia si tu cuenta no lo permite. Tu prudencia no es un obstáculo: es la razón por la que te va a ir bien con esto.

#### E-5. «Los detectores lo marcarán igual, y en mi empresa los usan» — Popularidad: 4/10
*Anclaje: E30 (el director de IT pasa emails por detectores), B18, B20, D-bloque.*

**Cita escéptica:**
«En mi empresa hay quien pasa los textos por detectores de IA. Ya lo hicieron con los emails de la directora de Recursos Humanos y les salió "IA" a la primera. Así que da igual que suene a mí: si un día a alguien le da por meter mi email en uno de esos programas y le sale un 80 %, me van a mirar raro. Yo no sé cómo funcionan esos detectores, pero sí sé que la gente se los cree. Si esta guía no me garantiza que el texto pase los detectores, no sé de qué me sirve. Las webs esas por lo menos te lo prometen, aunque luego no lo cumplan. Esto ni siquiera lo promete.»

**Validación:** Entiendo la inquietud. Si en tu entorno alguien usa detectores y se fía de ellos, es lógico temer que una cifra te ponga en evidencia aunque el texto sea tuyo. Es incómodo depender de una máquina que no entiendes.

**Contraargumento 1:** Lo que te ha pasado por la cabeza es exactamente lo que las webs de «humanizar» explotan. Pero mira lo que pasa en sus reseñas: el mismo texto da 0 %, 40 % y 100 % en distintos detectores; el detector de la propia web dice «100 % humano» y otro dice «100 % IA»; textos escritos a mano salen como IA. **Nadie puede garantizarte un detector, porque los detectores no son fiables**, y quien te lo garantiza te está mintiendo. Por eso aquí no se promete. Lo que sí está en tu mano es lo que de verdad decide en tu trabajo: que la persona que lo lee (tu jefe, tu cliente, tu compañero) reconozca tu forma de escribir. Un 80 % en una máquina se discute. Un email que suena a ti no hay que discutirlo.

**Contraargumento 2:** Que te fíes más de lo que ves que de una promesa que «luego no cumplen» dice que tienes buen juicio. Quien se compra la promesa del 0 % acaba pagando la suscripción, viendo cómo falla y con el texto destrozado. Tú prefieres la honestidad de alguien que te dice lo que puede y lo que no puede hacer. Esa es justo la mentalidad que hace falta: la de quien sabe que la confianza de las personas se gana con lo que escribes, no con un porcentaje. Y si alguna vez alguien te enseña una cifra, tendrás algo mucho más sólido que un número: textos que cualquiera que te conozca sabe que son tuyos.

### C. PREOCUPACIONES SOBRE EL PRODUCTO

#### P-1. «Esto es otro humanizador / otra estafa» — Popularidad: 9/10
*Anclaje: D1, D3, D6, D8, D14, D25; sesgo de disponibilidad; Restricción 9.*

**Cita escéptica:**
«Ya me sé cómo va esto. Te prometen que tu texto va a sonar humano, te enseñan un antes y un después precioso, pagas y luego descubres la letra pequeña. Me pasó con una de esas webs: decía "al mes, cancela cuando quieras" y me cobraron el año entero. Otra vez vi un cargo en la cuenta que ni reconocía, y era de una herramienta que creía haber cancelado. Y el texto que me devolvían era peor que el original: palabras raras, mayúsculas en medio de la frase. Así que, cuando veo algo que promete que la IA no se va a notar, mi primer pensamiento es "otra estafa más". No voy a volver a caer. Ya busqué en Google "nombre más estafa" con los anteriores, y con este haré lo mismo.»

**Validación:** Después de eso, sería raro que no desconfiaras. Te cobraron lo que no esperabas, te dejaron el texto peor y encima tuviste que pelear para recuperar el dinero. Buscar «estafa» antes de pagar no es paranoia: es aprender de lo que te pasó.

**Contraargumento 1:** Esa experiencia te da una ventaja enorme: sabes exactamente qué tienen en común todas esas webs. Viven de que vuelvas. Te cobran por cada texto, por cada palabra o cada mes, porque su negocio es arreglar **después** lo que tu IA escribe mal **antes**. Esto funciona al revés: lo configuras una vez dentro de tu propia IA y, a partir de ahí, **no me necesitas**. No hay suscripción que cancelar, ni créditos, ni otra pestaña, ni otra web que reescriba tu texto a ciegas. Se paga una vez, el precio se ve antes de pulsar y, si no te convence, te devuelvo el dinero, no créditos. Quien no ha vivido lo que tú no sabe distinguir. Tú vas a reconocer en diez segundos que esto es lo contrario de lo que te estafó.

**Contraargumento 2:** Buscar «estafa» antes de comprar es lo que hace la gente lista. Mientras otros siguen pagando la renovación automática sin enterarse, tú aprendiste, te protegiste y ahora exiges pruebas. Esa exigencia te hace exactamente el tipo de cliente con el que esto funciona mejor, porque vas a mirar con lupa la demostración, vas a comprobar el resultado en tu propio email y no te vas a conformar con promesas. Haz esa búsqueda, por supuesto. Y luego compara: una cosa vive de que dependas de ella; esta otra te deja libre. Que hayas sido escéptico hasta ahora no es un defecto. Es la razón por la que, cuando algo sea de verdad, lo vas a reconocer.

#### P-2. «Ya probé las Instrucciones personalizadas y no funcionó» — Popularidad: 8/10
*Anclaje: A19, A26, A27, A29, E9, E12; Restricción 7. Es la objeción más peligrosa para el mecanismo del producto.*

**Cita escéptica:**
«Esto que vendéis ya lo hice yo. Encontré en un vídeo unas instrucciones para pegar en los ajustes de ChatGPT, de esas de "no uses palabras formales, no uses listas, escribe como una persona", y las puse. Los primeros mensajes, bien. Pero en cuanto la conversación se alargaba, volvía a lo de siempre: el "¡Claro!", el "en resumen", las tres frases que empiezan igual. Luego probé a darle ejemplos de mis emails y a explicarle mi estilo, y después de seis u ocho intentos seguía sonando a robot. En los foros hay mucha gente diciendo lo mismo. Así que no me vengas con que una "configuración permanente" lo arregla, porque es exactamente lo que hice y no funcionó. ¿Qué tiene esto de diferente?»

**Validación:** Tienes toda la razón para desconfiar: lo intentaste en serio, con instrucciones y con ejemplos, y viste cómo se deshacía a los pocos mensajes. Es frustrante dedicarle tiempo y comprobar que vuelve a ser lo de siempre. Es normal que «configuración permanente» te suene a lo mismo.

**Contraargumento 1:** Has hecho algo que la mayoría ni se plantea, y eso te pone en el mejor sitio para entender por qué falló. Las instrucciones típicas que circulan fallan por tres motivos: (1) dicen **lo que no hacer** («no uses palabras formales») y, como pasa cuando le pides que no suene a IA, la máquina piensa todavía más en lo prohibido; (2) son **de otra persona**, una plantilla genérica que no describe cómo hablas tú; y (3) no tienen en cuenta que **en conversaciones largas se diluyen**. Esta guía ataca los tres puntos: construyes tu configuración **en positivo**, a partir de tu forma real de escribir, atacando las cuatro huellas y no solo el vocabulario, y con pautas para que no se degrade. Tú ya sabes dónde estaba el fallo. Esto empieza justo ahí.
*[**Condición de producto:** este contraargumento solo es honesto si el producto hace de verdad estas tres cosas.]*

**Contraargumento 2:** Que lo hayas intentado por tu cuenta, con constancia y probando cosas distintas, dice que no eres de los que se rinden ni de los que esperan que se lo den todo hecho. Esa curiosidad y esa persistencia son raras, y son lo que distingue a quien acaba dominando una herramienta de quien la abandona. Lo único que te ha faltado es el mapa, no las ganas. Con esa base vas a sacar mucho más partido que alguien que empieza de cero, porque reconocerás en cada paso por qué funciona. La gente como tú, la que ya se ha peleado con el problema, es la que mejor nota la diferencia cuando por fin algo encaja.

#### P-3. «Esto lo encuentro gratis en YouTube» — Popularidad: 7/10
*Anclaje: E53 (rulebook gratuito en un short), E24, E25.*

**Cita escéptica:**
«Hay vídeos en YouTube y en TikTok que te dan las instrucciones gratis. Vi uno de un minuto que decía exactamente esto: "en vez de pelearte con ChatGPT cada vez, dale un manual de reglas una vez". ¿Por qué voy a pagar 29 euros por algo que me cuentan gratis en un vídeo? Además hay mil artículos con listas de palabras que delatan a la IA. Si me pongo una tarde, seguro que lo encuentro todo sin pagar. Está claro que el truco ya circula por ahí. Pagar por esto me parece pagar por algo que ya es de dominio público.»

**Validación:** Es verdad que circulan vídeos y listas gratis, y es razonable no querer pagar por lo que parece estar al alcance de cualquiera. Si ya has visto la idea en un minuto, pagar por ella parece de primo.

**Contraargumento 1:** Tienes razón en que la **idea** circula: «configúralo una vez» ya se dice en vídeos de un minuto. Y precisamente por eso has visto también que con la idea no basta. Ese vídeo te da **unas reglas**, las suyas, genéricas, para pegar y ya. Es lo que mucha gente ha probado y lo que se degrada a los tres mensajes. Lo que no te da un vídeo de un minuto es **la tuya**: entender las cuatro huellas para saber qué corregir, construir tu configuración a partir de cómo escribes tú y comprobar paso a paso que funciona en tu email. Quien se queda con el vídeo gratis se queda con la plantilla de otro. Tú pagas por no tener que pasarte una tarde buscando entre mil artículos contradictorios y por acabar con algo tuyo que funciona.

**Contraargumento 2:** Que busques primero lo gratis demuestra que no tiras el dinero, y eso es un rasgo de alguien que gestiona bien sus recursos. Esa misma cabeza te dirá cuánto vale tu tiempo: una tarde buscando, probando plantillas ajenas que no suenan a ti y volviendo a reescribir cuando fallan, frente a una guía que te lleva directamente al resultado. La persona que sabe distinguir entre una idea gratis y un método que funciona es la que mejor invierte. No pagas por la idea, que ya conoces. Pagas por saltarte todos los intentos fallidos que la idea sola provoca.

#### P-4. «¿Un PDF y un plugin por 29 €? ¿Qué tiene que no tenga un prompt?» — Popularidad: 6/10
*Anclaje: Lógica transaccional; criterio de precio; formato del producto.*

**Cita escéptica:**
«A ver si lo he entendido: un PDF y una especie de plugin. Por 29 euros. Un PDF lo hace cualquiera y, al final, lo que te dan será un texto largo para pegar en ChatGPT, o sea, un prompt. ¿Cuánto vale un prompt? Nada. Por ese precio me compro un libro entero. Si fuera un programa, una aplicación o algo con soporte, vale, pero un PDF… Además no sé ni qué es eso del "plugin" o la "skill", ni si me va a servir en mi ordenador. No veo dónde está el valor. Me da la sensación de que pago por algo que, si lo ves por dentro, son cuatro párrafos.»

**Validación:** Es justo preguntárselo. Hay mucho PDF inflado que, por dentro, son cuatro ideas, y cuando no ves el producto físico cuesta ver el valor. Comparar con un libro es lo más natural del mundo.

**Contraargumento 1:** Haces bien en comparar, así que comparemos con lo que de verdad compite en tu cabeza. Una web «humanizadora» cuesta de 20 a 200 euros al año, cobra cada mes y te deja el texto peor. Media hora retocando cada email importante es tu tiempo, cada día. Esto se paga una vez, por menos que un mes de cualquiera de esas webs, y no es «un prompt»: es (1) entender por qué tu IA suena a IA, que es lo que te permite juzgar cualquier texto el resto de tu vida, y (2) **una guía que te va haciendo preguntas y te ayuda a construir tu propia configuración**, la que describe cómo hablas tú y que nadie puede venderte hecha porque no te conoce. Quien compra un prompt genérico se lleva cuatro párrafos de otro. Tú te llevas los tuyos.

**Contraargumento 2:** Que no te dejes impresionar por el formato y vayas directo a la pregunta («¿qué me llevo?») es el tipo de pensamiento que tienen los buenos compradores. No pagas por el papel ni por la tecnología. Pagas por el resultado: dejar de reescribir y que tus textos vuelvan a ser tuyos. Y lo valioso de verdad, tu voz descrita y puesta a trabajar, lo vas a aportar tú, con la guía como andamio. Por eso funciona: la gente que valora el resultado más que la apariencia es la que mejor partido saca de algo así.

#### P-5. «¿Y si estropeo mi ChatGPT? ¿Y mis datos?» — Popularidad: 5/10
*Anclaje: Capacidad real (miedo a romper), C21; HIP sobre la palabra «plugin».*

**Cita escéptica:**
«Lo que me preocupa es tocar algo y que luego ChatGPT empiece a hacer cosas raras. Lo uso todos los días para trabajar; si se me estropea, me fastidia la semana. Y eso del plugin… ¿qué hace exactamente? ¿Tengo que darle acceso a mis correos? ¿Va a leer lo que escribo? Ya hay bastante con que la IA tenga mis cosas como para meter a otro intermediario. No sé cómo se deshace si no me gusta, ni si va a cambiar algo de mi cuenta. Si no tengo claro que es seguro y que puedo volver atrás, prefiero no arriesgarme. Prefiero un ChatGPT que escribe como un robot pero que funciona a uno que escribe como yo pero que no sé qué está haciendo.»

**Validación:** Proteger la herramienta con la que trabajas y tus datos es lo mínimo que hay que exigir. Es razonable querer saber qué hace exactamente cada cosa y cómo volver atrás antes de tocar nada.

**Contraargumento 1:** Haces exactamente las preguntas que hay que hacer, y merecen respuestas claras antes de pagar: qué hace la guía, qué escribes y dónde, qué no toca nunca (tus correos, tus documentos, tu cuenta) y cómo se deshace [**el creador debe documentarlo con precisión según el formato real del producto**]. La configuración principal no es más que un texto que tú escribes en un menú de tu propio ChatGPT, un texto que puedes leer entero, cambiar cuando quieras y borrar en un minuto para volver a como estaba. No se conecta a tu correo ni se queda con lo que escribes. Quien instala cosas sin preguntar es el que se lleva los sustos. Tú vas a saber en todo momento qué hay dentro, porque lo vas a haber escrito tú.

**Contraargumento 2:** Que antepongas la seguridad a la comodidad es una señal de madurez digital que mucha gente, incluidos muchos usuarios «avanzados», no tiene. Esa forma de pensar es justamente la que hace que esta configuración sea perfecta para ti, porque es transparente: no es una caja negra, es tu propia descripción de cómo escribes. No tienes que fiarte de un intermediario, porque el control lo tienes tú. Las personas que preguntan antes de tocar nada son las que mantienen sus herramientas en orden y nunca pierden el trabajo. Esa prudencia no te aleja de esto: te convierte en el usuario ideal.

### Clasificación de las 15 objeciones por momento de lectura de la carta

| Objeción | (a) Momento principal | (b) Momento secundario | (c) Elemento que la resuelve |
|---|---|---|---|
| I-1 No soy técnico | **M1 — Titular / primeras líneas** | M3 | **Titular/subtitular** («sin programar, en tu ChatGPT») + bullet de capturas paso a paso |
| I-2 Para lo que tardo, lo escribo yo | M2 — Historia | M4 | **Historia** (la media hora frente a los cinco minutos) + **anclaje de precio** (coste del tiempo) |
| I-3 No tengo voz | M3 — Bullets / producto | M2 | **Bullet específico** («tu "cualquier cosa me dices" ya es una voz») |
| I-4 No tengo tiempo | M4 — Precio | M3 | **Bullet** («una sola sesión, primer cambio en minutos») + **anclaje de precio** |
| I-5 Es hacer trampa | M2 — Historia | M1 | **Historia** (la norma «usar está bien; que se note, no») + reencuadre en el lead |
| E-1 No tiene arreglo | **M1 — Titular / primeras líneas** | M2 | **Titular/lead** (la paradoja y las cuatro huellas) |
| E-2 Todos sospechan | M2 — Historia | M3 | **Historia** + bullet («las huellas también en lo que escribes a mano») |
| E-3 Lo arreglarán / caducará | M4 — Precio | M3 | **Anclaje de precio** («tuyo, portable, sin renovar») + bullet de portabilidad |
| E-4 Cuenta de trabajo / gratis | M3 — Bullets / producto | M4 | **Bullet específico** de requisitos + FAQ cerca del precio |
| E-5 Detectores | M3 — Bullets / producto | M1 | **Bullet** («no prometemos detectores: te explicamos por qué nadie puede») |
| P-1 Otro humanizador / estafa | **M1 — Titular / primeras líneas** | M4 | **Lead** («no es otro humanizador») + **garantía** (dinero, no créditos) |
| P-2 Ya probé instrucciones | M2 — Historia | M3 | **Historia** (los tres motivos del fallo) + bullet («en positivo, con tu voz, resiste») |
| P-3 Gratis en YouTube | M4 — Precio | M3 | **Anclaje de precio** («no pagas la idea, pagas saltarte los intentos») |
| P-4 PDF + plugin por 29 € | M4 — Precio | M3 | **Anclaje de precio** (frente a los humanizadores y al tiempo) + bullet del contenido |
| P-5 Estropear / datos | M3 — Bullets / producto | M4 | **Bullet** de transparencia y reversibilidad + **garantía** |

**Lectura de la tabla:** el **Momento 1** concentra las tres objeciones más populares (I-1, E-1, P-1). Por eso **el titular y el lead tienen que desactivar a la vez el «no soy técnico», el «no tiene arreglo» y el «otra estafa»**. Encaja con la palanca crítica (reducir la ansiedad) y con la decisión de romper la predicción.

---

## Lógica Transaccional y Justificación

### 1. Prioridades de gasto (derroche frente a ahorro)

**¿En qué gasta alegremente? [HIP basada en mercados similares; DATO INSUFICIENTE en el corpus]**
- Café y comidas fuera en días de trabajo.
- La suscripción de ChatGPT Plus o Claude Pro, si ya la tiene: lo justifica como «herramienta de trabajo». A28 sugiere que paga.
- Pequeñas mejoras de comodidad: un teclado mejor, una funda, una app que «le arregla algo».
- Formación corta y práctica **si es pago único** y parece útil al momento.

**¿En qué es irracionalmente tacaño?**
- **Suscripciones** de software que no entiende (la herida de D8, D14 y D25).
- **Herramientas de IA «extra»** («ya pago ChatGPT, no voy a pagar otra cosa encima»). **[HIP con anclaje A28]**
- **Cosas que «deberían venir de serie»** («¿por qué tengo que pagar para que ChatGPT funcione bien?»). **[HIP]**
- **Productos digitales sin «cosa»**: le cuesta ver el valor de un PDF. **[HIP]**

**¿Cómo encuadrar la oferta en el «derroche aceptable»?**
- Como **herramienta de trabajo de pago único**, en la misma categoría mental que «el ratón bueno» o «el curso de Excel que por fin me ahorró horas».
- Como **lo contrario de una suscripción**: «menos de lo que cuesta un mes de esas webs que no funcionan, y para siempre».
- Como **mejora de algo que ya paga**: «sacarle partido de verdad a tu ChatGPT».

### 2. El coste de la inacción (ROI negativo)

**Monetización del problema** **[cálculo ilustrativo HIP sobre anclas ANCL]**:
- **Tiempo:** si un email importante pasa de 5 a 30 minutos (F2) y escribe **3 al día**, son **75 minutos diarios** de exceso → unas **6 horas a la semana** → unas **25 horas al mes**. Con un coste-hora prudente de 15 € (empleado medio), son unos **375 € al mes** en tiempo de retoque. Con el coste-hora de un autónomo (30-50 €), entre **750 y 1.250 € al mes**. Aunque fueran solo 15 minutos de exceso al día, serían unas 5 horas al mes, es decir, 75-250 €.
- **Dinero tirado en humanizadores:** 20 $ (D1), 60 $ (D9), unos 180 $/año (D36) y más de 200 $/año (D8).
- **Coste comercial:** un cliente que pide descuento al sospechar IA (E19) o un proyecto despachado con un «suena a ChatGPT» (F7: más de 50 horas de trabajo). Una sola de estas situaciones supera con creces el precio. **[ANCL, minoritario]**
- **Coste del límite de uso:** mensajes del plan consumidos corrigiendo el tono (A28).

**Argumento lógico sólido:**
> **«Invertir 29 € una vez te ahorra la media hora que hoy le dedicas a retocar cada email importante. Si escribes tres al día, recuperas el precio el primer día. Todo lo que viene después es tiempo tuyo.»**

**Precaución:** las cifras son **ilustrativas**. En el copy hay que presentarlas como un cálculo que el lector hace con sus propios números («haz la cuenta con los tuyos»), no como datos medidos.

### 3. Anclaje de precios

**¿Con qué va a comparar el precio?**
1. Con **los humanizadores** (20, 60, 180 o más de 200 $, con suscripción).
2. Con **un mes de ChatGPT Plus** (unos 20-23 €). **[HIP]**
3. Con **un libro** (15-25 €).
4. Con **el vídeo gratis de YouTube** (0 €).
5. Con **contratar a un redactor** (para un autónomo, cientos de euros al mes). **[HIP]**

**3 comparaciones favorables:**
1. **«Menos de lo que te cobra una web "humanizadora" en un solo mes, y no se renueva nunca.»**
2. **«Lo que cuesta una comida de menú con café. Una vez. Para todos los emails que escribas a partir de hoy.»**
3. **«Una sola hora de un redactor profesional cuesta más, y él tampoco sabría cómo hablas tú.»**

**Comparación que hay que evitar:** con el libro, porque coloca el producto en la categoría «información», donde 29 € parece caro. Hay que llevarlo a la categoría «herramienta / resultado».

### 4. Formato numérico preferido

- **Formato dominante: coste de la inacción por unidad de tiempo** («Cada email importante te cuesta media hora de retoques»; «Cada semana que lo dejas, son seis horas más»). **Por qué:** el dolor se vive a diario y el tiempo es la única métrica medible del problema (Matriz, medibilidad 4). Además crea urgencia natural sin escasez artificial, y eso es clave para el cuadrante de ansiedad.
- **Formato secundario: velocidad de retorno** («Lo recuperas el primer día que no reescribes»). **Por qué:** con un precio bajo y un ahorro diario, el retorno es casi inmediato, lo que refuerza la sensación de compra sensata.
- **Formatos que hay que evitar:**
  - **Porcentajes de mejora** («un 80 % más humano»): recuerdan a los detectores y a los humanizadores.
  - **Ahorro total anual** («ahorras 3.000 € al año»): suena a gurú y no es creíble con este precio.
- **Implicación para el copy:** los números aparecen **tarde**, después de la demostración, siempre en **minutos y en «cada vez»**, y siempre invitando a que el lector haga su cuenta.

### 5. El guion de «permiso»

> **«No me estoy comprando otro cacharro de IA: me estoy ahorrando la media hora que pierdo cada día retocando lo que escribe el que ya tengo.
> Lo pago una vez, menos que un mes de esas webs que no funcionaban, y si no me sirve me devuelven el dinero.
> Es lo que haría cualquiera que se toma en serio su trabajo: ajustar la herramienta a su medida en lugar de pelearse con ella todos los días.»**

---

## Alternativas a Eliminar

> Cada alternativa se nombra por su **categoría genérica**, como pide el prompt. Los hechos que se citan salen del corpus (con su código). **El producto no tiene todavía casos de éxito propios.** Donde el prompt pide «casos de éxito», la ventaja se argumenta con el mecanismo y la lógica, y se marca dónde habrá que añadir casos reales cuando existan. No se inventa ninguno.

### 1. Las webs «humanizadoras» de texto por suscripción

**a) Qué prometen y cómo funcionan:** pegas el texto que te ha escrito la IA en una caja, le das a un botón y la web lo «reescribe» para que suene humano y «no lo detecte nadie». Suelen enseñarte un porcentaje de «humano» y cobrarte por palabras, por créditos o por suscripción mensual o anual.

**b) Desventajas:** Vale, seamos sinceros. Suena a magia: pegas, clicas, listo. Pero mira lo que cuentan quienes las han pagado. Una persona metió su texto y el porcentaje de IA **subió** del 20 % al 80 % (D15). Otra recibió el texto con mayúsculas en medio de las frases y palabras que no existen, y cada vez que repetía el proceso se le iban miles de palabras del plan (D23). Otra cuenta que la herramienta le cambió el sentido de lo que quería decir (D19, D33). Y luego está la parte de la tarjeta: «decía al mes y me cobraron el año entero» (D14), un cargo de más de 200 dólares que no esperaba (D8), una suscripción que creía cancelada y que seguía cobrando (D25), y créditos en lugar de devolución (D10). Encima hay que esperar: una persona tardó casi una hora en procesar mil palabras, con bucles de reCAPTCHA incluidos (D37). Así que pagas, esperas y te toca arreglar lo que te han roto.

**c) Por qué lo nuestro es mejor:** Ahora, piénsalo así: esas webs arreglan **después** lo que tu IA escribe mal **antes**. Por eso necesitan que vuelvas cada vez, y por eso te cobran cada mes. Lo nuestro va a la raíz: configuras una vez tu propia IA para que escriba con tu voz desde el primer mensaje. Sin caja donde pegar, sin otra pestaña, sin porcentajes que no significan nada y sin un tercero que reescriba tu texto a ciegas y te cambie lo que querías decir. Tu texto sale bien a la primera porque tu IA ya sabe cómo hablas. Y se paga una vez. No hay nada que cancelar, porque no hay nada que se renueve. Si no te convence, te devolvemos el dinero, dinero de verdad y no créditos. Es la diferencia entre ir al mecánico cada semana por el mismo ruido o arreglar la pieza que lo provoca. *(Casos de éxito: añadir cuando existan.)*

### 2. Reescribirlo todo a mano

**a) Qué promete y cómo funciona:** la solución «de toda la vida». Le pides a la IA un borrador y luego lo rehaces tú, frase por frase, hasta que suena a ti. La gente lo da como consejo de oro: «que te lo escriba la IA y luego lo reescribes con tus palabras» (E36).

**b) Desventajas:** Funciona, no te digo que no. El problema es lo que cuesta. Un email de cinco minutos se convierte en media hora de relecturas (F2). Alguien en un foro contaba que reescribe más o menos la mitad de cada borrador y borra las palabras que jamás usaría (A4). Otro lo resumía en tres palabras: «basically rewriting it anyway», o sea, que al final lo reescribe igual (A31). Y otro remataba: «para cuando le he explicado lo que quiero, ya podría haberlo escrito yo» (E22). Así que el ahorro que te prometía la IA desaparece. Y no solo pierdes tiempo, también energía. Al final del día ya no reescribes con la cabeza fresca, sino con prisa, y se te cuela el «Espero que este mensaje te encuentre bien» que no viste. Es un sistema que depende de tu vigilancia, y la vigilancia se cansa.

**c) Por qué lo nuestro es mejor:** Lo que quiero decir es que reescribir a mano es poner tu esfuerzo en el sitio equivocado. Estás corrigiendo el resultado cuando lo que falla es el punto de partida. Si tu IA ya escribe con tu forma de hablar, el borrador sale cerca de lo que tú escribirías y tu trabajo pasa de «rehacer» a «leer y enviar». Sigues revisando el contenido (las cifras, las fechas, lo que de verdad importa), pero dejas de pelearte con el tono. Y lo bueno es que no dependes de estar despierto y atento a las once de la noche: tu voz está escrita en la configuración, no en tu cansancio. Sigues teniendo el control de cada palabra, pero sin pagarlo con media hora cada vez.

### 3. Pedirle «que suene más natural» en cada mensaje

**a) Qué promete y cómo funciona:** el truco más común. Al final de tu petición añades «que suene natural», «más casual», «menos formal» o directamente «que no suene a IA». Es gratis, inmediato y está a mano.

**b) Desventajas:** Si eso te suena familiar, ya sabes cómo acaba. Una persona se pasó un cuarto de hora atascada con una frase de un email importante, se la pegó a ChatGPT con un «que suene más natural» y el resultado no le sirvió (A20). Otra lo dijo con todas las letras: «por el amor de Dios, no le digas que no suene a IA. Lo probé y te juro que usó todos sus clichés favoritos todo lo que pudo» (E12). Otra probó con tono casual y cínico y seguía recibiendo textos «ridículos» (A26). Y en los textos largos vuelve siempre la misma cadencia impecable (A25). El problema de fondo es que «natural» no significa nada para la máquina: no sabe cuál es **tu** natural. Además, tienes que repetirlo en cada mensaje, y cada vez que lo repites gastas tiempo y, si tienes límite de uso, mensajes (A28).

**c) Por qué lo nuestro es mejor:** Verás, pedir «más natural» es como decirle a un sastre «hazme un traje que me quede bien» sin dejarle tomarte las medidas. Lo intentará, pero te hará uno de talla estándar. Nuestra configuración es tomar las medidas: le dices a tu IA, una sola vez y bien explicado, cómo hablas tú, qué palabras usas, cómo saludas y cómo te despides, lo largo o corto que escribes. A partir de ahí no tienes que pedirle «natural» en cada mensaje, porque ya sabe cuál es tu natural. Y como está construida en positivo (lo que eres, no lo que no debe hacer), evitas el efecto rebote de «no suenes a IA», que mete aún más clichés. ¿Tiene sentido, verdad?

### 4. Las listas de palabras prohibidas

**a) Qué prometen y cómo funcionan:** artículos, carruseles y posts que te dan «las 30 palabras que delatan a ChatGPT» para que las quites, o para que le pidas a la IA que no las use nunca.

**b) Desventajas:** Ahora, no me malinterpretes: algunas palabras chirrían de verdad. Pero mira lo que cuentan quienes lo han probado. Las listas de patrones prohibidos quitan algunos tics, pero no consiguen meter tu personalidad en el texto (A29). Alguien lo advertía en un foro: evitar activamente esas frases puede hacer que suenes como una IA a la que le han dicho que nunca use esos términos (E9). Otro decía que usar una o un puñado de palabras como prueba de «esto es IA» es un criterio terrible (E4). Y hay un problema más: los tics cambian con cada versión. Las palabras que eran el meme hace dos años ya no son las que la gente nota ahora. Ahora la gente se queja de las frases cortadas y de la cadencia entrecortada (A33). Una lista se queda vieja en unos meses. Quitas palabras y el texto sigue sonando igual, porque lo que suena a máquina no es solo el vocabulario.

**c) Por qué lo nuestro es mejor:** Lo siguiente que debes saber es esto: el vocabulario es **una** de las cuatro huellas. Las otras tres son cómo se construyen las frases (siempre con la misma estructura), el tono de asistente educado (la hiperformalidad) y el ritmo en el que todo mide lo mismo (la cadencia uniforme). Nuestro PDF te enseña a ver las cuatro y la configuración las ataca a la vez, desde tu voz y no desde una lista de prohibiciones. Y como se basa en cómo hablas tú y no en las palabras de moda de este año, no caduca cuando cambia la versión de la IA. Mientras otros siguen tachando palabras, tú tienes una IA que suena a ti de entrada.

### 5. Las plantillas gratuitas de instrucciones (los vídeos de un minuto)

**a) Qué prometen y cómo funcionan:** un short o un reel te dice: «En vez de pelearte con ChatGPT cada vez, dale un manual de reglas una vez» (E53), y te enseña un texto para pegar en los ajustes.

**b) Desventajas:** Bueno, déjame decirte algo: la idea es buena. Tan buena que es la misma que la nuestra. El problema está en la ejecución. Esa plantilla es **la del creador del vídeo**, con sus reglas y su estilo, genérica para millones de personas. Quienes han probado este tipo de instrucciones cuentan que funcionan al principio y se degradan a medida que avanza la conversación (A19). Una persona dio ejemplos e instrucciones, gastó seis u ocho intentos y seguía saliendo «terriblemente IA» (A27). Otra probó varias instrucciones de personalización y sigue con textos ridículos (A26). Y el vídeo dura un minuto: no te explica por qué funciona ni qué hacer cuando falla, ni sabe nada de ti. Si tu pantalla es distinta a la suya, ni siquiera sabes dónde pegarlo.

**c) Por qué lo nuestro es mejor:** Vale, sigamos. Nosotros partimos de la misma intuición (configurarlo una vez), pero hacemos lo que el vídeo no puede hacer. Primero, te explicamos **por qué** suena a IA, para que sepas qué estás corrigiendo. Segundo, en lugar de darte la plantilla de otro, te guiamos paso a paso para construir **la tuya** a partir de cómo escribes tú. Tercero, la construimos en positivo y con pautas para que no se diluya en conversaciones largas, que es donde fallan las plantillas genéricas. Y todo en la pantalla que ya conoces, en español, con capturas. Es la diferencia entre ver a alguien conducir en un vídeo y que alguien te siente al volante de tu coche y te lo enseñe.

### 6. Los packs de prompts de pago

**a) Qué prometen y cómo funcionan:** «50 prompts para que ChatGPT escriba como un humano». Pagas por un documento con frases preparadas que copias y pegas según el tipo de texto que necesites. **[HIP: categoría frecuente en el mercado; no aparece con nombre en el corpus]**

**b) Desventajas:** Así que pensaste que con el prompt perfecto se acababa el problema. El primer inconveniente es práctico: tienes que buscar el prompt adecuado, copiarlo, pegarlo y adaptarlo **cada vez**. Es exactamente el ciclo de pestañas que tanto cansa (A21). El segundo es de fondo: un prompt es una petición puntual, y la IA vuelve a su voz por defecto en cuanto la conversación avanza (A19). El tercero: esos prompts están escritos para «un humano» genérico, no para ti, y lo que buscas no es sonar a un humano cualquiera, sino a ti (A4, A22). Y el cuarto: muchos de esos packs incluyen precisamente las instrucciones en negativo («no uses…») que, según cuentan los propios usuarios, pueden empeorar el resultado (E12). Pagas por cincuenta formas de repetir lo mismo.

**c) Por qué lo nuestro es mejor:** Y por eso no te damos cincuenta prompts. Te damos una sola configuración, la tuya, que se queda puesta. No tienes que acordarte de qué prompt toca para qué texto ni pegar nada en cada mensaje. Abres tu ChatGPT y ya escribe como tú, sea un email, un mensaje al equipo o un post. Si un día necesitas un tono más formal, se lo pides en una línea y lo hace sin dejar de sonar a ti, porque la base ya es tu voz. Es menos cosas que recordar, menos pasos y más resultado. Lo que buscabas no era una colección: era dejar de pensar en esto.

### 7. Los parafraseadores y correctores con IA

**a) Qué prometen y cómo funcionan:** herramientas que reformulan tus frases o corrigen tu gramática y tu estilo con IA para que «quede mejor» o «más profesional».

**b) Desventajas:** Te entiendo, todos hemos pasado por eso: quieres que el texto quede un poco más pulido y le das al botón de «mejorar». El problema es que «mejorar», para una IA, suele significar **hacerlo sonar más a IA**. Una persona usó ChatGPT solo para mejorar la gramática de su propio texto y acabó marcada como IA (B12). Otra temía consecuencias incluso habiéndolo usado solo para la ortografía (B13). En el trabajo pasa lo mismo: hay jefes y departamentos de Recursos Humanos que pasan textos humanos por IA para «editarlos» y los devuelven con un tono impersonal y artificial (A8, C9). Un escritor contaba que su editor le cambió «serene» por «tranquil» y lo empeoró todo (E47). Estas herramientas no saben cuál es tu voz. Tiran hacia el «correcto estándar», que hoy es justo lo que suena a máquina.

**c) Por qué lo nuestro es mejor:** No digo que corregir esté mal. Digo que corregir sin saber cómo hablas te borra. Nuestra configuración funciona al revés: primero le enseñas a tu IA cuál es tu forma de escribir y, a partir de ahí, cualquier corrección o mejora respeta esa forma. Corrige las faltas, pero no te cambia el «un abrazo» por «Atentamente». Ordena la idea sin convertirla en un folleto. Y el PDF te enseña a detectar cuándo una «mejora» ha introducido las huellas de la máquina, para que no se te cuelen. Mereces una herramienta que te pula sin borrarte.

### 8. Los cursos largos de IA o de «prompt engineering»

**a) Qué prometen y cómo funcionan:** formaciones de varias horas o semanas para «dominar la IA», aprender a hacer prompts profesionales, automatizar tareas y escribir mejor con ChatGPT.

**b) Desventajas:** Vamos, seamos sinceros: tú no quieres dominar la IA. Quieres que tus emails no suenen a robot. Un curso largo te hace pasar por diez módulos que no necesitas (automatizaciones, imágenes, hojas de cálculo) para llegar, con suerte, a una lección sobre el tono. Quien se define como poco técnico describe la experiencia de prompts, opciones y ajustes como algo que avanza más rápido de lo que puede asimilar (A36), y otra persona contaba que, incluso tras dedicar mucho tiempo a aprender, seguía confusa con cómo conseguir el tono que quería (A35). Además, muchos de esos cursos están pensados para usuarios avanzados, con jerga, pantallas que no reconoces y herramientas de código. Y luego está el clásico: el curso se queda a medias en la carpeta de descargas. Mucho tiempo, mucha teoría, y el email de mañana sigue sonando igual.

**c) Por qué lo nuestro es mejor:** Lo nuestro hace **una sola cosa** y la hace bien: que tu IA escriba como tú. No tienes que aprender la IA, tienes que enseñarle a la IA cómo eres. Es un PDF que se lee en un rato y explica por qué suena a máquina, más una guía que te lleva paso a paso, en una sesión, a dejarlo configurado. Sin módulos de relleno, sin jerga y sin herramientas de programación. Lo terminas en una tarde y el lunes ya lo estás usando. Es la diferencia entre apuntarte a la autoescuela para aprender mecánica o que alguien te ajuste el asiento y los espejos y te deje conducir.

### 9. Contratar a un redactor o ghostwriter

**a) Qué promete y cómo funciona:** pagas a un profesional para que escriba tus textos importantes (posts, propuestas, emails delicados) con un estilo cuidado.

**b) Desventajas:** Ahora, no me malinterpretes: un buen redactor vale su peso en oro para ciertos textos. Pero para el día a día no tiene sentido. Primero, por el precio: pagar a alguien por cada email o mensaje no es viable, y una sola hora suya cuesta más que esta guía. Segundo, por los tiempos: el email al cliente tiene que salir hoy, no cuando el redactor tenga hueco. Tercero, y esto es lo curioso: **tampoco sabe cómo hablas tú** al principio. Necesita tiempo, ejemplos y correcciones para pillarte el tono. Y cuarto, en el propio corpus aparece el reverso: ghostwriters que ven cómo sus clientes pasan después su texto por ChatGPT y lo convierten en *slop* (C5), y copywriters que acaban dimitiendo al ver su trabajo convertido en IA (C6). Es decir, ni siquiera pagando un profesional tienes garantizado que lo que llega al cliente suene a ti.

**c) Por qué lo nuestro es mejor:** Lo que tienes con esta configuración es, en cierto modo, tu propio redactor que ya conoce tu voz, disponible a las once de la noche y por el precio de una comida, una sola vez. No sustituye a un profesional para una campaña de lanzamiento, pero sí para el 95 % de lo que escribes a diario. Y como la voz que le enseñas es la tuya, nadie la «traduce» por el camino: lo que sale es lo que tú dirías. Para el email de cada día no necesitas un escritor. Necesitas que tu herramienta deje de escribir como un extraño.

### 10. Las herramientas técnicas para programadores (APIs, agentes, clonadores de estilo)

**a) Qué prometen y cómo funcionan:** soluciones para usuarios avanzados que conectan la IA por API, crean agentes o «entrenan» a la IA con cientos de textos tuyos para clonar tu estilo, y que normalmente exigen herramientas de código o configuraciones complejas.

**b) Desventajas:** Si eso te suena a chino, es normal: está hecho para otra gente. Exigen saber cosas que tú no tienes por qué saber (claves de API, terminales, archivos de configuración) y suelen costar dinero por uso. Y ni siquiera garantizan el resultado. Una persona contaba que, tras probar humanizadores, clonadores de voz y prompts de estilo durante una semana, miraba el resultado y sabía que tendría que reescribirlo prácticamente entero (A30). Otra describía a un amigo que alimentó a ChatGPT, «desesperadamente», con cientos de emails para que imitara el estilo de su jefe (E18). Mucho esfuerzo técnico para un resultado incierto. Y si algo falla, ¿a quién le preguntas? Para ti, una solución que necesita un manual técnico es una solución que no vas a usar.

**c) Por qué lo nuestro es mejor:** Nosotros tomamos la idea útil de esas herramientas (darle a la IA información real sobre cómo escribes) y la llevamos al sitio donde tú ya estás: la ventana de chat de ChatGPT o de Claude que usas cada día. Sin código, sin claves y sin instalar nada técnico. Te guiamos para que describas tu voz con tus palabras y unos cuantos textos tuyos, y para dejarlo configurado en tu propia cuenta. Toda la ventaja de «personalizar tu IA», sin la parte que te dejaba fuera. Porque usar bien la IA no debería ser solo para los que saben programar.

---

## Segmentación por motivaciones

### Pregunta crítica: ¿hay dentro de este mercado 2 o más grupos con motivaciones de compra claramente distintas?

**Respuesta: SÍ.** Hay al menos **dos segmentos con motivaciones claramente distintas** en el corpus, y **un tercero probable** que el corpus no permite caracterizar. He revisado con rigor los dos ejes candidatos que me indicaron (uso NEGOCIO frente a PERSONAL y confianza técnica alta frente a baja) y el resultado **no coincide exactamente** con esas etiquetas. La divisoria real es otra: **quién es el juez del texto** (una persona o un algoritmo).

### Análisis de los ejes candidatos

**Eje 1, NEGOCIO frente a PERSONAL (etiquetas del corpus):**
- La etiqueta [PERSONAL] del corpus (43 entradas) **no es un segmento homogéneo**. Unas 21 de las 43 son **académicas o de admisiones** (estudiantes ante Turnitin o GPTZero, candidatos a Medicina, Odontología, UCAS, *fellowships*). Las demás se reparten entre **escritores y creativos acusados** (novela, ensayo, relato), **voces de juez en relaciones personales** (la amiga, el amigo, el hermano, el match de la app de citas) y comentaristas.
- El **adulto de 35 a 60 años que usa la IA para su vida personal** (mensajes a la familia, felicitaciones, pésames, reclamaciones, comunidad de vecinos, grupo del colegio), que encaja con la definición del producto («no tienen que tener negocio propio»), **prácticamente no aparece como emisor**. Solo aparece como **juez** (C18, C19, B3, C20). **[DATO INSUFICIENTE]**
- Conclusión: NEGOCIO frente a PERSONAL-académico **sí** divergen claramente. NEGOCIO frente a PERSONAL-adulto **probablemente** divergen, pero no hay datos.

**Eje 2, confianza técnica alta frente a baja:**
- Ambos grupos comparten **la misma motivación** (que no se note, que suene a uno mismo) y **el mismo detonante** (comentario o hartazgo). Divergen en **las barreras** (miedo a no saber frente a «ya lo probé») y en **la ruta de decisión** (el técnico compara con su propio *system prompt*; el no técnico busca seguridad).
- Conclusión: **no son segmentos de motivación distintos**. Son **variantes de barrera dentro del mismo segmento**, ya cubiertas por los arquetipos «La que firma con su nombre», «El veterano desbordado» y «El que ya probó las instrucciones». El usuario de confianza técnica **muy alta** (el que domina los *system prompts*) es en la práctica **anti-persona** («esto me lo hago yo en diez minutos»).

### Segmentos detectados

**Segmento 1 — «El que firma con su nombre ante personas»** (PRINCIPAL; es el que desarrolla este documento)
- Adultos que usan la IA para textos de trabajo que leen jefes, clientes y compañeros. **Su juez es una persona.**
- **Detonante:** el comentario de una persona («¿esto lo has escrito con ChatGPT?») o el hartazgo de reescribir.
- **Éxito:** que nadie diga nada; mandarlo a la primera; que suene a él.
- **Barreras:** ansiedad técnica, desconfianza hacia la categoría, «ya lo probé».
- **Ruta:** rápida, basada en la confianza, pago único, demostración visual.
- **Peso en el corpus:** ≈ 42 emisores directos, más ≈ 37 jueces que describen su amenaza social. Es **el segmento con más base y más coherencia**, y el único que encaja a la vez con la definición del producto y con el corpus.

**Segmento 2 — «El que tiene que pasar el detector»** (estudiantes y candidatos; también los productores de contenido masivo)
- **Su juez es un algoritmo** (Turnitin, GPTZero, ZeroGPT, Pangram), y detrás de él una autoridad (profesor, Dean, comité de admisiones).
- **Detonante:** un porcentaje, un cero, una acusación formal, una fecha de entrega.
- **Éxito:** un número (0 % IA).
- **Barreras:** que no le garanticen el número; precio por volumen.
- **Ruta:** comparar humanizadores, probar en varios detectores, Trustpilot y Reddit.
- **Peso en el corpus:** ≈ 43 entradas (casi todo el bloque D y parte del B).
- **Divergencia con el Segmento 1:** en **todo**: detonante, criterio de éxito, barreras y ruta.

**Segmento 3 (probable, no caracterizable con los datos) — «El adulto que escribe para su vida personal»**
- Adultos de 35 a 60 años que usan ChatGPT para mensajes personales o de su vida civil. **Su juez es una persona querida** (familia, amigos) o una institución (administración, colegio).
- **Hipótesis de divergencia:** el detonante sería un comentario de un ser querido («qué formal», «pareces un robot»); el éxito, «que suene cariñoso / que suene a mí»; la barrera, el pudor de reconocer que usa IA para algo íntimo; la ruta, recomendación de un conocido o un vídeo de YouTube o Facebook.
- **Peso en el corpus:** 0 emisores directos; solo jueces (C18, C19, C20, B3).

### Dónde divergen

| Dimensión | Segmento 1 (personas, trabajo) | Segmento 2 (detector) | Segmento 3 (personal adulto, HIP) |
|---|---|---|---|
| Detonante | Comentario de jefe o cliente; hartazgo | Porcentaje / cero / acusación | Comentario de un ser querido |
| Definición de éxito | Que nadie note nada; ahorrar tiempo | 0 % en el detector | Sonar cercano y auténtico |
| Barrera principal | Ansiedad técnica + desconfianza | Que no garanticen el número | Pudor + ansiedad técnica |
| Ruta de decisión | Rápida, confianza, demostración visual | Comparativa de herramientas y pruebas en detectores | Recomendación personal, vídeo |
| Encaje con el producto | **Alto** | **Bajo** (no puede garantizar detectores) y **conflicto ético** | Probablemente alto (por verificar) |

### Recomendación

1. **Construir un único buyer persona ahora, para el Segmento 1.** Es el que desarrolla este documento: es mayoritario entre los compradores reales según el corpus, encaja con el producto y su motivación dominante («usar la IA sin que se note») es coherente.

2. **NO construir un buyer persona para el Segmento 2 (detector).** **Recomendación explícita: tratarlo como Anti-Persona** (ya está hecho en esta sección). Motivos: (a) el producto **no puede** prometer resultados en detectores, que el propio corpus demuestra que son inconsistentes (B18: 0 %, 40 % y 100 % para el mismo texto), así que generaría devoluciones y malas reseñas; (b) posicionarse para él empuja el producto a la categoría desprestigiada de los humanizadores; (c) supone un riesgo ético y reputacional (ayudar a hacer pasar trabajo académico de IA como propio). **Importante:** si el copy no lo excluye activamente, este segmento llegará igual, porque es muy activo buscando. Los filtros del Anti-Persona son obligatorios.

3. **SÍ RECOMIENDO un segundo buyer persona, pero CONDICIONADO a nuevo research: el Segmento 3 (el adulto que escribe para su vida personal, 35-60 años, baja confianza técnica).** Justificación: (a) la definición del producto lo incluye explícitamente («no tienen que ser copywriters ni tener negocio propio»); (b) es probablemente grande en el mercado hispanohablante, donde WhatsApp y los mensajes personales tienen mucho peso **[HIP]**; (c) su detonante, su criterio de éxito y su barrera **probablemente** son distintos (un juez afectivo en vez de profesional, el pudor de lo íntimo, una búsqueda vía recomendación o vídeo) y un único perfil de trabajo **podría alienarle** («esto es para gente con clientes y jefes»). **Pero con el corpus actual sería un persona inventado**: no hay ni una sola voz emisora de este segmento. **Research mínimo antes de construirlo:** (i) minar grupos de Facebook y comentarios de YouTube en español sobre «ChatGPT para escribir mensajes / cartas / felicitaciones»; (ii) 6-8 entrevistas con usuarios de 40 a 65 años que usan ChatGPT para asuntos personales. Si ese research confirma la divergencia de detonante y de barrera, **merece un persona separado**. Si muestra que el detonante y la barrera son los mismos que en el Segmento 1 (miedo a que se note + ansiedad técnica), basta con **añadir escenas personales** al persona actual.

4. **Mientras tanto, para no alienar al Segmento 3**, el copy del Segmento 1 debe evitar que el producto parezca exclusivamente para gente con clientes y jefes. Hay que incluir al menos una escena personal (la felicitación que salió «qué formal») como ejemplo secundario y no hablar de «tu negocio» en el titular.

---

## Validación final del análisis (Quality Gate)

| # | Criterio | Estado | Justificación (una línea) |
|---|---|---|---|
| 1 | **Mass Desire dominante** | **CUMPLE** | Una sola («usar la IA sin que se note»), dimensionada (U 7, SP 8, S 8) y justificada frente a «ahorrar tiempo reescribiendo» y «recuperar mi voz» (y frente a «pasar el detector»). |
| 2 | **4 fuerzas de Moesta** | **CUMPLE** | Palanca crítica única: **reducir la ansiedad** (8/10), justificada frente a las otras tres, con la ecuación 12 contra 14 y cómo invertirla. |
| 3 | **Customer Job Statement** | **PARCIAL** | Construido con situación, tres capas y resultado visual, y anclado en el corpus. Pero el **vocabulario nativo en español es HIP** (no hay ni una voz en español), así que conviene validarlo antes de usarlo sin editar como primera línea. |
| 4 | **Granularidad emocional** | **PARCIAL** | Todas las frases en primera persona llevan anclaje temporal, situacional o sensorial y etiqueta de procedencia. Pero **muchos anclajes sensoriales son HIP**: el corpus tiene pocas sensaciones corporales del emisor adulto. Una frase (Herida 1) va marcada [DATO INSUFICIENTE: falta un anclaje sensorial]. Se han descartado explícitamente las tibias. |
| 5 | **Predicción del lector** | **CUMPLE** | Documentada por canal (redes, landing, email, vídeo corto), con contaminación, emoción objetivo granular y decisión justificada: **romper la predicción**. |
| 6 | **Awareness + Sophistication** | **CUMPLE** | Problema consciente (45 %) con franja de solución consciente (35 %), y sofisticación de nivel 4 (anglófono) o 3-4 (hispano), con ejemplos concretos del mercado (humanizadores, listas, prompts, el *rulebook* de E53). Los porcentajes son HIP declarada. |
| 7 | **Disparadores de Expulsión** | **CUMPLE** | Diez, específicos de este mercado («100 % humano», «plugin» en la entrada, porcentajes de detector, ridiculizar al que copia y pega, mencionar la edad, una landing que suene a IA…), no genéricos. |
| 8 | **Anti-Persona** | **CUMPLE** | Construido para autoexcluir: frases-filtro literales («Esto no es para engañar a un detector…») y requisitos de implicación. |
| 9 | **Test del headline ya** | **CUMPLE** | Hay material para un headline ultraespecífico ahora mismo. Ejemplos: «¿Por qué todo lo que te escribe ChatGPT suena a ChatGPT? (Y por qué pedirle que no lo haga lo empeora)» o «A nadie le molesta que uses ChatGPT. Le molesta que se note. Así se arregla, una vez, sin programar». **Matiz:** la redacción final en español conviene validarla con research en español, pero el headline es escribible. |
| 10 | **Test del Big Idea** | **CUMPLE** | **«Lo que te delata no es que uses IA; es que tu IA todavía no sabe cómo hablas tú.»** No describe funcionalidades, deriva de la Mass Desire y del CJS e incluye el mecanismo (enseñarle una vez) sin nombrar el formato. |
| 11 | **Procedencia y ponderación del dato** | **CUMPLE** | Declarados el tipo de fuente, el tipo de participante (recién llegado ≈ 15 %, ocasional ≈ 45-50 %, insider ≈ 35-40 %) y el rol (emisor, juez, acusado…). Advertida la infrarrepresentación del comprador objetivo, el sesgo de idioma y nacionalidad y el de soltura técnica. Marcadas como [FUENTE ÚNICA] y como mensajería de competidor las entradas correspondientes. |

**Recuento:** 9 CUMPLE, 2 PARCIAL, 0 NO CUMPLE. Los criterios 9 y 10 se **cumplen**, así que **el análisis está listo para empezar a redactar copy**, con las cautelas siguientes.

### Dónde falta material y qué research lo completaría

Aunque no hay tres NO CUMPLE, los dos PARCIAL y las áreas de baja confianza apuntan a las mismas lagunas, que conviene cerrar **antes de escalar la inversión en publicidad**:

1. **Vocabulario nativo en español** (afecta a los criterios 3 y 4, y a todo el copy). → Minar comentarios de YouTube en español y grupos de Facebook sobre ChatGPT. Recoger las frases literales con las que el hispanohablante describe que algo «suena a ChatGPT» y los tics que **él** detecta en español.
2. **Anclajes sensoriales del emisor adulto** (criterio 4, Interoceptivos, Herida). → 8-12 entrevistas con el target, con preguntas del tipo: «¿Qué sentiste exactamente, físicamente, cuando el cliente te preguntó si lo habías escrito con ChatGPT?».
3. **La sensación de «la tecnología me ha superado»** (residual en el corpus y central en el producto). → Las mismas entrevistas y los mismos grupos de Facebook. Hay que verificar si es un motor de compra o solo un tono.
4. **El deseo explícito de «configurar una vez»** ([FUENTE ÚNICA], E53). → Test A/B de anuncios: «configúralo una vez» frente a «deja de reescribir» frente a «que no se note», para medir qué ángulo tracciona en frío.
5. **Segmento 3 (uso personal adulto).** → Ver la recomendación de Segmentación.
6. **Disposición a pagar y forma de pago** (29 € como pago único). → Encuesta corta o test de precio en la landing (29 € frente a 19 €).
7. **Validación técnica del producto frente a la objeción P-2** («ya probé las instrucciones»). → Antes de lanzar, el creador debe comprobar que la configuración **resiste la degradación en conversaciones largas** y que está construida **en positivo**, sobre la voz real del usuario. Si no es así, la promesa central fallará igual que le falló a A26 y A27, y ningún copy lo compensará.

### Bloques que deben revisarse antes de la redacción definitiva

- **Customer Job Statement y «La frase exacta del segundo anterior»:** revalidar el vocabulario con research en español.
- **Mecanismos Interoceptivos y Un Día en la Vida:** sustituir los anclajes sensoriales HIP por anclajes reales de las entrevistas.
- **Objeciones E-4 y P-5, y Restricción 11:** completar con los requisitos técnicos reales del producto (planes, cuentas de empresa, móvil, qué hace exactamente el plugin con los datos y cómo se deshace).
- **Restricción 13 (fórmula de desafío personal):** solo puede usarse cuando el creador haya hecho y documentado de verdad la prueba «a ciegas» que describe.
- **Prueba social:** todo el documento asume **cero testimonios**. En cuanto existan, priorizar los de personas no técnicas de 40-60 años con su escenario concreto y revisar el bloque «Tipo de prueba».


