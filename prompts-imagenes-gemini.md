# PROMPTS PARA GENERAR IMÁGENES CONSISTENTES — HYDROCELL

> Pegar cada prompt en **Gemini** (https://gemini.google.com) o **Google AI Studio** (https://aistudio.google.com) usando el modelo **Imagen 3** o pidiéndole a Gemini que genere la imagen.
>
> **Truco para consistencia:** todos los prompts comparten el mismo "STYLE GUIDE" al inicio. NO lo modifiques entre prompts. Eso es lo que garantiza que las imágenes se sientan parte de la misma marca.

---

## STYLE GUIDE (copiar EXACTAMENTE al inicio de cada prompt)

```
STYLE: professional automotive photography, cinematic lighting,
clean modern aesthetic, brand palette of teal-cyan (#00b9b5, #3bb4c3)
and emerald green (#4EBD8D) with soft natural light, shallow depth
of field, premium look, photorealistic, 16:9 aspect ratio,
no text or watermarks, no logos.
```

---

## IMAGEN #1 — Hero página Descarbonización

**Contexto:** Hero principal de "Descarbonización de motores con tecnología de hidrógeno"
**Archivo original (perdido):** `4902689f-0248-4136-a163-68e4851787ab_...jpeg`

```
[STYLE GUIDE]

Subject: A modern car engine bay viewed from above, with a faint
glowing cyan-teal mist (representing hydrogen gas) flowing into
the intake. Clean professional auto-shop environment. The engine
looks well-maintained and slightly futuristic. Soft hydrogen-blue
glow accents around the intake manifold. Hands of a mechanic in
clean gloves visible at the edge holding a diagnostic tool. The
overall mood is "clean technology meets automotive precision."
```

---

## IMAGEN #2 — "¿En qué consiste el servicio?"

**Contexto:** Explicación del proceso de descarbonización con hidrógeno
**Archivo original:** `1b50bbf4-5c52-48b7-87be-14510cde1366_...jpeg`

```
[STYLE GUIDE]

Subject: Close-up of a hydrogen-generating machine (HHO generator)
connected by transparent tubing to a car's intake. The machine
has a teal-cyan accent light. Background slightly blurred showing
the engine bay of a sedan. Bubbles visible inside the device's
water chamber. Mood: scientific, clean, safe, professional.
No people, no text.
```

---

## IMAGEN #3 — "Quiénes somos" (foto del equipo / taller)

**Contexto:** Imagen institucional de HYDROCELL S.A.S.
**Archivo original:** `758d6abf-82f8-418d-ba1a-3cbde9a43b02_...jpeg`

```
[STYLE GUIDE]

Subject: A professional automotive workshop in Medellín, Colombia.
Three Latino mechanics in matching clean teal-cyan polo shirts
working confidently around a sedan that has its hood open. One is
checking a tablet/diagnostic device, another is connecting a hose
to the engine, the third stands smiling at the camera. Bright
modern workshop with white walls, organized tools, natural
daylight from large windows. Mood: trustworthy, expert,
approachable.
```

---

## IMAGEN #4 — "Análisis de gases (HC)"

**Contexto:** Explicación de la medición de hidrocarburos en gases de escape
**Archivo original:** `4fe38446-6e9a-4104-a7d9-57dfe2c9ca70_...jpeg`

```
[STYLE GUIDE]

Subject: Close-up of a professional gas analyzer probe inserted
into a car's exhaust pipe. The analyzer's digital screen visible
slightly out of focus showing green numbers and percentages.
Hands of a technician in nitrile gloves holding the probe. Faint
exhaust vapor in the air. Subtle teal-cyan reflection on the
chrome of the exhaust. Mood: precise, technical, environmentally
conscious. No readable text on the screen.
```

---

## IMAGEN #5 — "¿Cada cuánto? — Limpieza cuerpo aceleración"

**Contexto:** Frecuencia recomendada de mantenimiento (cada cambio de aceite)
**Archivo original:** `04b8b9a2-c2c7-48cf-a4fb-fd91ea50220a_...jpeg`

```
[STYLE GUIDE]

Subject: An odometer/dashboard close-up showing a digital
mileage display around 10,000 km, with a soft teal-cyan glow.
Modern car interior, slightly blurred steering wheel in
foreground. Conveys the idea of scheduled maintenance.
Mood: clean, modern, precise, friendly. No readable brand
names on the dashboard.
```

---

## IMAGEN #6 — "Desinfección Profunda de Cojinería y Tapicería"

**Contexto:** Servicio principal de desinfección interna del vehículo
**Archivo original:** `78d398f8-554a-41b9-9a8e-dc56f9ec17fb_...jpeg`

```
[STYLE GUIDE]

Subject: Pristine clean car interior — gray-and-black leather
seats sparkling clean, sunbeam through windshield, a subtle
teal-cyan vapor mist rising from the air conditioning vents
(representing hydrogen-vapor sanitization). The cabin looks
freshly detailed, smelling new. View from the rear seat looking
forward. Mood: fresh, sanitized, premium, healthy.
```

---

## IMAGEN #7 — "Beneficios del servicio" (desinfección)

**Contexto:** Beneficios para personas alérgicas, niños, mascotas
**Archivo original:** `ab4aecae-a596-435c-a656-5e9ef8f54037_...jpeg`

```
[STYLE GUIDE]

Subject: A happy Latino family — mother, father, two children
around 6-9 years old — getting into a clean modern car. The mom
is smiling at the kids buckling up in the back seat. Sunny day,
soft natural light. The interior of the car looks immaculate.
Subtle teal-cyan accent in the scene (a hint in the sky reflection
or the car's color). Mood: safe, healthy, family-friendly,
trustworthy.
```

---

## TIPS PARA MÁXIMA CONSISTENCIA EN GEMINI

1. **Genera todas en la misma sesión** — Gemini mantiene contexto y aprende tu estilo a medida que avanzas.
2. **Después de cada imagen, dile:** *"Make the next image with the same lighting, color palette and photographic style as this one"*.
3. **Si una sale fuera de tono**, di: *"Match the teal-cyan accent and warm natural lighting from the previous image"*.
4. **Pide variaciones** de la misma imagen para tener 2-3 opciones por slot.
5. **Formato exportación:** descarga en PNG o JPG y guárdalas en `/Users/macbook/Documents/hydrocell/imagenes-generadas/`.

## ALTERNATIVAS GRATUITAS si Gemini no genera imágenes

- **Google AI Studio** (aistudio.google.com) — modelo `imagen-3.0-generate-002`
- **Microsoft Designer / Bing Image Creator** (bing.com/create) — usa DALL-E 3 gratis
- **Leonardo.ai** — créditos diarios gratis
- **Krea.ai** — gratis con cuenta

Para máxima consistencia con foto-realismo, **Imagen 3** o **DALL-E 3** suelen dar los mejores resultados.
