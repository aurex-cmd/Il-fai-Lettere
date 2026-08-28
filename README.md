# Il Fai Lettere

Strumento offline-first per la formattazione di documenti clinici, in tre schede:

- **Anamnesi** — riordina e impagina il testo di cartella clinica (anamnesi familiare/fisiologica, farmacologica, patologica remota, patologica prossima) in ordine fisso, senza chiamate esterne.
- **Farmaci** — trasforma un elenco di farmaci copiato dalla cartella clinica in un elenco formattato e ordinato per orario di somministrazione, senza chiamate esterne.
- **Epicrisi** — genera epicrisi o riscrive testo libero tramite API OpenAI (richiede una API key personale, salvata solo nel browser).

Nessun dato lascia il browser, tranne per la scheda Epicrisi che chiama l'API OpenAI con la chiave inserita dall'utente.

## Uso
Apri `index.html` (oppure la pagina GitHub Pages, una volta attivata).

## GitHub Pages
Settings → Pages → Deploy from branch → `main` → `/ (root)`.
