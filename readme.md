<!-- Descrizione:
Partendo dal markup della versione consegnata, creare uno slider usando Vue.
Usate i dati presenti, modificandone la posizione, in modo che siano utilizzabili nell'istanza di Vue in uso.
Bonus:
1 - Aggiungere le thumbnails che si illuminano quando la relativa immagine e' attiva
2-  Aggiungere un evento di click sulle thumbnails per rendere attiva l'immagine relativa
Consigli del giorno:
regola d'oro: riciclare ovunque possibile!
il riciclo spesso va a braccetto con le funzioni! Sapendole sfruttare bene, l'esercizio si riduce a poche righe -->

creo un ciclo v-for per slides sul div che contiene le immagini e le relative informazioni

associo i vari valori all'interno del array ai tag corrispondenti usando v-bind e {{}}

dichiaro una variabile activeindex = 0

creo 2 funzioni in methods 
    che aggiungano 1 se activeindex minore della lunghezza di slides - 1 altrenti activeindex = 0
    che sottraggano 1 fino a che activeindex e' maggiore di 0 altrimenti active index = lunghezza di slides - 1

creo un tag v-show all'interno del div item e pongo come condizione che index==activeindex

collego le 2 funzioni ai relativi bottoni nel html
