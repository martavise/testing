# HTML

## `index.html`
È il modo più semplice per creare e gestire una landing page. È la prima pagina caricata quando si apre un sito web.

## Shortcuts and elements

In **VS Code** posso generare la struttura generale di una pagina HTML digitando <strong>!</strong> e premendo `Enter`.

### Testo e formattazione

- `<p>` — per creare paragrafi.
- `<strong>` — per il grassetto.
- `<em>` — per il corsivo.
- `<h1>` – `<h6>` — per creare titoli di diverse dimensioni.
- `<br>` — per andare a capo.
- `<hr>` — per inserire una linea orizzontale.

### Liste

- `<ul>` — per creare una lista puntata (unordered list).
- `<ol>` — per creare una lista numerata (ordered list).
- `<li>` — per definire un elemento della lista.

### Immagini

- `<img>` — per inserire un'immagine.
- `src` — per specificare il percorso o l'URL dell'immagine.
- `alt` — per inserire una descrizione alternativa dell'immagine.
- `width` — per definire la larghezza.
- `height` — per definire l'altezza.


esempio:
```
<img src="immagine.jpg" alt="Descrizione immagine" width="300">
```

### Hyperlink (collegamenti)

- `<a>` — per creare un collegamento (anchor).
- `href` — per specificare l'indirizzo della pagina di destinazione.
- `target="_blank"` — per aprire il collegamento in una nuova scheda.


Posso anche collegare pagine nel mio progetto, in quel caso il path non conterrà https.

esempio:
```
<a href="https://www.google.com">Vai a Google</a>
```

Per aprire il link in una nuova scheda:
```
<a href="https://www.google.com" target="_blank" rel="noopener noreferrer">
  Vai a Google
</a>
```


