# Vincoli negativi comuni

Usali nel campo *negative prompt*. Se lo strumento non lo ha (molti modelli di editing e alcuni video), incolla la versione "Avoid:" in coda al prompt.

## Immagini (keyframe e riferimenti)

```
3D render, CGI, Pixar style, photorealistic, photo, realistic fur rendering, anime style, chibi, vector flat art without outlines, glossy plastic look, oversaturated neon colours, change of drawing style, thin uniform digital lines;
mirrored or flipped ear, cropped ear on the wrong side, both ears cropped, ear cut too deep, half ear missing, jagged torn ear, bite marks, notches, ragged ear edge;
wrong eye colour, green eyes, blue eyes, slit pupils, different coat colour, brown cat, black cat (for Macpalle), white patches, stripes, tabby markings on Macpalle;
skinny cat, obese cat, inconsistent body size, inconsistent belly, oversized or emphasised genitals, genitals as focal point;
extra limbs, extra paws, extra tail, missing tail, five legs, fused legs, extra fingers, deformed hands, malformed anatomy, twisted joints, distorted face, asymmetrical eyes (unintended), melted features;
owner's torso, owner's arms, owner's hands, owner's face, owner's head, upper body, chest, reflection of the owner, shadow showing the owner's upper body, different shoes, sneakers, sandals, barefoot owner, different shorts, plain shorts, jeans, trousers, muscular bodybuilder legs on the owner, very thin legs;
text, letters, captions, subtitles, logo, watermark, signature, frame border, UI elements, speech bubbles;
blood, wounds, injuries, gore, realistic violence.
```

Versione "Avoid:" (compatta):
```
Avoid: 3D/CGI/photoreal look or any style change; cropped ear on the wrong side, both ears cropped, ear cut too deep or jagged; eye colour or coat changes; skinny or obese body; emphasised genitals; extra or deformed limbs, paws, fingers or tails; any part of the owner above the waist, his hands or reflection; different shoes or shorts; text, logos, watermarks; blood or injuries.
```

## Video (clip animate)

```
style drift, turning 3D, photorealism, morphing face, face changing over time, ear flipping side, ear shape changing, coat colour shift, body size change, belly growing or shrinking, muscular cat in real-world scenes, normal cat in imagined scenes before transformation, extra limbs appearing, limbs merging, flickering lines, jittery outlines, boiling textures, camera shake (unless requested), sudden zoom, scene cut inside the clip, new characters appearing, owner's upper body or hands entering frame, door opening inward, door hinge switching side, shoes changing colour, text, watermark, blood.
```

## Controlli manuali dopo ogni generazione

| Controllo | Scarta se… |
|---|---|
| Orecchio | La punta tagliata non è sull'orecchio destro anatomico, oppure il taglio è irregolare/profondo. |
| Volto | Occhi non giallo oro, naso non grigio scuro, muso diverso tra normale e muscoloso. |
| Corpo | Pancetta sparisce o diventa obesità; zampe in più; mani deformi nel muscoloso. |
| Padrone | Si vede qualcosa sopra l'elastico; Crocs non rosse; fantasia dei pantaloncini diversa. |
| Ambiente | Porta che si apre verso l'interno, maniglia a destra, nascondiglio spostato rispetto alla porta. |
| Stile | Linee scure scomparse, look 3D, colori troppo saturi nelle scene reali. |
| Pulizia | Testo, lettere, watermark, firme. |
