# Guida operativa Higgsfield — Ep. 1 "Il re del tetto"

> Prezzi e crediti raccolti a ottobre 2026 da fonti in gran parte non ufficiali e **non sempre concordi**. Prima di pagare, controlla la pagina prezzi ufficiale di Higgsfield e il costo in crediti mostrato accanto al pulsante di generazione.

## 1. Quale piano

**Higgsfield Plus, mensile, un solo mese** (circa 59 $ al mese; con fatturazione annuale costa meno al mese ma ti impegna per 12 mesi).

- Il piano **Plus** è indicato come il primo che include il **controllo di fotogramma iniziale e finale** (start/end frame), che ci serve. Lo Starter non basta né come funzioni né come crediti.
- Il Plus include circa **1.200 crediti** al mese.
- I piani a pagamento includono l'uso commerciale.
- Subito dopo l'iscrizione, **disattiva il rinnovo automatico** nelle impostazioni dell'account: i crediti restano usabili fino alla fine del mese pagato. Verifica nelle condizioni se i crediti scadono a fine periodo, e usali tutti entro quella data.

## 2. Budget in crediti

Costi indicativi per generazione: **Nano Banana Pro ≈ 2 crediti** per immagine (alcune fonti dicono illimitato per i piani a pagamento); **Kling 3.0, 5 s: ≈ 7 crediti a 720p, ≈ 8 a 1080p**.

| Fase | Quantità | Crediti stimati |
|---|---|---|
| Riferimenti R1–R8 (circa 4 tentativi ciascuno, più varianti) | ~40 immagini | ~80 |
| Keyframe START/END (40 immagini, ~3 tentativi) | ~120 immagini | ~240 |
| Correzioni (orecchio, mani, dettagli) | ~30 immagini | ~60 |
| Clip video, 31 inquadrature × 3 tentativi, 5 s, 1080p | ~93 clip | ~745 |
| **Totale** | | **~1.125 su 1.200** |

Margine stretto: per non sforare
- fai la **prima prova di ogni clip a 720p** (≈7 crediti) e passa a 1080p solo per la versione buona;
- non superare **3 tentativi per clip**; se dopo 3 non va, semplifica il prompt o cambia START/END invece di insistere;
- tieni d'occhio il saldo dopo ogni sequenza (tabella al punto 6).

Se i crediti finiscono prima del montaggio, Higgsfield vende pacchetti extra; prima di acquistarli chiedimi di rivedere le clip mancanti: spesso basta accorciare o semplificare l'azione.

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
| Orecchio invertito o troppo tagliato nel keyframe | Correzione locale con Nano Banana Pro (prompt al punto 3), non rigenerare tutto. |
| Il gatto diventa più realistico/3D nel video | Riduci l'intensità del movimento; togli movimenti di camera; riaggiungi in testa *"2D hand-drawn cartoon animation, flat, no 3D"*. |
| Nel muscoloso il muso cambia a metà clip | Usa START **ed** END entrambi con il muso corretto; usa in montaggio solo il tratto prima della deriva. |
| Il padrone mostra mani o busto in 7B | Rigenera con il prompt che inquadra dal ginocchio in giù; se compare una mano a bordo quadro, ritaglia in FCP. |
| Rifiuto di contenuto per i testicoli (7A, 8B) | Togli quella frase dal prompt di quell'inquadratura. |
| Rifiuto o deformazione della fantasia dei pantaloncini | Usa il keyframe con il padrone come START: il video eredita la fantasia dall'immagine. |

## 6. Registro crediti (da compilare)

| Sequenza | Crediti previsti | Crediti usati | Saldo |
|---|---|---|---|
| Riferimenti R1–R8 | 80 | | |
| Keyframe Seq. 1–2 | 50 | | |
| Keyframe Seq. 3–6 | 130 | | |
| Keyframe Seq. 7–9 | 60 | | |
| Correzioni | 60 | | |
| Clip Seq. 1–2 (6 clip) | 145 | | |
| Clip Seq. 3–6 (17 clip) | 410 | | |
| Clip Seq. 7–9 (8 clip) | 190 | | |
| **Totale** | **~1.125** | | |
