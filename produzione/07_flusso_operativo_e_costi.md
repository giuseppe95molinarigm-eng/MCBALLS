# Flusso operativo, strumenti e costi

## Cosa posso fare io e cosa no (stato attuale di questa sessione)

| Attività | Posso farla ora? | Note |
|---|---|---|
| Sceneggiatura tecnica, shot list, prompt, vincoli, piano audio e montaggio | **Sì: fatto** (questa cartella) | — |
| Generare immagini, video, musica, effetti | **No** | In questa sessione non ho strumenti di generazione né connettori collegati. Non ho generato nessuna immagine o clip. |
| Chiamare API esterne (fal.ai, ElevenLabs…) | **No, per ora** | Ho provato: la rete di questo ambiente blocca `fal.run` e `api.elevenlabs.io`. |
| Fare pagamenti, abbonamenti, inserire carte | **No, mai** | Non gestisco credenziali di pagamento. Gli acquisti li fai tu. |
| Controllare le immagini generate (orecchio, stile, continuità) | **Sì** | Se carichi i file nel repo o in chat, li guardo e approvo/scarto con la checklist. |
| Premontaggio con ffmpeg (animatic, rough cut con timecode) | **Sì** | ffmpeg è installato. Con keyframe o clip nel repo posso montare un animatic 9:16 di 60 s. |
| Montaggio finale in Final Cut Pro | **No** | Lo fai tu sul Mac, seguendo `06_audio_e_montaggio.md`. |

