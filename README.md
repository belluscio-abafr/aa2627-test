# Computer Art 2026/27 — esercitazioni e progetto

Repository personale per le esercitazioni e il progetto del corso di **Computer Art**, Accademia di Belle Arti di Frosinone.

Le consegne, con obiettivi, vincoli e modalità di realizzazione, stanno nella sezione [Attività](https://codestesie.it/aa2627/ca/attivita/) del sito del corso: sono quelle il riferimento, e vanno lette per intero prima di iniziare.

## Per iniziare, una volta sola

**I programmi.** Vanno installati nell'ordine, perché l'ultimo passaggio dipende dai precedenti.

1. [Visual Studio Code](https://code.visualstudio.com/), l'editor in cui si scrive il codice.
2. [Git](https://git-scm.com/downloads), che non si apre e non si usa direttamente: è il programma con cui VS Code scarica e aggiorna il repository, e con cui OpenCode può annullare le proprie modifiche.
3. L'estensione **Live Server**, dal pannello *Estensioni* di VS Code: serve a vedere lo sketch nel browser. Aprendo il file `index.html` con un doppio clic, invece, le funzioni di p5.js che caricano immagini, suoni o dati non funzionano.
4. **OpenCode**, l'agente di programmazione, dal terminale di VS Code (*Terminale › Nuovo terminale*):

   ```
   winget install SST.opencode
   ```

   Su macOS e su Linux, al posto di questo comando:

   ```
   curl -fsSL https://opencode.ai/install | bash
   ```

   Dopo l'installazione il terminale va chiuso e riaperto.

5. L'estensione di OpenCode per VS Code **si installa da sé**: basta scrivere `opencode` nel terminale e confermare. Da lì in poi l'agente si apre con `Ctrl+Esc`.
6. Al primo avvio OpenCode chiede il modello da usare: si segue la procedura con il comando `/connect` e le istruzioni indicate nel terminale.

**Il repository.**

1. Attivare GitHub Pages: nella pagina del repository, *Settings › Pages › Source: Deploy from a branch › main › / (root) › Save*. Dopo circa un minuto il sito è raggiungibile.
2. Aggiungere il docente come collaboratore: *Settings › Collaborators › Add people*. Serve per le revisioni dirette.
3. Scaricare il repository sul proprio computer: in VS Code, *Controllo del codice sorgente › Clona repository*, scegliendo il repository e una cartella dove metterlo. Poi *Apri* la cartella.
4. Con il repository aperto, lanciare OpenCode e dare il comando `/inizio`: scrive il proprio nome nelle pagine e l'indirizzo pubblico in questo file.

## Come si lavora

1. Creare la cartella dell'attività con il comando `/crea es1`, oppure `/crea progetto`.
2. Scrivere il codice in `sketch.js`, dentro quella cartella.
3. Vedere il risultato: tasto destro su `index.html` della cartella › *Open with Live Server*.

   Conviene attivare il salvataggio automatico, *File › Salvataggio automatico*: con Live Server il browser si aggiorna a ogni salvataggio, quindi le modifiche si vedono mentre si scrive, senza premere ogni volta `Ctrl+S`.

4. Pubblicare il lavoro: nel pannello *Controllo del codice sorgente* scrivere un messaggio che dica che cosa è stato fatto, premere **Commit** e poi **Sincronizza**.

Dopo circa un minuto il lavoro è online all'indirizzo `https://NOMEUTENTE.github.io/aa2627-ca/es1/`, con il proprio nome utente di GitHub al posto di `NOMEUTENTE` e la cartella giusta al posto di `es1`.

## Come si consegna

Quando il lavoro è concluso e pubblicato, si segnala aprendo una *issue* nel repository del corso, che è il registro delle consegne:

1. aprire [github.com/belluscio-abafr/aa2627-ca/issues](https://github.com/belluscio-abafr/aa2627-ca/issues);
2. premere il pulsante verde **New issue**;
3. scegliere **Consegna** fra i moduli proposti e premere *Get started*;
4. compilare i campi: nome utente di GitHub, attività consegnata, indirizzo del lavoro, eventuali note per la revisione;
5. premere **Create** in fondo alla pagina.

Il docente risponde nella stessa pagina, e la risposta arriva per posta elettronica. La issue viene chiusa quando la revisione è conclusa: le issue aperte sono i lavori ancora da rivedere.

## I comandi di OpenCode

- `/inizio` — scrive il proprio nome e l'indirizzo pubblico del repository;
- `/crea es2` o `/crea progetto` — crea la cartella dell'attività, leggendo la consegna dal sito del corso;
- `/verifica es2` — confronta il lavoro con i vincoli della consegna e dice quali non sono rispettati;
- `/consegna es2` — controlla, pubblica e ricorda l'indirizzo da segnalare.

## Struttura

Nella radice ci sono solo l'elenco dei lavori (`index.html`) e i file di servizio. Ogni attività ha la sua cartella, con dentro tutto quello che le serve:

```
es1/
  index.html    la pagina che carica p5.js e lo sketch
  sketch.js     il codice
  style.css     lo stile della pagina, solo di questa cartella
```

Le cartelle si chiamano `es1`, `es2`, … e `progetto`: gli stessi nomi delle consegne sul sito. Non sono nomi liberi, perché su quelli si costruiscono l'indirizzo del lavoro pubblicato e il collegamento con la consegna.
