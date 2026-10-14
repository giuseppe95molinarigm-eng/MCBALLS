# Piano audio e montaggio (Final Cut Pro)

## Impostazioni progetto FCP
- Nuovo progetto: **formato verticale 1080×1920, 24p**, audio stereo 48 kHz.
- Ruoli audio: `Effetti` (SFX), `Ambiente`, `Gatto` (miagolii), `Musica`. Comodi per mixare e per esportare stem.
- Importa le clip in una libreria "McBalls_EP01", eventi: `01_Clip`, `02_SFX`, `03_Musica`, `04_Ambiente`.
- Le clip generate durano 5 s: ritaglia con il **trim** al tratto indicato in `04_prompt_animazione.md`. Se la clip è a 30 fps o 25 fps, imposta "Conformazione velocità automatica" e controlla che non ci siano fotogrammi duplicati a scatti.

## Ordine delle clip (storyline principale)

| # | In | Out | Durata | Transizione in ingresso | Note di montaggio |
|---|---|---|---|---|---|
| 1A | 00:00:00 | 00:03:00 | 3,0 | Nessuna (apertura su immagine) | — |
| 1B | 00:03:00 | 00:06:00 | 3,0 | Stacco | — |
| 1C | 00:06:00 | 00:08:00 | 2,0 | Stacco | — |
| 2A | 00:08:00 | 00:10:12 | 2,5 | Stacco | — |
| 2B | 00:10:12 | 00:12:00 | 1,5 | Stacco | — |
| 2C | 00:12:00 | 00:14:00 | 2,0 | Stacco | Ultimi 4 fotogrammi (00:13:20–00:14:00): **flash oro** = generatore colore giallo-oro #F2C14E al 100% con dissolvenza in entrata di 2 fotogrammi. |
| 3A | 00:14:00 | 00:16:00 | 2,0 | Dissolvenza dal bianco-oro (4 fotogrammi) | Primo fotogramma dell'immaginario. Leggera **correzione colore calda** su tutte le clip 3A–6D (Temperatura +, Saturazione +10%) per distinguerle dalla realtà. |
| 3B | 00:16:00 | 00:18:00 | 2,0 | Stacco | — |
| 3C | 00:18:00 | 00:20:00 | 2,0 | Stacco | — |
| 4A | 00:20:00 | 00:22:00 | 2,0 | Stacco | — |
| 4B | 00:22:00 | 00:24:00 | 2,0 | Stacco sul movimento | — |
| 4C | 00:24:00 | 00:25:12 | 1,5 | Stacco sul movimento | — |
| 4D | 00:25:12 | 00:27:00 | 1,5 | Stacco sul movimento | — |
| 4E | 00:27:00 | 00:29:00 | 2,0 | Stacco | Primi 3 fotogrammi: piccolo "frame hold" sull'impatto. |
| 5A | 00:29:00 | 00:30:00 | 1,0 | Stacco | — |
| 5B | 00:30:00 | 00:31:12 | 1,5 | Stacco | **Rallenty 50%** con flusso ottico (usa 0,75 s di sorgente). |
| 5C | 00:31:12 | 00:33:00 | 1,5 | Stacco | — |
| 5D | 00:33:00 | 00:34:12 | 1,5 | Stacco | Effetto "Shake" leggero se la clip non lo ha. |
| 5E | 00:34:12 | 00:36:00 | 1,5 | Stacco | — |
| 6A | 00:36:00 | 00:38:00 | 2,0 | Stacco | — |
| 6B | 00:38:00 | 00:39:12 | 1,5 | Stacco | — |
| 6C | 00:39:12 | 00:41:00 | 1,5 | Stacco sull'impatto | — |
| 6D | 00:41:00 | 00:43:00 | 2,0 | Stacco | — |
| 7A | 00:43:00 | 00:44:12 | 1,5 | **Stacco netto, senza transizione** | Togli la correzione calda: si torna ai colori freddi e spenti. |
| 7B | 00:44:12 | 00:46:00 | 1,5 | Stacco | — |
| 7C | 00:46:00 | 00:48:00 | 2,0 | Stacco | — |
| 8A | 00:48:00 | 00:50:00 | 2,0 | Stacco | — |
| 8B | 00:50:00 | 00:52:00 | 2,0 | Stacco | — |
| 8C | 00:52:00 | 00:54:00 | 2,0 | Stacco | — |
| 8D | 00:54:00 | 00:56:00 | 2,0 | Stacco | — |
| 9A | 00:56:00 | 01:00:00 | 4,0 | Stacco | Se il push-in generato è troppo rapido, usa la clip più lenta e aggiungi Ken Burns 100→110%. **Stacco al nero secco** a 01:00:00 (ultimo fotogramma immagine 00:59:23), senza dissolvenza. |

(Timecode in secondi:fotogrammi a 24 fps; "00:10:12" = 10 s e 12 fotogrammi = 10,5 s.)

## Musica — punti esatti

