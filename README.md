# Computer Art 2026/27 — esercitazioni e progetto

Repository personale per le esercitazioni e il progetto del corso di **Computer Art**, Accademia di Belle Arti di Frosinone.

## Come si lavora

1. Aprire la cartella in Visual Studio Code.
2. Lavorare nella cartella dell'esercitazione in corso (`es1/`, `es2/`, …) o in `progetto/`: il codice sta in `sketch.js`.
3. Vedere il risultato nel browser, aprendo il file `index.html` della cartella.
4. Quando il lavoro è concluso, pubblicarlo: nel pannello *Controllo del codice sorgente* scrivere un messaggio, premere **Commit** e poi **Sincronizza**.

Dopo circa un minuto il lavoro è online all'indirizzo:

```
https://NOMEUTENTE.github.io/aa2627-ca/es1/
```

sostituendo `NOMEUTENTE` con il proprio nome utente di GitHub e `es1` con la cartella giusta.

## Come si consegna

La consegna si segnala aprendo una *issue* nel repository del corso, con il modulo **Consegna**: bastano il nome utente, l'attività e l'indirizzo del lavoro. Il docente risponde nella stessa issue e la chiude quando la revisione è fatta.

## Comandi di OpenCode

Nel repository ci sono due comandi pronti, da richiamare nell'interfaccia di OpenCode:

- `/specifiche es2` — legge la consegna sul sito del corso e ne riassume obiettivo e vincoli;
- `/nuova-esercitazione es2` — crea la cartella a partire dalle specifiche, con i vincoli in testa a `sketch.js`;
- `/verifica es2` — confronta il lavoro con i vincoli della consegna e dice quali non sono rispettati;
- `/consegna es2` — controlla che il lavoro sia a posto, lo pubblica e ricorda l'indirizzo da segnalare.

Le specifiche di ogni esercitazione stanno su `https://codestesie.it/aa2627/ca/attivita/es2/`, cioè nella pagina dell'attività sul sito del corso: è lì che l'agente va a leggere che cosa è richiesto.

## Che cosa non va toccato

Il file `style.css` nella radice serve a tutte le pagine: conviene aggiungere gli stili particolari nella cartella dell'esercitazione. La versione di p5.js è indicata nell'`index.html` di ogni cartella.
