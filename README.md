# Il Fai Lettere

Strumento offline-first per la formattazione di documenti clinici, in quattro schede:

- **Anamnesi** — riordina e impagina il testo di cartella clinica (anamnesi familiare/fisiologica, farmacologica, patologica remota, patologica prossima) in ordine fisso, senza chiamate esterne.
- **Esami** — sistema i referti tramite API OpenAI: nome dell'esame in grassetto, data (senza orario) tra parentesi, testo riportato fedelmente con punteggiatura corretta, esami in ordine cronologico.
- **Farmaci** — trasforma un elenco di farmaci copiato dalla cartella clinica in un elenco formattato e ordinato per orario di somministrazione, senza chiamate esterne.
- **Epicrisi** — genera epicrisi (sintetica o estesa, con diagnosi e codici ICD-9-CM) o riscrive testo libero tramite API OpenAI.

Ogni scheda ha il tasto **Copia** e la cronologia degli ultimi 5 risultati.

## API Key e modello
Le schede Esami ed Epicrisi richiedono una API Key OpenAI personale. Si inserisce dal pulsante **🔑 API Key** in alto a destra, che apre una finestra dove si sceglie anche il modello (gpt-5.5, gpt-5, gpt-5-mini, gpt-5-nano, gpt-4.1 o un nome libero).

- Pulsante **grigio**: nessuna chiave inserita.
- Pulsante **giallo**: chiave salvata.

La chiave è salvata solo nel browser (localStorage) del dispositivo in uso: va reinserita su altri dispositivi o browser, o dopo aver cancellato i dati del sito.

## Privacy
Anamnesi e Farmaci funzionano interamente nel browser. Esami ed Epicrisi inviano il testo incollato all'API OpenAI, usando la chiave inserita dall'utente.

## Uso
Apri `index.html` (oppure la pagina GitHub Pages, una volta attivata).

## GitHub Pages
Settings → Pages → Deploy from branch → `main` → `/ (root)`.

## Cloudflare Workers
Pubblicata anche su https://il-fai-lettere.au-guarnaccia.workers.dev: Cloudflare è collegato a questo repository (ramo `main`) e ripubblica a ogni modifica.
