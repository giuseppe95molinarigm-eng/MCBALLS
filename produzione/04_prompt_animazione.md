# Prompt di animazione per clip (image-to-video) — inglese

Regole generali:
- **Una sola azione principale per clip.** Genera clip da **5 s** (minimo comune ai generatori) e usa in montaggio solo il tratto migliore della durata indicata ("Uso in montaggio").
- Imposta **9:16**, senza audio generato (l'audio si fa a parte), motion/creatività media. Dove c'è **END**, usa la funzione primo + ultimo fotogramma.
- In coda a ogni prompt aggiungi il blocco negativo video di `05_vincoli_negativi.md`.
- Genera 2–3 varianti per clip; scarta subito quelle in cui cambia l'orecchio, lo stile o la corporatura.
- Ogni prompt ripete i tratti chiave apposta: alcuni modelli "dimenticano" il riferimento dopo 2–3 secondi.

Stile da ripetere (già incluso sotto): *2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, slightly desaturated colours, no 3D.*

---

### 1A · Generare 5 s → uso 3,0 s · START 1A
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, slightly desaturated colours, no 3D. Vertical 9:16.
Static camera at floor level. Macpalle, a warm taupe-grey Chartreux cat with golden eyes, modest belly and a tiny straight-cropped tip on his right ear, sits on his bottom facing a closed teal-blue door, seen from behind; he lifts his head and meows pleadingly twice, body bobbing slightly with each meow, tail flicking on the terracotta floor. The owner's lower body (navy sponge-pattern shorts, red Crocs-style clogs) stands perfectly still in front of the door, cut at the waist.
Keep unchanged: door closed, framing, owner never shown above the waist, cat design, ear.
```

### 1B · 5 s → uso 3,0 s · START 1B · push-in lento
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, slightly desaturated colours, no 3D. Vertical 9:16.
Slow push-in. Macpalle, a warm taupe-grey Chartreux cat with golden-yellow eyes, dark grey nose, pale whiskers, modest belly, only the tiny tip of his right ear cropped straight (viewer's left), sits on his bottom crying dramatically: he looks at the door off-screen right, then tilts his head up toward the owner above frame, then back to the door, mouth opening in a wailing meow, ears flat, eyes glossy.
Keep unchanged: cat proportions, ear on viewer's left, flat cartoon style, background landing.
```

### 1C · 5 s → uso 2,0 s · START 1C · camera fissa
```
2D hand-drawn cartoon animation, dark ink outlines, painterly paper texture, slightly desaturated colours, no 3D. Vertical 9:16.
Static low camera. The owner's lower legs in red Crocs-style clogs, navy shorts hem with yellow sponge pattern at top edge, stand completely still in front of a closed teal-blue door. At bottom left, the warm taupe-grey head of Macpalle (golden eyes, pale whiskers, tiny straight-cropped right ear tip) rises into frame, looks up and sobs, chin trembling.
Keep unchanged: owner motionless, nothing above the shorts hem, cat design.
```

### 2A · 5 s → uso 2,5 s · START 2A
```
2D hand-drawn cartoon animation, dark ink outlines, small fur and leg-hair strokes, painterly paper texture, slightly desaturated colours, no 3D. Vertical 9:16.
Static close-up on the owner's shin and red Crocs-style clog. A round warm taupe-grey cat paw enters from the left and taps the shin twice gently just above the clog, then withdraws; the cat's warm taupe-grey head at the left edge turns away toward the door in the background. The leg does not move.
Keep unchanged: clog colour and shape, shorts pattern at top edge, nothing above the shorts, cat has one paw in frame only.
```

### 2B · 5 s → uso 1,5 s · START 2B
```
2D hand-drawn cartoon animation, dark ink outlines, painterly paper texture, slightly desaturated colours, no 3D. Vertical 9:16.
Static low side camera. The owner's left foot in a bright red Crocs-style clog slides sideways and plants itself firmly in front of the teal-blue door, blocking it more. In the foreground Macpalle, a warm taupe-grey Chartreux cat with golden eyes and modest belly, leans back on his bottom, offended.
Keep unchanged: only knees-down visible for the owner, door closed, same clogs and shorts.
```

### 2C · 5 s → uso 2,0 s (+ flash in montaggio) · START 2C → END 2C · push-in deciso
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, no 3D. Vertical 9:16.
Fast continuous push-in from close-up to extreme close-up. Macpalle, a warm taupe-grey Chartreux cat with golden-yellow eyes, dark grey nose, pale whiskers, tiny straight-cropped tip on his right ear (viewer's left), ends a long theatrical meow; his mouth closes abruptly, tears vanish, eyelids lower to half-closed, a confident asymmetric smirk appears. The camera dives into his golden eye, where a reflection of an epic rooftop under a giant golden sun grows brighter until warm gold light fills the frame.
Keep unchanged: cat identity, ear side, 2D drawn look.
```

### 3A · 5 s → uso 2,0 s · START 3A → END 3A · camera bassa fissa
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, warm epic sunset colours, no 3D. Vertical 9:16.
Static low angle on an epic terracotta rooftop with a giant golden-yellow sun behind. Seen from behind, a normal warm taupe-grey Chartreux cat rises onto his hind legs; a burst of golden light and dust flashes and his body swells into a huge muscular half-cat half-man standing upright, long grey tail lashing, black athletic shorts appearing. Exaggerated cartoon squash-and-stretch transformation.
Keep unchanged: warm taupe-grey fur colour, cat head shape and ears with small straight-cropped tip on his right ear, same tiles and sun.
```

### 3B · 5 s → uso 2,0 s · START 3B · orbita lenta 15° verso destra
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, warm epic sunset light, no 3D. Vertical 9:16.
Slow 15-degree orbit to the right, low angle. Hero Macpalle — muscular anthropomorphic half-cat half-man with short uniform warm taupe-grey fur, black athletic shorts with grey stripe, silver dog tag, long grey tail; Chartreux cat head with golden eyes, pale whiskers, tiny straight-cropped right ear tip on viewer's left — tilts his head sharply left then right, cracking his neck with a hand on it, shoulders rolling, tail whipping once. Bored superior face.
Keep unchanged: cat face identity, two arms and two legs, five-fingered padded hands, costume, sun behind.
```

### 3C · 5 s → uso 2,0 s · START 3C · camera fissa
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, warm golden rim light, no 3D. Vertical 9:16.
Static front close-up. Hero Macpalle, muscular warm taupe-grey furry Chartreux cat-man with dog tag, looks straight into the camera; wind ruffles his fur and pale whiskers; he slowly lowers his eyelids to half-closed and raises one corner of his mouth into a smug asymmetric smirk; a tiny cartoon sparkle glints on a fang.
Keep unchanged: golden-yellow eyes with round black pupils, dark grey nose, small straight-cropped tip on his right ear on viewer's left, face identical to normal Macpalle.
```

### 4A · 5 s → uso 2,0 s · START 4A · tracking laterale
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, warm epic sunset colours, no 3D. Vertical 9:16.
Camera tracks sideways at the same speed as the subject. Hero Macpalle, muscular warm taupe-grey furry half-cat half-man in black athletic shorts, runs left to right across rows of terracotta curved tiles with huge powerful strides, tail streaming, dog tag bouncing, tile dust flicking up. Giant golden sun in the background scrolling slowly.
Keep unchanged: two legs, two arms, cat head with golden eyes and straight-cropped right ear tip, consistent tiles.
```

### 4B · 5 s → uso 2,0 s · START 4B · camera bassa fissa
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, warm epic sunset colours, no 3D. Vertical 9:16.
Static low front camera behind a red-brick chimney. Hero Macpalle, muscular warm taupe-grey furry half-cat half-man in black shorts, plants one hand on the chimney cap and vaults sideways over it in one smooth arc, landing beyond it and continuing to run past the camera.
Keep unchanged: chimney shape and bricks, character proportions, cat face, no extra limbs.
```

### 4C · 5 s → uso 1,5 s · START 4C · camera fissa larga
```
2D hand-drawn cartoon animation, dark ink outlines, painterly paper texture, strong golden backlight, no 3D. Vertical 9:16.
Static wide shot. Hero Macpalle, a muscular cat-man silhouette with warm taupe-grey fur edges lit gold and a long tail, flies across the gap between two tiled roofs from left to right in a long slow-motion leap against a giant golden sun, landing on the far roof.
Keep unchanged: giant sun, two roof sections, silhouette proportions.
```

### 4D · 5 s → uso 1,5 s · START 4D · camera che ruota leggermente con lui
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, warm sunset sky, no 3D. Vertical 9:16.
Camera rolls gently with the motion. Hero Macpalle, muscular warm taupe-grey furry half-cat half-man in black shorts, performs one full tucked forward somersault in mid-air against a teal-blue sky and giant golden sun, tail wrapping around him, then opens his body to prepare to land. Cartoon motion arcs.
Keep unchanged: exactly two arms and two legs, cat head, fur colour, costume.
```

### 4E · 5 s → uso 2,0 s · START 4E → END 4E · camera fissa
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, warm epic sunset light, no 3D. Vertical 9:16.
Static low front camera. Hero Macpalle holds a superhero landing (knee and fist on cracked terracotta tiles) for a beat as the dust shockwave spreads, then slowly rises to full height, brushes dust off his shoulder and gives a half smile with half-closed golden eyes.
Keep unchanged: warm taupe-grey Chartreux cat face, small straight-cropped tip on right ear on viewer's left, black shorts with grey stripe, dog tag, giant sun.
```

### 5A · 5 s → uso 1,0 s · START 5A
```
2D hand-drawn cartoon animation, dark ink outlines, feather and fur strokes, painterly paper texture, warm epic sunset light, no 3D. Vertical 9:16.
Static medium shot. Two puffed-up cartoon villain pigeons with frowning eyebrows land heavily on the terracotta tiles in the foreground, wings spread wide, chests out, blocking the path; behind them hero Macpalle, muscular warm taupe-grey cat-man in black shorts, stops and stares unimpressed.
Keep unchanged: two pigeons only, character design, sun behind.
```

### 5B · 5 s → uso 1,5 s (rallentato al 50% in montaggio) · START 5B
```
2D hand-drawn cartoon animation, dark ink outlines, fur and feather strokes, painterly paper texture, warm sunset light, no 3D. Vertical 9:16.
Static side view, slow-motion feel. A cartoon pigeon dives from the right; hero Macpalle, muscular warm taupe-grey furry cat-man in black shorts, bends far backward in a smooth slow dodge, the pigeon passing just above his face, a few feathers floating; he straightens back up calmly.
Keep unchanged: anatomy (two arms, two legs, one tail), cat face, no injury.
```

### 5C · 5 s → uso 1,5 s · START 5C
```
2D hand-drawn cartoon animation, dark ink outlines, fur and feather strokes, painterly paper texture, warm sunset light, no 3D. Vertical 9:16.
Static medium front shot. A second cartoon pigeon dives at hero Macpalle; he sweeps an open palm sideways in a martial-arts parry and the pigeon spins away like a top, dizzy but unharmed, flapping off-screen. Macpalle returns to his stance.
Keep unchanged: warm taupe-grey Chartreux cat-man design, golden eyes, straight-cropped right ear tip on viewer's left, cartoon slapstick, no blood.
```

### 5D · 5 s → uso 1,5 s · START 5D · micro-shake di camera
```
2D hand-drawn cartoon animation, dark ink outlines, fur strokes, painterly paper texture, warm epic light, no 3D. Vertical 9:16.
Front close-up with a short camera shake. Hero Macpalle opens his mouth absurdly wide and roars; a cartoon shockwave ring blasts outward, his whiskers and fur blow back, and in the background two pigeons are blown away tumbling in a cloud of feathers.
Keep unchanged: warm taupe-grey Chartreux cat face, golden eyes, ear tip on viewer's left, muscular shoulders, dog tag.
```

### 5E · 5 s → uso 1,5 s · START 5E · camera fissa
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, golden rim light, no 3D. Vertical 9:16.
Static extreme close-up. A small grey feather rests on Macpalle's nose; without moving his head he puffs his cheeks and blows it away upward with a short puff, keeping half-closed smug golden eyes and a slight smirk.
Keep unchanged: warm taupe-grey Chartreux face, dark grey nose, pale whiskers, straight-cropped right ear tip on viewer's left.
```

### 6A · 5 s → uso 2,0 s · START 6A · camera che gira lentamente intorno
```
2D hand-drawn cartoon animation, dark ink outlines, fur strokes, painterly paper texture, warm epic sunset light, no 3D. Vertical 9:16.
Slow circular camera move around the centre. A big orange tabby tomcat and a lean black cat circle hero Macpalle on the terracotta rooftop, backs arched, hissing, tails bristling; Macpalle, muscular warm taupe-grey furry cat-man in black shorts, stands still with arms crossed, only his golden eyes following them.
Keep unchanged: two enemy cats on four legs, intact ears on enemies, Macpalle's design and ear, sun.
```

### 6B · 5 s → uso 1,5 s · START 6B · leggera vista dall'alto
```
2D hand-drawn cartoon animation, dark ink outlines, fur strokes, painterly paper texture, warm sunset light, no 3D. Vertical 9:16.
Static slightly high wide shot. The orange tabby leaps from the left and the black cat from the right; hero Macpalle in the centre ducks low and spins on the spot, tail sweeping, so both cats fly over him toward each other.
Keep unchanged: three characters only, readable action, terracotta tiles, cartoon style.
```

### 6C · 5 s → uso 1,5 s · START 6C → END 6C
```
2D hand-drawn cartoon animation, dark ink outlines, fur strokes, painterly paper texture, warm sunset light, no 3D. Vertical 9:16.
Static medium shot. The orange tabby and the black cat bonk heads in mid-air with a cartoon impact star, then flop onto the tiles dazed with little stars circling their heads, unharmed. Hero Macpalle stands up over them and dusts off his hands with a smug smirk.
Keep unchanged: slapstick only, no injuries, Macpalle's warm taupe-grey fur, golden eyes, ear tip on viewer's left.
```

### 6D · 5 s → uso 2,0 s · START 6D · lentissimo push-in dal basso
```
2D hand-drawn cartoon animation, dark ink outlines, fur strokes, painterly paper texture, glorious golden backlight, no 3D. Vertical 9:16.
Very slow low-angle push-in. Hero Macpalle stands on top of a towering brick chimney against a giant golden sun, fist raised, wind blowing his warm taupe-grey fur, tail and dog tag; he grins triumphantly. Light rays pulse gently.
Keep unchanged: pose, chimney, cat face and right ear tip on viewer's left, costume.
```

### 7A · 5 s → uso 1,5 s · START 7A · camera fissa
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, slightly desaturated cool colours, no 3D. Vertical 9:16.
Static floor-level camera on a dim landing. Macpalle, a normal warm taupe-grey Chartreux cat with modest belly, golden eyes and straight-cropped right ear tip on viewer's left, sits on his bottom with hind legs spread and one front paw raised high; he blinks, realises, and slowly lowers the paw, embarrassed.
Keep unchanged: normal cat proportions (not muscular), door closed in background, owner's red clogs static at frame edge.
```

### 7B · 5 s → uso 1,5 s · START 7B → END 7B · camera fissa
```
2D hand-drawn cartoon animation, dark ink outlines, painterly paper texture, slightly desaturated colours, no 3D. Vertical 9:16.
Static low camera. The teal-blue wooden door swings open OUTWARD, away from camera, on its right hinges (handle and hand stay off-screen); daylight floods the terracotta floor. The owner's left foot in a red Crocs-style clog slides back and aside, opening a clear gap to the threshold.
Keep unchanged: door direction, nothing of the owner above the knees, clogs and shorts pattern.
```

### 7C · 5 s → uso 2,0 s · START 7C
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, soft daylight, no 3D. Vertical 9:16.
Static low camera from behind. Macpalle, a warm taupe-grey Chartreux cat with modest belly, looks up at the owner's leg beside him, then hesitantly places one front paw outside onto the terracotta roof tiles beyond the threshold, body still inside.
Keep unchanged: normal cat anatomy, four legs, ear tip on the viewer's right when seen from behind, red clog at frame left.
```

### 8A · 5 s → uso 2,0 s · START 8A
```
2D hand-drawn cartoon animation, dark ink outlines, fur and feather strokes, painterly paper texture, slightly desaturated overcast colours, no 3D. Vertical 9:16.
Static low camera on a real terracotta roof. An ordinary grey city pigeon a few metres away takes two steps and bobs its head, cooing. In the foreground Macpalle, a warm taupe-grey Chartreux cat with golden eyes, freezes; his fur puffs up slightly and his eyes go wide.
Keep unchanged: pigeon normal size and harmless, cat normal proportions, chimney and tiles.
```

### 8B · 5 s → uso 2,0 s · START 8B → END 8B
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, slightly desaturated colours, no 3D. Vertical 9:16.
Static low front camera. Macpalle, a warm taupe-grey Chartreux cat with modest belly, tries to spin around in fright, tangles his front paws, trips and falls backward, landing on his bottom in a sitting pose with hind legs spread forward and paw pads toward camera; a small puff of dust; dazed wide eyes.
Keep unchanged: four legs only, normal proportions, straight-cropped right ear tip on viewer's left, cartoon clumsy timing.
```

### 8C · 5 s → uso 2,0 s · START 8C · camera fissa
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, slightly desaturated colours, no 3D. Vertical 9:16.
Static low camera facing the stairwell housing: open teal-blue door at right, large propped terracotta tile shelter at left. Macpalle, a warm taupe-grey Chartreux cat, scrambles up clumsily and runs in an uncoordinated zig-zag toward the tile shelter, claws slipping on the tiles.
Keep unchanged: door and shelter positions, roof geometry, cat anatomy.
```

### 8D · 5 s → uso 2,0 s · START 8D → END 8D · camera fissa
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, slightly desaturated colours, no 3D. Vertical 9:16.
Static close shot. Macpalle, a warm taupe-grey Chartreux cat, wriggles head-first under the large propped terracotta tile; his hindquarters wiggle in, and finally the tip of his grey tail slips inside. The tile wobbles once.
Keep unchanged: shelter shape and position, teal-blue door threshold at right, cat body size fits the shelter.
```

### 9A · 5 s → uso 4,0 s · START 9A → END 9A · push-in lentissimo
```
2D hand-drawn cartoon animation, dark ink outlines, small fur strokes, painterly paper texture, slightly desaturated colours, no 3D. Vertical 9:16.
Very slow push-in toward the dark opening of the terracotta tile shelter. Inside, Macpalle's warm taupe-grey Chartreux face: at first golden eyes wide open in fear; he slowly turns his gaze directly into the camera, holds it, then lowers his eyelids to half-closed and forms a small asymmetric smirk, smug and knowing. In the soft-focus background one red Crocs-style clog rests motionless on the door threshold. Then hold still.
Keep unchanged: cat face identity, straight-cropped right ear tip on viewer's left, red clog static, nothing of the owner above the ankle.
```
