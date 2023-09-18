# Progetto-Editoria-2023
## Introduzione

Questo progetto nasce dalla volontà di preservare e condividere le ricette della tradizione familiare in un formato moderno e accessibile.

Tutto ha avuto origine da un antico libro di ricette, un'eredità di mia nonna che aveva già vissuto una trasformazione simile in passato.

Portare le nostre ricette familiari nel mondo digitale è stata una sfida, ma credo che ciò che abbiamo creato non deluderà. Questa collezione digitale non sarà solo un archivio di gustosi ricordi per le future generazioni, ma anche un compagno insostituibile per gli amanti della cucina.

Con la sua forma digitale, le nostre ricette saranno a portata di mano per tutti, ovunque e in qualsiasi momento, rendendo facile la condivisione di questi tesori culinari con chi desideriamo. Questo sforzo sottolinea il nostro impegno nel preservare e promuovere la nostra eredità culinaria di famiglia.

## Utilizzo

### Fase 1 : Trasformazione

All'interno della cartella `Utility`, troverai gli strumenti essenziali per la conversione. Per iniziare:

> Nota: Assicurati di aver installato pandoc per eseguire correttamente il programma ([pandoc install](https://pandoc.org/installing.html))

1. Apri il terminale nella cartella `Utility`.
2. Esegui il seguente comando per avviare il convertitore:
   
   ```
   python /percorso/convertitore.py
   ```

3. Dopo averlo lanciato, inserisci il percorso del file da convertire, come:

   ```
   esempi/polpettone-marinara.md
   ```

Dopo questi passaggi, otterrai i file convertiti in formati .html e .xhtml. La procedura è ora terminata.

### Fase 2 : Inserimento pagina e-book

Per aggiungere una nuova ricetta, segui i passi qui indicati:

> Nota: Sebbene le seguenti istruzioni siano specifiche per l'editor Sigil (consigliato), puoi utilizzare un altro editor di tua scelta. [Scarica Sigil da qui](https://sigil-ebook.com/sigil/download/).

1. Avvia Sigil.
2. Clicca sull'icona a forma di cartella `apri` e seleziona il tuo ricettario.
3. All'interno della sezione `Text`, posiziona il cursore dove desideri inserire la nuova pagina.
4. Seleziona l'icona *"aggiungi file esistenti"* (rappresentata da un simbolo di più) e scegli il file .xhtml che hai creato nella fase precedente.

#### Unisco file - ePub 

Per compilare diversi file in un unico epub, assicurati di avere tutti i file desiderati in una cartella, rispettando la struttura richiesta dal formato epub.

Dopo aver sistemato i file, esegui i seguenti comandi nel terminale:

```shell
zip -X0 nome_file.epub mimetype
zip -rDX9 nome_file.epub * -x mimetype
```

