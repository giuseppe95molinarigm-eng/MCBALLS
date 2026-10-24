# Voiceover — Ep. 1 "Il re del tetto"

Aggiunto su richiesta (18/10/2026): un narratore racconta l'episodio. Sostituisce la scelta iniziale "niente voce narrante"; miagolii, effetti e ambiente restano.

## Tono
**Lingua: inglese** (decisione del 24/10/2026). Voce maschile adulta, calda e solenne, da **documentario naturalistico**, recitata sempre seriamente. La comicità nasce dal contrasto: il narratore descrive con enfasi epica ciò che Macpalle immagina, e con la stessa solennità la ritirata nella realtà. Niente ammiccamenti nella voce.

**Regola d'oro: il narratore tace sulle battute visive.** Restano senza voce il miagolio lungo con lo sguardo sicuro (2C), il cigolio della porta (7A), il "gru-gru" e la caduta (8A–8B) e tutto il finale (9A).

## Testo con tempi

| Timecode | Inquadratura | Battuta | Durata parlato |
|---|---|---|---|
| 0:00.5–0:02.8 | 1A | «This is McBalls. A Chartreux.» | ~2,0 s |
| 0:03.0–0:06.0 | 1B | «And he's crying because behind that door lies the only thing he truly desires… the roof.» | ~3,0 s |
| 0:08.3–0:11.8 | 2A–2B | «But his owner knows his cat. And the door stays shut.» | ~3,5 s |
| 0:12.0–0:14.0 | 2C | *(silenzio: miagolio lungo e sguardo)* | — |
| 0:15.0–0:19.0 | 3A–3C | «Because up there, McBalls knows who he really is.» … *(pausa)* … «The King of the Roof.» | ~3,5 s |
| 0:20.5–0:26.5 | 4A–4D | «Agile. Unstoppable. Master of every tile, of every chimney.» | ~5,0 s |
| 0:29.3–0:31.0 | 5A–5B | «Pigeons fear him.» | ~1,5 s |
| 0:36.3–0:38.0 | 6A | «The neighbourhood cats respect him.» | ~1,8 s |
| 0:41.3–0:43.0 | 6D | «No one has ever beaten him.» | ~1,6 s |
| 0:43.0–0:44.5 | 7A | *(silenzio: cigolio)* | — |
| 0:45.0–0:47.5 | 7B–7C | «And here it is, at last… his kingdom.» | ~2,3 s |
| 0:48.0–0:52.0 | 8A–8B | *(silenzio: "gru-gru", caduta sul sedere)* | — |
| 0:52.3–0:55.8 | 8C–8D | «After careful consideration, the king chooses… a strategic retreat.» | ~3,5 s |
| 0:56.0–1:00.0 | 9A | *(silenzio, poi minuscolo miagolio a 0:58.75)* | — |

Totale circa 70 parole: ritmo lento e chiaro, con spazio per le gag.

## Generazione della voce

**Dove:** nella sezione audio/Voiceover di Higgsfield, che include modelli vocali di terze parti (tra cui Eleven v3), quindi senza un altro abbonamento. Se i crediti finiscono, il ripiego è ElevenLabs Starter (circa 6 $/mese, con uso commerciale).

**Come:**
- genera **una battuta per file**, non tutto il testo insieme: così sistemi i tempi in Final Cut Pro senza tagliare le frasi;
- scegli una voce inglese maschile matura (accento britannico da documentario), adatta a un documentario; provane 2–3 sulla prima battuta e poi tieni **sempre la stessa voce e le stesse impostazioni**;
- per i puntini di sospensione lascia la pausa nel testo; se il modello la ignora, separa la frase in due file;
- nomina i file `VO_01.wav` … `VO_09.wav` nell'ordine della tabella.

Istruzione di stile, se il modello la accetta: *"British male narrator, warm deep voice, solemn nature-documentary delivery, slow pace, completely serious."*

## Mix con la voce
- In FCP aggiungi il ruolo audio `Voce`.
- Voce a circa −16/−14 LUFS sul parlato, picchi sotto −3 dBFS.
- **Ducking della musica:** durante ogni battuta abbassa la musica di 6–8 dB con dissolvenze di 0,3 s; tra una battuta e l'altra torna su.
- Il taglio netto della musica a 0:43.0 resta invariato.
- Ambiente ed effetti restano come in `06_audio_e_montaggio.md`; abbassa di 3 dB solo l'ambiente sotto la voce.
