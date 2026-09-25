---
description: Crea la cartella di un'esercitazione o del progetto
---

Preparare la cartella `$1` di questo repository.

Prima di tutto il nome della cartella. Se `$1` è una variante riconoscibile di `esN` («esercizio 2», «e2», «Es 3») o del progetto, usare la forma standard (`es2`, `progetto`) e dirlo allo studente in una riga. Se invece il nome non è riconoscibile, o sembra provvisorio («es1 prova», «variante esercizio 1»), avvisare che con un nome così l'indirizzo pubblico e il collegamento con la consegna non funzioneranno, e chiedere se crearla ugualmente.

1. Leggere le specifiche su `https://codestesie.it/aa2627/ca/attivita/<cartella>/`. Se l'indirizzo non risponde, avvisare e fermarsi: l'attività non è ancora stata pubblicata.
2. Creare la cartella con tre file.
   - `index.html`: pagina in italiano con `<meta charset="utf-8">`, il titolo dell'attività, lo script di p5.js `https://cdn.jsdelivr.net/npm/p5@2.3.3/lib/p5.min.js`, il proprio `style.css` e `sketch.js`.
   - `style.css`: solo l'essenziale, cioè margini a zero e la tela come blocco.
   - `sketch.js`: in cima, come commenti, l'obiettivo dell'attività e l'elenco dei vincoli ricavati dalle specifiche; poi le variabili dei parametri con un commento ciascuna.
3. Scrivere in `sketch.js` uno **sketch di base funzionante**: la soluzione più diretta e più ovvia delle specifiche, quella che verrebbe a chiunque le passi a un modello linguistico. Codice minimo, nessuna variazione personale.
4. Aggiungere la voce all'elenco nell'`index.html` della radice, togliendo la riga «Ancora nessun lavoro pubblicato» se è ancora lì.
5. Chiudere dicendo in modo esplicito che quello è il punto di partenza comune a tutti e non il lavoro da consegnare, e chiedere allo studente che cosa vuole ottenere.

**Non proporre un elenco di direzioni da scegliere**: l'idea deve venire da lui, altrimenti l'esercitazione diventa una scelta fra opzioni preconfezionate e i lavori si somigliano tutti. Se non sa da dove partire, aiutarlo con domande sul risultato che ha in mente, non con un menù di alternative.

Nelle richieste successive, assistere sulle parti complesse e lasciare a lui le modifiche semplici: quando si tratta di cambiare numeri, colori o proporzioni, dire dove intervenire e invitarlo a farlo direttamente nel codice.
