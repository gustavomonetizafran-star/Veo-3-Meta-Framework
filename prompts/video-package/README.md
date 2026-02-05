# Paquete: Video (Virtual Production + AI fallback)

Descripción
Este paquete está diseñado para producir vídeo lo más realista posible sin rodaje físico usando Virtual Production (Unreal Engine + MetaHuman) como enfoque principal y con prompts optimizados para AI (Runway / Pika) como fallback para mood reels rápidos.

Estructura del paquete
- unreal_meta_human_instructions.md — instrucciones paso a paso para crear el MetaHuman con las medidas del personaje, shaders y setup en Unreal.
- prompts_runway_pika.md — 8 prompts optimizados (uno por escena) listos para Runway Gen-2 / Pika Labs, con parámetros (aspect, duration, seed, LUT emulado).
- storyboard_and_shotlist.md — shot list y mini-descripciones temporizadas por escena.
- voice_script_es.md — guion de voz en off en español (neutro) con marcas de tiempo por escena.
- ffmpeg_and_resolve.md — comandos y pasos para unir clips, aplicar LUTs y entrega final (DaVinci Resolve + ffmpeg).

Cómo usar
1. Si eliges Virtual Production: sigue unreal_meta_human_instructions.md y monta las escenas en Unreal. Usa Sequencer para renderizado y exporta EXR/ProRes.
2. Si eliges AI rápido: copia los prompts de prompts_runway_pika.md a Runway/Pika y genera clips por escena (4K, 16:9, 8s). Itera seeds y negative prompts según necesidad.
3. Usa ffmpeg_and_resolve.md para ensamblar los clips y aplicar LUTs finales.

Licencias y recursos
- Música/SFX sugerido: enlaces en ffmpeg_and_resolve.md a bibliotecas libres de royalties.
