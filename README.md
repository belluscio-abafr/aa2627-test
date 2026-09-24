# Computer Art 2026/27 — esercitazioni e progetto

Repository personale per le esercitazioni e il progetto del corso di **Computer Art**, Accademia di Belle Arti di Frosinone.

Le consegne, con obiettivi, vincoli e modalità di realizzazione, si trovano nella sezione [Attività](https://codestesie.it/aa2627/ca/attivita/) del sito del corso: sono quelle il riferimento, e vanno lette per intero prima di iniziare.

## Prima di iniziare

Servono tre programmi e due estensioni di Visual Studio Code, da installare nell'ordine, perché gli ultimi passaggi dipendono dai precedenti. Le scorciatoie da tastiera indicate sono quelle di Windows e Linux: su macOS, al posto di `Ctrl`, si usa `Cmd`.

1. [Visual Studio Code](https://code.visualstudio.com/), l'editor in cui si scrive il codice.
2. [Git](https://git-scm.com/downloads), che non si apre e non si usa direttamente: è il programma con cui VS Code scarica e aggiorna il repository, e con cui OpenCode può annullare le proprie modifiche.
3. L'estensione **Live Server** di VS Code, da *Visualizza › Estensioni* (`Ctrl+Shift+X`), cercandola per nome: serve a vedere lo sketch nel browser evitando problemi di sicurezza con il caricamento di immagini, suoni o dati.
4. **OpenCode**, l'agente di programmazione. La sua [pagina di installazione](https://opencode.ai/v2/docs) propone molti modi per installarlo: quello che funziona allo stesso modo su Windows e su macOS, senza dover sistemare percorsi a mano, passa da npm. Serve quindi prima [Node.js](https://nodejs.org/), che si installa come qualsiasi altro programma e si usa solo per questo, e poi, nel terminale di VS Code (*Terminale › Nuovo terminale*), il comando

   ```
   npm install -g @opencode/cli
   ```

   Va installata la versione **Terminale**, non l'app desktop: è quella che l'estensione di VS Code usa per lavorare. Se più avanti il comando `opencode` non viene riconosciuto, basta chiudere e riaprire VS Code.

5. L'estensione **OpenCode** di VS Code, di nuovo da *Visualizza › Estensioni*: apre l'agente in un pannello laterale, più comodo della finestra bassa del terminale. Dopo l'installazione conviene chiudere e riaprire VS Code.
6. Al primo avvio l'agente sceglie da sé un modello gratuito. Per cambiarlo si scrive `/models` nella conversazione e si sceglie dall'elenco; per usare modelli a pagamento occorre prima collegare un account con `/connect`.

## Come si prepara il repository

Una volta sola, all'inizio del corso.

1. Creare un profilo su [github.com](https://github.com/signup), se non se ne ha già uno. Il nome utente scelto comparirà negli indirizzi dei propri lavori, quindi conviene sceglierlo breve e leggibile. Registrandosi con la posta dell'Accademia si può poi chiedere il [GitHub Student Developer Pack](https://education.github.com/pack), che dà gratuitamente il piano Pro.
2. Creare la propria copia del modello: nella pagina del repository del corso, premere **Use this template › Create a new repository**, dare al proprio repository il nome `aa2627-ca-lavori`, lasciarlo **Public** e premere *Create repository*. La copia è indipendente e resta sul proprio profilo.
3. Attivare GitHub Pages, che pubblica i lavori: *Settings › Pages › Source: Deploy from a branch › main › / (root) › Save*.
4. Aggiungere il docente come collaboratore, per le revisioni dirette: *Settings › Collaborators › Add people*.
5. Copiare l'indirizzo del **proprio** repository, quello appena creato, che GitHub mostra subito dopo la creazione: pulsante verde **Code**, scheda *HTTPS*, icona della copia.
6. Scaricare il repository sul proprio computer: in VS Code, *Visualizza › Riquadro comandi* (`Ctrl+Shift+P`), scrivere `clona` e scegliere *Git: Clona*; poi incollare l'indirizzo e indicare la cartella dove metterlo. Alla domanda se aprire il repository clonato, rispondere di sì.
7. Con la cartella aperta, aprire l'estensione di OpenCode e dare il comando `/inizio`, che scrive il proprio nome nelle pagine e l'indirizzo pubblico in questo file.

## Come si lavora

1. Creare la cartella dell'attività con il comando `/crea es1`, oppure `/crea progetto`.
2. Scrivere il codice in `sketch.js`, dentro quella cartella.
3. Vedere il risultato: tasto destro su `index.html` della cartella › *Open with Live Server*.

   Conviene attivare il salvataggio automatico, *File › Salvataggio automatico*: con Live Server il browser si aggiorna a ogni salvataggio, quindi le modifiche si vedono mentre si scrive, senza premere ogni volta `Ctrl+S`.

4. Pubblicare il lavoro: aprire *Visualizza › Controllo del codice sorgente* (`Ctrl+Shift+G`), scrivere un messaggio che dica che cosa è stato fatto, premere **Commit** e poi **Sincronizza**.

Dopo circa un minuto il lavoro è online all'indirizzo `https://NOMEUTENTE.github.io/aa2627-ca-lavori/es1/`, con il proprio nome utente di GitHub al posto di `NOMEUTENTE` e la cartella giusta al posto di `es1`.

Le cartelle si chiamano `es1`, `es2`, … e `progetto`: sono gli stessi nomi delle consegne sul sito, e non sono nomi liberi, perché su quelli si costruiscono l'indirizzo del lavoro pubblicato e il collegamento con la consegna.

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
- `/crea es1` o `/crea progetto` — crea la cartella dell'attività, leggendo la consegna dal sito del corso;
- `/verifica es1` — confronta il lavoro con i vincoli della consegna e dice quali non sono rispettati;
- `/consegna es1` — controlla, pubblica e ricorda l'indirizzo da segnalare.
