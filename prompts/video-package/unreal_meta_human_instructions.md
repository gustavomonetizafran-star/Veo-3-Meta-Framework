# Unreal + MetaHuman: instrucciones resumidas (uso técnico)

Objetivo
Crear un MetaHuman que reproduzca las medidas del personaje (head = 220 mm, ojos 32 mm, intercanthal 32 mm, etc.) y montar las 8 escenas en Unreal Engine con Sequencer para renders cinematográficos 4K.

1) Crear MetaHuman base
- Abre Quixel Bridge > MetaHuman Creator.
- Selecciona template masculino/femenino cercano y ajusta proporciones:
  - Head height: target 220 mm (usar escala relativa en la ficha del head).
  - Intercanthal (pupils center-to-center): 64 mm → ajustar eye spacing hasta proporción.
  - Eye palpebral width: 32 mm.
  - Nose length: 50 mm; bridge width ~18 mm; alar width 36 mm.
  - Jaw width gonion-gonion: 120 mm; chin height 25 mm.
- Exportar MetaHuman a Unreal (Live Link + Bridge). Exporta con morph targets/blendshapes.

2) Skin shader y SSS
- Usar Material de piel PBR con SSS:
  - SSS profile: 3 layers (epidermis, dermis, subdermal).
  - SSS radius: [0.2, 0.6, 1.0] (ajustable en unidad de escena).
  - Specular: 0.5, roughness base 0.25, micro-surface normal maps para poros.
- Usar mapas: base color, normal, roughness, subsurface color, AO.

3) Rigging y expresiones
- Exportar FBX con blendshapes para labios y ojos. Configurar ARKit shape set si usar captura facial.
- Verificar control de párpados, iris, y micro-gestos (blink, squint, smile subtle).

4) Escenas y Sequencer (ajustes globales)
- Proyecto: UE5, ACEScg o Rec.709 pipeline (usar ACES for grading, export EXR).
- Secuencias: crear 8 shots, cada shot 8 segundos, 24 fps, 4K (3840x2160).
- Cámara virtual: asignar focales por escena (ver shotlist). Usar motion blur 1/48 equivalente.
- Iluminación: usar 3-point lighting recipes (key/fill/rim) con lux target y Kelvin. Añadir practicals (lamps, glowing stone).

5) Postprocesado y LUTs
- Usar PostProcess Volume: filmic tone mapping, bloom subtle, sharpen 0.1.
- Exportar EXR multilayer y comp en Nuke/After Effects. Alternativa: render ProRes 4444 for direct edit.
- LUTs recomendadas: ARRI Rec709 / Kodak 2383 para look filmic.

6) Notas de render y calidad
- Close-ups: aumentar sample count y denoiser (OptiX/Intel) para skin detail.
- Depth of Field realista: ajustar aperture y focal length (equivalente a T-stop indicado en presets).
- Export: EXR 16-bit half float o ProRes 4444 HQ para contenedor final.
