# Ensamblaje, LUTs y entrega (ffmpeg + DaVinci Resolve)

1) Nombres de archivos esperados (por escena): scene01.mp4 ... scene08.mp4 (4K 24fps)

2) Concatenar clips con ffmpeg (si todos codecs iguales):
- Crear file list: printf "file 'scene01.mp4'\nfile 'scene02.mp4'\n..." > list.txt
- Comando: ffmpeg -f concat -safe 0 -i list.txt -c copy rough_cut.mp4

3) Aplicar LUT con ffmpeg (si tienes LUT .cube):
ffmpeg -i input.mp4 -vf "lut3d='Kodak2383.cube'" -c:v prores_ks -profile:v 3 output_prores.mov

4) Recomendación DaVinci Resolve:
- Importar EXR / ProRes masters.
- Pipeline: ACEScg -> Timeline in Rec709 (or deliver in Rec709/BT.2020 según destino).
- Aplicar LUT base (ARRI Rec709 o Kodak 2383), ajustar skin tones en qualifier.
- Export: ProRes 422 HQ for deliverable, H.264/H.265 for web.

5) Música y SFX (royalty-free sugerida)
- Music: "Cinematic Ambient" from Free Music Archive or Artlist (licencia necesaria para comercial).
- SFX: footsteps, rain, ambient forest — Freesound.org (revisar licencia CC)

6) Notas finales
- Guardar proyecto Resolve y exportar dailies para revisión (ProRes 422 LT dailies).