# Prompts optimizados para Runway Gen-2 / Pika Labs (8 escenas)

Parámetros generales (usar en cada prompt): aspect_ratio=16:9, resolution=3840x2160, duration=8s, fps=24. Seed sugerido: 42 (puedes variar).
Negatives comunes: lowres, deformed, extra limbs, bad anatomy, text, watermark.

1) Amanecer frente al espejo
Prompt (Runway/Pika):
"Cinematic morning bathroom portrait of an adult with oval face, almond eyes centered, straight nose and soft jaw. Shot emulating RED Komodo 6K 50mm T1.5 look, warm side key 3200K, shallow depth of field, mirror 800x600mm visible, soft natural skin detail, Kodak 2383 grade. aspect 16:9, 3840x2160, 8s, seed=42. --neg lowres,deformed,bad anatomy,watermark"

2) Calle lluviosa — reflexión en movimiento
"Rainy city walk at dusk, subject with balanced oval face under transparent umbrella Ø900mm, trench coat, reflective wet asphalt, cinematic bokeh, emulating ARRI Alexa LogC4 + 35mm anamorphic look, teal-orange grade, 16:9 3840x2160 8s seed=43 --neg lowres,deformed,bad anatomy"

3) Sesión de estudio — catálogo
"Studio headshot series, neutral seamless background, subject with almond eyes and centered iris, razor-sharp eyes, natural pores visible, emulating RED 6K 85mm portrait lens, softbox key, high detail skin, 16:9 3840x2160 8s seed=44 --neg cartoon,lowres"

4) Sala de reuniones tensa
"Boardroom presentation cinematic shot, glass table reflections, subject confident posture, shallow depth but visible environment, ARRI Alexa look 35-50mm, cool room light with warm face key, 16:9 3840x2160 8s seed=45 --neg bad anatomy,watermark"

5) Noche íntima — confesión
"Warm lamp-lit close-up in living room, tender expression, soft highlights on eyes, wine glass visible, emulating RED 6K 50mm T1.8, cozy tungsten key 2800K, high skin detail, 16:9 3840x2160 8s seed=46 --neg lowres,deformed"

6) Claro del bosque — encuentro místico
"Forest clearing at dawn with soft mist, glowing stone 450x300mm, rim-lit silhouette approaching, serene expression, emulating cinematic ARRI/RED grade, soft bloom, 16:9 3840x2160 8s seed=47 --neg bad anatomy,lowres"

7) Medbay (ciencia ficción)
"Sci-fi medical bay facial scan, holographic overlays showing measurements (intercanthal 32mm, pupil center 64mm), cool clinical blue lighting, subject calm, emulating RED 6K 50mm macro look, crisp detail, 16:9 3840x2160 8s seed=48 --neg artifacts,lowres"

8) Anuncio / comercial de belleza
"High-key beauty close-up, subject with oval face, subtle cupid's bow, product bottle 60x120mm next to face, macro-level skin detail, emulating RED 6K 85-100mm macro, soft specular highlights, clean white background, 16:9 3840x2160 8s seed=49 --neg lowres,cartoon"

Notas de uso
- Para Runway: pegar prompt en campo principal; ajustar seed y usar negative prompts si aparecen errores.
- Para Pika: adaptar sintaxis según interfaz; incluir "--neg" negative list si disponible.
- Itera 2–4 renders por escena y selecciona mejor take para montaje.