### Come rendermi autonomo (opzionale)
Se vuoi che generi io, scegliendo e scartando le varianti e salvando tutto nel repo:
1. Crea un account **fal.ai** (immagini + video da un'unica API, pagamento a consumo) e uno **ElevenLabs** (effetti e musica). Ricarica un credito prepagato e imposta un **limite di spesa** (consiglio **120 $** totali).
2. Nelle impostazioni dell'ambiente cloud (menu dell'ambiente nella barra del titolo della sessione → *Edit*):
   - aggiungi le chiavi come segreti/variabili d'ambiente con i nomi **`FAL_KEY`** ed **`ELEVENLABS_API_KEY`**. **Non incollarle in chat**;
   - in *Network access*, aggiungi agli **Allowed domains**: `fal.run`, `queue.fal.run`, `rest.alpha.fal.ai`, `fal.media`, `v3.fal.media`, `api.elevenlabs.io` (guida: https://code.claude.com/docs/en/cloud-environments#network-access).
3. Apri una nuova sessione su questo repo: io verifico gli endpoint attuali dei modelli, ti confermo il costo stimato prima di ogni lotto e procedo per checkpoint (riferimenti → keyframe → clip → audio → animatic), fermandomi alle approvazioni dei riferimenti R1–R4.

## Strumenti consigliati (verifica prezzi e funzioni prima di pagare)

Ho controllato fonti online a ottobre 2026, ma sono quasi tutte di terze parti e i listini cambiano spesso: **i prezzi sotto sono indicativi e vanno verificati sulle pagine ufficiali.**

| Fase | Strumento principale | Perché | Alternative |
|---|---|---|---|
| Riferimenti e keyframe | **Nano Banana Pro** (Google, via app Gemini o via fal.ai) | Ottimo nel mantenere un personaggio partendo da più immagini di riferimento e nel correggere singoli dettagli (orecchio) senza ridisegnare tutto. | **Midjourney V7** con *Omni Reference* (`--ow` alto per bloccare l'identità): stile pittorico eccellente, editing meno preciso. |
| Animazione | **Kling 3.0** (app Kling o via fal.ai) | Image-to-video 9:16, primo + ultimo fotogramma, buona tenuta dello stile 2D. | Seedance (anche primo/ultimo fotogramma), Google Veo, Runway. |
| Effetti e musica | **ElevenLabs** (Sound Effects + Music) | Effetti da testo e brano con struttura a tempi; licenza commerciale con piani a pagamento. | Librerie con licenza (Epidemic Sound, Artlist), Freesound per i miagolii reali. |
| Montaggio | **Final Cut Pro** | Già previsto. | — |

### Stima dei costi

**Percorso A — lavori tu con gli abbonamenti (1 mese)**
| Voce | Costo indicativo |
|---|---|
| Midjourney Basic/Standard *oppure* Google AI Pro (Gemini, Nano Banana Pro) | 10–30 $ / ~22 € al mese |
| Kling, piano a pagamento intermedio (crediti sufficienti per ~100 clip da 5 s: verifica il consumo per clip sul piano) | ~25–65 $ al mese |
| ElevenLabs Starter/Creator | ~6–11 $ al mese |
| **Totale** | **~45–110 $ per l'episodio** |

**Percorso B — API a consumo, lavoro io (se abiliti chiavi e rete)**
| Voce | Calcolo | Costo indicativo |
|---|---|---|
| Immagini (8 schede di riferimento + 40 keyframe, ~3 varianti ciascuna ≈ 150 immagini) | 0,04–0,15 $ per immagine | 6–25 $ |
| Video (31 clip × 3 varianti × 5 s ≈ 465 s), Kling 3.0 Pro senza audio | ~0,112 $/s | ~52 $ |
| Effetti e musica ElevenLabs | piano Starter/Creator | 6–11 $ |
| **Totale** | | **~65–90 $**, limite di spesa consigliato 120 $ |

Per ridurre i costi: fai le prove di movimento con un modello più economico (ad es. una versione "Turbo"), e usa il modello Pro solo sulle varianti finali.

## Piano scelto: Higgsfield (tutte le 31 inquadrature animate)

Scelta del 18/10/2026: un solo abbonamento **Higgsfield Plus**, un mese, senza rinnovo. Tutte le inquadrature diventano clip video. Guida operativa completa in [`08_guida_higgsfield.md`](08_guida_higgsfield.md).

## Flusso di lavoro concreto (passo per passo)

1. **Riferimenti** (`02_riferimenti.md`): R1 → R2 → R3 → R4 → R5 → R6 → R7 → R8. Approva ognuno con la checklist. Salvali in `riferimenti/approvati/`.
2. **Keyframe** (`03_prompt_keyframe.md`): genera START (ed END dove previsto) di tutte le 31 inquadrature, allegando i riferimenti indicati. Correggi orecchio e dettagli con l'inpainting. Salva come `keyframe/1A_start.png`, `keyframe/1A_end.png`…
3. **Animatic** (consigliato, lo posso fare io): monta i keyframe come immagini ferme con i tempi esatti e un audio provvisorio. Serve a verificare ritmo e comicità **prima** di spendere crediti video.
4. **Clip** (`04_prompt_animazione.md`): 2–3 varianti per inquadratura, 5 s, 9:16, senza audio. Scegli la migliore. Salva come `clip/1A_v1.mp4`…
5. **Audio** (`06_audio_e_montaggio.md`): musica di 32 s (con struttura a tempi), effetti dalla lista, miagolii reali.
6. **Montaggio in Final Cut Pro** seguendo ordine, transizioni e punti musica. Correzione colore calda solo su 3A–6D.
7. **Revisione finale** con la checklist di `05_vincoli_negativi.md` fotogramma per fotogramma sulle inquadrature critiche: 2C, 3A, 3C, 7A, 8B, 9A.

## Rischi noti e soluzioni

| Rischio | Soluzione |
|---|---|
| L'orecchio cambia lato durante l'animazione | Usa START + END entrambi corretti; scegli clip brevi; se succede negli ultimi fotogrammi, accorcia il taglio. |
| Il muscoloso non sembra lo stesso gatto | Rigenera la testa di R3 con inpainting usando R2; nei prompt video ripeti sempre volto e orecchio. |
| Il padrone mostra le mani all'apertura della porta (7B) | Inquadratura dal ginocchio in giù; se compare una mano, ritaglia/scala il quadro in FCP (9:16 a 1080 lascia margine se generi a risoluzione più alta). |
| Generatore rifiuta testicoli o fantasia SpongeBob | Il dettaglio dei testicoli è necessario solo in 7A e 8B: se viene rifiutato, toglilo da quel prompt (resta visibile nel riferimento base). La fantasia è descritta senza nomi di marchi. |
| Lo stile diventa 3D nelle scene d'azione | Abbassa il "motion"/creatività, rigenera; evita camere troppo dinamiche. |
