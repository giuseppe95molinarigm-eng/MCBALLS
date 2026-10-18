# Guida operativa Higgsfield — Ep. 1 "Il re del tetto"

> **Nota (18/10/2026):** l'abbonamento effettivamente acquistato è **Artlist AI Toolkit** (toolkit.artlist.io), piano 16.500 crediti Monthly, 19,99 €. Ha gli stessi modelli (Nano Banana Pro/2, Kling 3.0, Seedance, Veo), il Voiceover e la musica AI: tutte le istruzioni di questa guida valgono uguali. Utili in Artlist: la sezione **References** per salvare Macpalle come personaggio e richiamarlo con **@** nei prompt, e l'interruttore **Unlimited**, da provare per generare senza consumare crediti.

> Prezzi e crediti raccolti a ottobre 2026 da fonti in gran parte non ufficiali e **non sempre concordi**. Prima di pagare, controlla la pagina prezzi ufficiale di Higgsfield e il costo in crediti mostrato accanto al pulsante di generazione.

## 1. Quale piano (aggiornato dalla schermata prezzi del 18/10/2026)

Pacchetti mostrati da Higgsfield **con fatturazione annuale** (sconto 40%, impegno di 12 mesi):

| Pacchetto | Prezzo (annuale, al mese) | Totale annuo | Note |
|---|---|---|---|
| 16.500 crediti | 11,99 € | ~144 € | Nessuna generazione illimitata |
| 40.000 crediti | 23,99 € | ~288 € | ∞ generazioni senza crediti su 17 modelli |
| 80.000 crediti | 41,66 € | ~500 € | ∞ come sopra; 900 generazioni veloci, 5 in parallelo. Prezzo mensile: 69,99 € |

Prezzi **mensili** (schermata "Monthly", senza impegno annuale): **16.500 crediti 19,99 €**, **40.000 crediti 39,99 €**, **80.000 crediti 69,99 €**. Nella vista mensile non compare il simbolo ∞: le generazioni illimitate risultano legate all'annuale, quindi su Monthly anche le immagini consumano crediti.

**Scelta: 16.500 crediti, Monthly, 19,99 €.** Se i crediti non bastano si aggiungono crediti extra o si passa al pacchetto superiore, senza perdere il lavoro fatto.

Il pacchetto da 80.000 dichiara "fino a 1.600 video, 8.000 immagini, 16 ore di voiceover": le cifre "fino a" sono calcolate sui modelli più economici. In proporzione sono circa **50 crediti a video**, **10 a immagine** e **~80 al minuto di voce**.

**Per un solo episodio:**
1. Seleziona **Monthly**, non Yearly: l'annuale ti impegna per 12 mesi.
2. In "See all plans" verifica che il pacchetto da **16.500** includa Kling 3.0 con fotogramma iniziale e finale, Nano Banana Pro e il Voiceover.
3. Dopo l'iscrizione, prima di generare, controlla quanti crediti costa **una clip Kling 3.0 da 5 s, 9:16, con START+END** (il costo appare accanto al pulsante di generazione).
   - **Fino a ~120 crediti per clip** → il pacchetto da **16.500** basta.
   - **Oltre ~120 crediti per clip** → serve il **40.000**, che rende anche gratuite le immagini sui modelli illimitati.
4. Disattiva subito il rinnovo automatico. I crediti si rinnovano ogni mese e con ogni probabilità non si accumulano: usali entro il mese.

Se prevedi altri episodi di McBalls nei prossimi mesi, l'annuale da 16.500 (11,99 €/mese) diventa conveniente.

## 2. Budget in crediti (scala attuale, da verificare nell'app)

| Fase | Quantità | Crediti stimati |
|---|---|---|
| Riferimenti, keyframe, correzioni | ~190 immagini × ~10 | ~1.900 (0 se Nano Banana Pro è tra i modelli illimitati del tuo piano) |
| Clip video Kling 3.0, 31 inquadrature × 3 tentativi | ~93 clip × costo reale per clip | 93 × 50 = ~4.650 … 93 × 150 = ~14.000 |
| Voiceover (~1 minuto, con 2–3 prove per battuta) | ~3 min | ~250 |
| **Totale** | | **~7.000–16.000** |

Per stare larghi: fai le prove a 720p, passa a 1080p solo per la versione buona e non superare 3 tentativi per clip.

## 3. Strumenti da usare dentro Higgsfield

| Lavoro | Modello | Impostazioni |
|---|---|---|
| Riferimenti e keyframe | **Nano Banana Pro** | Carica le immagini di riferimento indicate in ogni prompt (fino al massimo consentito), formato **16:9** per le schede R1–R4 e R8, **9:16** per sfondi e keyframe. |
| Correzioni locali | Nano Banana Pro in modalità modifica, con l'immagine da correggere come input | Prompt breve e mirato, es. *"Change only the ears: only the tiny tip of the RIGHT ear (viewer's left) is cropped with a straight healed edge, the left ear is intact. Keep everything else identical."* |
| Animazione | **Kling 3.0** (image-to-video) | 9:16, 5 s, START dal keyframe; END dove previsto in `04_prompt_animazione.md`; audio generato **disattivato**. |
| Alternativa per le azioni difficili (4A–4E, 5B–5C, 6B–6C) | Seedance, se disponibile nel piano | Da usare solo se Kling deforma corpo o stile dopo 2 tentativi. |

