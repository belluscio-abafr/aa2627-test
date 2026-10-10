# Computer Art 2026/27: esercitazioni

Repository personale per le esercitazioni del corso di **Computer Art**, Accademia di Belle Arti di Frosinone.

Le consegne, con obiettivi, vincoli e modalità di realizzazione, si trovano nella sezione [Attività](https://codestesie.it/aa2627/ca/attivita/) del sito del corso: sono quelle il riferimento, e vanno lette per intero prima di iniziare.

## Prima di iniziare

Servono **Visual Studio Code**, **Git**, **OpenCode** e due estensioni, OpenCode e Live Server. L'installazione, passo per passo e con le immagini, sta in due guide del sito del corso, una per sistema:

- [Visual Studio Code e OpenCode su Windows](https://codestesie.it/guide/vscode-opencode-windows/)
- [Visual Studio Code e OpenCode su macOS](https://codestesie.it/guide/vscode-opencode-macos/)

Al primo avvio l'agente sceglie da sé un modello gratuito, e per cambiarlo si scrive `/models` nella conversazione e si sceglie dall'elenco; per usare modelli a pagamento occorre prima collegare un account con `/connect`.

Le scorciatoie da tastiera indicate qui e più avanti sono quelle di Windows: su macOS, al posto di `Ctrl`, si usa `Cmd`.


## Come si prepara il repository

Una volta sola, all'inizio del corso. I primi tre passaggi si fanno **sul sito di GitHub**, con il browser; il quarto comincia lì e finisce in **Visual Studio Code**, dove si svolge anche l'ultimo.

1. **Creare un profilo su [github.com](https://github.com/signup)**, se non se ne ha già uno. \
   Il nome utente scelto comparirà negli indirizzi dei propri lavori, quindi conviene sceglierlo breve e leggibile. Registrandosi con la posta dell'Accademia si può poi chiedere il [GitHub Student Developer Pack](https://education.github.com/pack), che dà gratuitamente il piano Pro.
2. **Creare la propria copia del modello**, dalla pagina del repository del corso: \
   *Use this template › Create a new repository* \
   Dare alla copia il nome `aa2627-ca-es`, lasciarla *Public* e premere *Create repository*. È un repository indipendente e resta sul proprio profilo.
3. **Attivare GitHub Pages**, che pubblica i lavori in rete: \
   *Settings › Pages › Source: Deploy from a branch › main › / (root) › Save* \
   Dopo un minuto circa, in cima alla stessa pagina compare l'indirizzo pubblico del proprio sito, «Your site is live at…»: è la conferma che il passaggio è riuscito, e conviene aprirlo per vedere l'elenco dei lavori, ancora vuoto.
4. **Scaricare il repository sul proprio computer.** \
   Su GitHub si copia l'indirizzo del repository appena creato: \
   pulsante verde *Code › HTTPS ›* icona della copia. \
   In Visual Studio Code: \
   *Visualizza › Riquadro comandi* (`Ctrl+Shift+P`) *› Git: Clona* \
   Si incolla l'indirizzo, si indica la cartella dove mettere il repository e, alla domanda se aprirlo, si risponde di sì.
5. **Personalizzare il repository con il proprio nome**, con il comando `/inizio`. \
   La chat di OpenCode, che al primo avvio è chiusa, si apre con la piccola icona di OpenCode in alto a destra nel pannello attivo: `/inizio` si scrive nel campo editabile centrale. \
   Il comando scrive il nome nelle pagine e l'indirizzo pubblico in questo file, così gli indirizzi che si leggono qui sono già i propri.

## Come si lavora

Da qui in avanti si lavora **in Visual Studio Code**, nella cartella scaricata sul proprio computer: sul sito di GitHub non c'è più niente da fare a mano.

1. **Creare la cartella dell'esercitazione**, con il comando `/crea es1`.
2. **Scrivere il codice** in `sketch.js`, dentro quella cartella.
3. **Vedere il risultato nel browser**: \
   tasto destro su `index.html` della cartella *› Open with Live Server*
   > Conviene attivare il salvataggio automatico, *File › Salvataggio automatico*: con Live Server il browser si aggiorna a ogni salvataggio, quindi le modifiche si vedono mentre si scrive, senza premere ogni volta `Ctrl+S`.
4. **Controllare il lavoro con la consegna**, con il comando `/verifica es1`. \
   Rilegge le specifiche sul sito del corso e dice quali vincoli non sono ancora rispettati. Conviene darlo mentre si lavora, non solo alla fine: serve a sapere dove si è, non a dare un voto.
5. **Pubblicare il lavoro**, se lo si vuole vedere subito online, dal pannello del controllo di versione: \
   *Visualizza › Controllo del codice sorgente* (`Ctrl+Shift+G`) \
   Si scrive un messaggio che dica che cosa è stato fatto, si preme *Commit* e poi *Sincronizza*.
   > Il messaggio non è facoltativo: senza, il pulsante *Commit* non conclude niente, ed è il motivo per cui a volte sembra che non funzioni. Bastano poche parole, come «prima versione di es1» o «colori più scuri e sfondo nero».

Dopo circa un minuto il lavoro è online all'indirizzo `https://NOMEUTENTE.github.io/aa2627-ca-es/es1/`, con il proprio nome utente di GitHub al posto di `NOMEUTENTE` e la cartella giusta al posto di `es1`.

Le cartelle si chiamano `es1`, `es2` e così via: sono gli stessi nomi delle consegne sul sito, e non sono nomi liberi, perché su quelli si costruiscono l'indirizzo del lavoro pubblicato e il collegamento con la consegna.

## Come si consegna

Il primo passaggio si fa **in Visual Studio Code**, il secondo **nel browser**.

1. **Pubblicare il lavoro e ottenerne l'indirizzo**, con il comando `/consegna es1`. \
   Controlla che la cartella sia completa, fa commit e sincronizzazione, e mostra l'indirizzo pubblico da segnalare.
2. **Compilare il [modulo delle consegne](INDIRIZZO-DEL-MODULO)**: \
   l'esercitazione, cognome e nome, l'indirizzo appena mostrato dal comando ed eventuali note.

<!-- Da sostituire con l'indirizzo del modulo di Google, quello precompilato per questo corso. -->

Non è necessario nessun account Google per compilare il modulo. 

**La revisione arriva nella chat di Teams**, non qui. Se dopo la consegna si continua a lavorare sulla stessa esercitazione, si rifà la consegna: vale l'ultima.

> Se l'indirizzo serve senza passare dal `/consegna`, si pubblica il lavoro con Commit e Sincronizza, si apre nel browser il proprio elenco dei lavori, `https://NOMEUTENTE.github.io/aa2627-ca-es/`, si entra nella cartella dell'esercitazione e si copia l'indirizzo dalla barra. Attenzione a non confonderlo con quello di Live Server, che comincia per `127.0.0.1` e funziona solo sul proprio computer.

## I comandi di OpenCode

Quattro comandi sono stati scritti per questo corso e funzionano solo in questo repository:

- `/inizio`: scrive il proprio nome e l'indirizzo pubblico del repository;
- `/crea es1`: crea la cartella dell'esercitazione, leggendo la consegna dal sito del corso;
- `/verifica es1`: confronta il lavoro con i vincoli della consegna e dice quali non sono rispettati;
- `/consegna es1`: controlla, pubblica e ricorda l'indirizzo da segnalare.

Gli altri sono di OpenCode e funzionano in qualsiasi cartella. I più utili:

- `/help`: elenco completo dei comandi;
- `/models`: cambia il modello linguistico in uso;
- `/connect`: collega un account, per usare modelli a pagamento;
- `/undo`: annulla l'ultima richiesta e le modifiche ai file che ha prodotto (`/redo` le rimette);
- `/new`: comincia una conversazione nuova, quando si cambia argomento;
- `/sessions`: riprende una conversazione precedente;
- `/init`: rilegge il progetto e aggiorna il file `AGENTS.md`;
- `/export`: salva la conversazione in un file di testo.