| Timecode | Evento |
|---|---|
| 00:00–00:12:12 | **Nessuna musica.** |
| 00:12:12 (12,5 s) | Entra un **pad orchestrale grave** (archi bassi + timpano rullato pianissimo), in dissolvenza da −∞ a −18 dB in 1,5 s, sotto il miagolio lungo. |
| 00:13:20 | Riser + whoosh sul flash oro. |
| **00:14:00** | **Downbeat:** musica d'azione epica a pieno volume (ottoni, percussioni da trailer, cori). Colpo di trasformazione sincronizzato. |
| 00:20:00 | Inizio sezione ritmica più veloce per il parkour (≈140 BPM). |
| 00:29:00 | Variazione "kung-fu" (taiko, flauto) per gli uccelli; mini-stop di mezza battuta prima del ruggito a 00:33:00. |
| 00:36:00 | Build finale tensione. |
| 00:41:00–00:43:00 | **Culmine**: accordo finale tenuto con cori. |
| **00:43:00** | **Taglio netto della musica sul fotogramma esatto del cigolio.** Nessuna dissolvenza, nessuna coda di riverbero (taglia anche gli effetti in coda). |
| 00:43:00–01:00:00 | Nessuna musica fino alla fine. |

Struttura consigliata se generi la musica con un'AI: chiedi un brano di **32 secondi** con struttura "2 s swell, hit at 2 s, 6 s heroic intro, 9 s fast action, 7 s martial-arts variation, 7 s climax ending on a sustained chord" e allinealo con l'inizio a 00:12:00. Prompt di esempio:
```
Epic orchestral trailer action cue, 32 seconds, 140 BPM after the intro. 0–2 s: low ominous string swell and soft timpani roll. At 2 s: huge hit with brass and choir. 2–8 s: heroic brass theme. 8–17 s: driving percussion and staccato strings for a parkour chase. 17–24 s: playful martial-arts variation with taiko and bamboo flute, one half-bar stop at 21 s. 24–32 s: rising build to a triumphant climax ending on a sustained full-orchestra chord with choir. Over-the-top, slightly comedic, no vocals with words.
```

## Effetti sonori — elenco con timecode

| Timecode | Suono | Ruolo |
|---|---|---|
| 00:00–00:43 / 00:44–00:48 | Ambiente casa: stanza silenziosa, orologio lontano, frigorifero lontano | Ambiente |
| 00:00:12, 00:01:18 | Miagolii lamentosi 1 e 2 | Gatto |
| 00:03:12, 00:04:18 | Miagolii 3 e 4, più acuti e drammatici | Gatto |
| 00:06:12 | Miagolio singhiozzato | Gatto |
| 00:08:12, 00:09:00 | Due "tap" morbidi zampa su pelle | Effetti |
| 00:09:18 | Miagolino | Gatto |
| 00:10:18 | Squeak di gomma Crocs su cotto | Effetti |
| 00:12:00–00:13:05 | **Miagolio lunghissimo**, troncato di colpo a 00:13:05 | Gatto |
| 00:13:20 | Whoosh + riverbero "magico" | Effetti |
| 00:14:00 | Trasformazione: boom basso + stretch elastico cartoon + "power-up" | Effetti |
| 00:16:12, 00:17:06 | Due crack di collo cartoon | Effetti |
| 00:19:00 | "Ding" scintilla sul sorriso | Effetti |
| 00:14–00:43 | Ambiente immaginario: vento epico | Ambiente |
| 00:20:00–00:22:00 | Passi rapidi su coppi | Effetti |
| 00:22:12 | "Tak" mano su mattone + whoosh | Effetti |
| 00:24:00 | Whoosh lungo del salto | Effetti |
| 00:25:12 | Spin whoosh capriola | Effetti |
| 00:27:00 | **Impatto cinematografico**: sub-boom + detriti di tegole | Effetti |
| 00:29:00 | Battiti d'ali forti + tubare "minaccioso" (rallentato e abbassato di tono) | Effetti |
| 00:30:06 | Whoosh rallentato | Effetti |
| 00:32:00 | "Thwack" + frullo d'ali | Effetti |
| 00:33:00 | **Ruggito sproporzionato** (leone + riverbero ampio) | Effetti |
| 00:33:12 | Ali in fuga, piume | Effetti |
| 00:35:00 | "Pff" soffio | Effetti |
| 00:36:00 | Due soffi di gatto | Effetti |
| 00:38:00, 00:38:12 | Whoosh incrociati | Effetti |
| 00:39:18 | **"BONK"** cartoon + cinguettio/stelline | Effetti |
| **00:43:00** | **Cigolio della porta** (fino a 00:46:00) | Effetti |
| 00:44:12–01:00 | Ambiente esterno: vento leggero, rondini lontane, traffico lontano | Ambiente |
| 00:45:06 | Crocs che striscia sul cotto | Effetti |
| 00:47:06 | "Tic" zampa sulla tegola | Effetti |
| 00:48:12, 00:49:12 | **"Gru-gru"** del piccione, innocuo | Effetti |
| 00:51:06 | Piccolo tonfo morbido "puf" | Effetti |
| 00:52:00–00:54:00 | Corsetta impacciata + unghie che grattano | Effetti |
| 00:55:00 | Fruscio + "toc" leggero della tegola | Effetti |
| 00:56:00–00:58:18 | **Silenzio** (solo vento a −40 dB) | Ambiente |
| **00:58:18 (58,75 s)** | **Minuscolo miagolio** | Gatto |
| 01:00:00 | Nero, fine | — |

Per i miagolii consiglio **registrazioni reali** (anche del tuo gatto, col telefono) o librerie con licenza; gli effetti generati da AI sono più deboli sulle voci animali credibili.

## Mix
- Musica −14/−12 dB nei momenti pieni; SFX principali (impatto, ruggito, bonk) a picco −3 dBFS.
- Loudness finale **−14 LUFS integrati**, true peak −1 dBTP (standard per Instagram/TikTok/YouTube Shorts).
- Esporta: H.264 o HEVC, 1080×1920, 24p, 15–20 Mbps; e una versione ProRes master.