Non usare le funzioni "effetti/preset" di camera di Higgsfield sulle scene reali (1, 2, 7, 8, 9): il movimento di camera è già scritto nei prompt e deve restare quasi fermo.

## 4. Procedura passo per passo

### Fase 1 — Riferimenti (giorno 1)
1. Apri Nano Banana Pro. Carica `riferimenti/forniti/01_macpalle_seduto_posa_firma.webp`, `02_…` e `03_…`.
2. Incolla il prompt **R1** da `02_riferimenti.md` + il blocco "Avoid:" di `05_vincoli_negativi.md`.
3. Controlla con la checklist (soprattutto l'orecchio). Scarica la migliore come `R1_macpalle.png`.
4. **Mandami R1** (caricala qui in chat o nel repo in `riferimenti/approvati/`). La verifico prima che tu vada avanti: se R1 è sbagliata, tutto ciò che segue lo sarà.
5. Ripeti per R2 → R8, allegando ogni volta i riferimenti indicati. Mandami R2, R3 e R4 per approvazione; R5–R8 puoi approvarli da solo con la checklist.

### Fase 2 — Keyframe (giorni 2–3)
6. Per ogni inquadratura in `03_prompt_keyframe.md`: allega i riferimenti approvati indicati in **Refs**, incolla il prompt + "Avoid:", formato 9:16.
7. Salva come `1A_start.png`, `2C_end.png`, ecc.
8. Quando hai i keyframe di una sequenza, mandameli: li controllo e, con tutti i keyframe, ti monto l'**animatic** (anteprima ferma di 60 s con tempi e audio provvisorio) per verificare il ritmo prima di spendere i crediti video.

### Fase 3 — Clip (giorni 4–6)
9. Apri Kling 3.0. Per ogni inquadratura: carica `XX_start.png` come fotogramma iniziale e, se esiste, `XX_end.png` come finale.
10. Incolla il prompt da `04_prompt_animazione.md` e, in coda, il blocco video di `05_vincoli_negativi.md` (se c'è un campo negativo, mettilo lì).
11. 9:16, 5 s, audio off, 720p per la prova. Se la prova è buona, rigenera a 1080p con lo stesso seed/impostazioni (o tieni la 720p se regge: il montaggio è a 1080×1920 e le scene sono disegnate).
12. Salva come `clip/1A_v1.mp4`, `1A_v2.mp4`…

Ordine consigliato per le clip: prima le scene reali e semplici (1A, 1B, 1C, 7A, 7C, 9A) per prendere confidenza; poi le altre reali; per ultime le scene d'azione immaginate, che richiedono più tentativi.

### Fase 4 — Audio e montaggio
13. Audio come da `06_audio_e_montaggio.md`. Per contenere i costi: miagolii registrati dal vero, effetti da Freesound/Pixabay, musica epica libera da diritti (YouTube Audio Library o Pixabay Music). Se Higgsfield offre generazione audio inclusa nei crediti avanzati, puoi usarla per gli effetti mancanti.
14. Montaggio in Final Cut Pro seguendo `06_audio_e_montaggio.md`.

## 5. Problemi tipici su Higgsfield e rimedi

| Problema | Rimedio |
|---|---|
| Kling sul piano non ha il fotogramma finale | Spezza in due clip e taglia in montaggio: **3A** (si alza + flash / parte già muscoloso), **8B** (inciampa / parte già seduto sul sedere), **9A** (occhi spalancati / parte già strafottente, dissolvenza di 4 fotogrammi), **2C** (pianto / sguardo sicuro + zoom nell'occhio). Nelle altre clip con END basta il solo START. |
| Orecchio invertito o troppo tagliato nel keyframe | Correzione locale con Nano Banana Pro (prompt al punto 3), non rigenerare tutto. |
| Il gatto diventa più realistico/3D nel video | Riduci l'intensità del movimento; togli movimenti di camera; riaggiungi in testa *"2D hand-drawn cartoon animation, flat, no 3D"*. |
| Nel muscoloso il muso cambia a metà clip | Usa START **ed** END entrambi con il muso corretto; usa in montaggio solo il tratto prima della deriva. |
| Il padrone mostra mani o busto in 7B | Rigenera con il prompt che inquadra dal ginocchio in giù; se compare una mano a bordo quadro, ritaglia in FCP. |
| Rifiuto di contenuto per i testicoli (7A, 8B) | Togli quella frase dal prompt di quell'inquadratura. |
| Rifiuto o deformazione della fantasia dei pantaloncini | Usa il keyframe con il padrone come START: il video eredita la fantasia dall'immagine. |

## 6. Registro crediti (da compilare)

| Sequenza | Generazioni previste | Crediti usati | Saldo |
|---|---|---|---|
| Riferimenti R1–R8 | ~40 immagini | | |
| Keyframe Seq. 1–2 | ~25 immagini | | |
| Keyframe Seq. 3–6 | ~65 immagini | | |
| Keyframe Seq. 7–9 | ~30 immagini | | |
| Correzioni | ~30 immagini | | |
| Voiceover | 9 battute × 2–3 prove | | |
| Clip Seq. 1–2 (6 clip) | ~18 clip | | |
| Clip Seq. 3–6 (17 clip) | ~51 clip | | |
| Clip Seq. 7–9 (8 clip) | ~24 clip | | |
