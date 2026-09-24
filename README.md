# Computer Art 2026/27 — esercitazioni e progetto

Repository personale per le esercitazioni e il progetto del corso di **Computer Art**, Accademia di Belle Arti di Frosinone.

Le consegne, con obiettivi, vincoli e modalità di realizzazione, si trovano nella sezione [Attività](https://codestesie.it/aa2627/ca/attivita/) del sito del corso: sono quelle il riferimento, e vanno lette per intero prima di iniziare.

## Prima di iniziare

Servono tre programmi e due estensioni, da installare nell'ordine, perché gli ultimi passaggi dipendono dai precedenti.

1. [Visual Studio Code](https://code.visualstudio.com/), l'editor in cui si scrive il codice.
2. [Git](https://git-scm.com/downloads), che non si apre e non si usa direttamente: è il programma con cui VS Code scarica e aggiorna il repository, e con cui OpenCode può annullare le proprie modifiche.
3. L'estensione **Live Server**, da *Visualizza › Estensioni* (`Ctrl+Shift+X`): serve a vedere lo sketch nel browser evitando problemi di sicurezza con il caricamento di  immagini, suoni o dati.
4. **OpenCode**, l'agente di programmazione, dalla sua [pagina di download](https://opencode.ai/download). Serve la versione **Terminale**, non l'app desktop, perché è quella che lavora dentro VS Code. La pagina propone diversi modi di installarla: il più semplice è il primo, il comando che comincia con `curl`, da copiare e incollare in un terminale. Su macOS e su Linux va bene il terminale di VS Code; su Windows serve invece un terminale **Git Bash**, che si apre dalla freccia accanto al `+` del pannello del terminale e che è già sul computer, perché arriva insieme a Git.
5. L'estensione di OpenCode per VS Code **si installa da sé**: basta scrivere `opencode` in un terminale di VS Code (*Terminale › Nuovo terminale*) e confermare. Da lì in poi l'agente si apre con `Ctrl+Esc`.
6. Al primo avvio OpenCode chiede con quale modello lavorare: si seguono le istruzioni indicate nel terminale.

## Come si prepara il repository

Una volta sola, all'inizio del corso.

1. Creare la propria copia del modello: nella pagina del repository del corso, premere **Use this template › Create a new repository**, dare al repository il nome `aa2627-ca`, lasciarlo **Public** e premere *Create repository*. La copia è indipendente e resta sul proprio profilo.
2. Attivare GitHub Pages, che pubblica i lavori: *Settings › Pages › Source: Deploy from a branch › main › / (root) › Save*.
3. Aggiungere il docente come collaboratore, per le revisioni dirette: *Settings › Collaborators › Add people*.
4. Copiare l'indirizzo del proprio repository: nella sua pagina, pulsante verde **Code**, scheda *HTTPS*, icona della copia.
5. Scaricare il repository sul proprio computer: in VS Code, *Visualizza › Riquadro comandi* (`Ctrl+Shift+P`), scrivere `clona` e scegliere *Git: Clona*; poi incollare l'indirizzo e indicare la cartella dove metterlo. Alla domanda se aprire il repository clonato, rispondere di sì.
6. Con la cartella aperta, lanciare OpenCode con `Ctrl+Esc` e dare il comando `/inizio`, che scrive il proprio nome nelle pagine e l'indirizzo pubblico in questo file.

## Come si lavora

1. Creare la cartella dell'attività con il comando `/crea es1`, oppure `/crea progetto`.
2. Scrivere il codice in `sketch.js`, dentro quella cartella.
3. Vedere il risultato: tasto destro su `index.html` della cartella › *Open with Live Server*.

   Conviene attivare il salvataggio automatico, *File › Salvataggio automatico*: con Live Server il browser si aggiorna a ogni salvataggio, quindi le modifiche si vedono mentre si scrive, senza premere ogni volta `Ctrl+S`.

4. Pubblicare il lavoro: aprire *Visualizza › Controllo del codice sorgente* (`Ctrl+Shift+G`), scrivere un messaggio che dica che cosa è stato fatto, premere **Commit** e poi **Sincronizza**.

Dopo circa un minuto il lavoro è online all'indirizzo `https://NOMEUTENTE.github.io/aa2627-ca/es1/`, con il proprio nome utente di GitHub al posto di `NOMEUTENTE` e la cartella giusta al posto di `es1`.

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
