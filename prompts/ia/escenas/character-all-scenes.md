# Escenas completas (todas en un solo documento)

Archivo resumen que reúne las 8 escenas del personaje con props clave, ajustes cinematográficos resumidos para RED Komodo y ARRI Alexa, y un prompt IA por escena. Al final están las medidas técnicas en JSON.

---

## Personaje — referencia rápida
- Altura total: 1700 mm (170 cm). Cabeza = 220 mm (referencia de escala).
- Rasgos: rostro ovalado, ojos almendrados (iris centrados), nariz recta y punta ligeramente redondeada, mandíbula suave y mentón moderado.
- Usa las medidas detalladas al final para modelado/rigging/vestuario.

---

## 1) Amanecer frente al espejo
- Escenario: baño pequeño, luz matinal suave.
- Props clave: espejo 800×600 mm; lavabo 560×420 mm; toalla 700×1400 mm.
- Cinemática (resumen)
  - RED Komodo: 6K, 24 fps, 50 mm T1.5, ISO 800, 180°.
  - ARRI Alexa: 4.5K, 24 fps, 35–50 mm T1.3, LogC4, ISO 800.
- Prompt IA: "Morning bathroom portrait, soft warm side key, 50mm, shallow DOF, natural skin."

## 2) Calle lluviosa — reflexión en movimiento
- Escenario: avenida al anochecer, farolas y reflejos en asfalto.
- Props clave: paraguas transparente Ø900 mm; trench 1100 mm.
- Cinemática (resumen)
  - RED: 6K, 35 mm, ISO 800–1250, T2.2–T2.8.
  - ARRI: LogC4, 35 mm anamorphic opcional, ISO 800.
- Prompt IA: "Rainy city walk, reflective asphalt, trench coat, cinematic bokeh."

## 3) Sesión de estudio — catálogo/identidad
- Escenario: estudio con fondo neutro.
- Props clave: seamless 3×4 m; softbox 1.5 m.
- Cinemática (resumen)
  - RED: 6K, 85 mm, ISO 800, T2.0.
  - ARRI: 85 mm Master Prime, LogC4.
- Prompt IA: "Studio headshots, neutral background, razor-sharp eyes, natural pores."

## 4) Sala de reuniones tensa
- Escenario: sala de juntas moderna con mesa de vidrio.
- Props clave: mesa vidrio 2000×1000 mm; pantalla 75".
- Cinemática (resumen)
  - RED: 6K, 35–50 mm, ISO 800.
  - ARRI: 35 mm MP, LogC4, ISO 800.
- Prompt IA: "Boardroom presentation, confident posture, glass reflections, filmic contrast."

## 5) Noche íntima — confesión
- Escenario: sala con lámpara cálida y copa de vino.
- Props clave: lámpara 420 mm; copa 250 ml.
- Cinemática (resumen)
  - RED: 6K, 50–85 mm, ISO 800, T1.8.
  - ARRI: 65 mm, LogC4, ISO 800.
- Prompt IA: "Warm lamp-lit close-up, tender expression, soft highlights on eyes."

## 6) Claro del bosque — encuentro místico
- Escenario: bosque al amanecer con niebla y luz radial.
- Props clave: piedra luminosa ≈450×300 mm; capa 1400 mm.
- Cinemática (resumen)
  - RED: 6K, 35 mm, ISO 800–1000.
  - ARRI: 35–40 mm anamorphic opcional, LogC4.
- Prompt IA: "Forest clearing, glowing stone, soft mist, rim-lit silhouette."

## 7) Medbay (ciencia ficción)
- Escenario: módulo médico con escáner facial holográfico.
- Props clave: panel scanner Ø800 mm; camilla 2000×650 mm.
- Cinemática (resumen)
  - RED: 6K, 50 mm macro, ISO 800, T4.0.
  - ARRI: 65 mm/macro, LogC4, ISO 800.
- Prompt IA: "Sci‑fi facial scan, holographic overlays with measurements, cool clinical lighting."

## 8) Anuncio / comercial de belleza
- Escenario: set high-key, fondo blanco.
- Props clave: frasco 60×120 mm; pedestal acrílico Ø200 mm.
- Cinemática (resumen)
  - RED: 6K, 85–100 mm macro, ISO 800, T2.8–T5.6.
  - ARRI: 85–100 mm, LogC4.
- Prompt IA: "High-key beauty close-up, product beside face, macro skin detail."

---

## Medidas técnicas del personaje (resumen JSON)
{
  "units": "mm",
  "height_total": 1700,
  "head_height": 220,
  "head_width_bizygomatic": 140,
  "forehead_height": 65,
  "nasal_length": 50,
  "nasal_bridge_width": 18,
  "alar_width": 36,
  "lip_width": 50,
  "upper_lip_height": 8,
  "lower_lip_height": 10,
  "cupids_bow_radius": 6,
  "chin_height": 25,
  "jaw_width_gonion_to_gonion": 120,
  "chin_width_base": 50,
  "eye_horizontal_width_palpebral": 32,
  "intercanthal_distance_medial_to_medial": 32,
  "pupil_center_to_center": 64,
  "iris_diameter_visible": 11,
  "upper_eyelid_height_from_pupil": 12,
  "neck_length_jaw_to_clavicle": 95,
  "shoulder_width_acromion": 410,
  "chest_circumference": 920,
  "arm_length_shoulder_to_wrist": 590,
  "hand_length_wrist_to_middle_tip": 185,
  "foot_length_estimate_mm": 270
}