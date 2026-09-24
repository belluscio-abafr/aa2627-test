# Istruzioni per l'agente

Questo repository raccoglie le esercitazioni e il progetto di uno studente del corso di **Computer Art** (Accademia di Belle Arti di Frosinone, AA 2026/27).

## Lingua

Rispondere e scrivere in italiano, commenti nel codice compresi.

## Struttura e nomi delle cartelle

Nella radice stanno l'elenco dei lavori (`index.html`) e i file di servizio. Ogni attività ha la sua cartella, creata quando serve, con `index.html`, `sketch.js` e un `style.css` proprio: niente file condivisi fra le cartelle, perché le esercitazioni hanno bisogno di pochissimo stile e il progetto di uno tutto suo.

I nomi ammessi sono **`es1`, `es2`, … e `progetto`**, in minuscolo e senza spazi: sono gli stessi delle consegne sul sito, e su di essi si costruiscono sia l'indirizzo del lavoro pubblicato sia il collegamento con la consegna. Un nome diverso rompe tutte e due le cose.

Lo studente però nominerà le cose a modo suo. Quando indica un'attività in un altro modo — «esercizio 2», «e2», «Es 3», «la seconda» — ricondurre la richiesta al nome giusto e dirlo: «la cartella si chiama `es2`». Se la corrispondenza non è chiara, chiedere invece di indovinare. Se in una richiesta compare una cartella con un nome fuori schema, segnalarlo e proporre di rinominarla.

Lavorare solo nella cartella dell'attività in corso. Dell'`index.html` della radice si modifica soltanto l'elenco, per aggiungere una voce.

## Specifiche delle esercitazioni

Obiettivi, vincoli e modalità di ogni attività stanno sul sito del corso, a un indirizzo che segue sempre lo stesso schema:

```
https://codestesie.it/aa2627/ca/attivita/<cartella>/
```

dove `<cartella>` è il nome della cartella su cui si sta lavorando: `es1`, `es2`, … e `progetto`.

- Prima di iniziare a lavorare in una cartella, leggere quella pagina: è la fonte delle specifiche, e va riletta se il lavoro va avanti in sessioni diverse.
- Se una richiesta dello studente contrasta con un vincolo della consegna, dirlo chiaramente, indicare quale vincolo è e proporre un'alternativa che lo rispetti. Non aggirarlo in silenzio.
- Se l'indirizzo non risponde, l'esercitazione non è ancora stata pubblicata: fermarsi e chiederlo allo studente invece di procedere a intuito.
- Non riassumere le specifiche al posto dello studente: vanno lette da lui sul sito, per intero. Citarne un punto quando serve a spiegare una scelta o a segnalare un vincolo violato.
- Le specifiche valgono più delle istruzioni generali di questo file.

## Codice

- p5.js nella versione 2, caricata dal CDN nell'`index.html`: non aggiungere altre librerie senza chiederlo.
- Codice semplice e leggibile, anche a costo di essere più lungo: deve poter essere spiegato a voce durante la revisione.
- I parametri numerici vanno in variabili dichiarate all'inizio del file, con un nome che dica che cosa fanno, non sparsi dentro le funzioni.
- Commenti brevi sulle scelte, non sulla sintassi: `// il rumore di Perlin dà uno spostamento continuo`, non `// ciclo for`.

## Modo di lavorare

- Prima di riscrivere molto codice, proporre la modifica e attendere conferma.
- Dopo ogni modifica, dire in una o due righe che cosa è cambiato e perché, così lo studente può spiegarlo.
- Se una richiesta è ambigua, chiedere invece di inventare: le esercitazioni hanno consegne precise.
- Non inserire dati personali nelle conversazioni con il modello.
