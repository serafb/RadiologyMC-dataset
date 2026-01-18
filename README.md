# Radiology Masterclass Dataset

Dataset di quiz radiologici estratto da [Radiology Masterclass](https://www.radiologymasterclass.co.uk/).

## Struttura

* 📁 **`images_clean`**: Immagini originali dei quiz.
* 📁 **`images_annotation`**: Immagini con soluzioni e annotazioni grafiche.
* 📄 **`tasks.json`**: File pronto per l'importazione in **Label Studio** (domande, riferimenti e soluzione).
* 📄 **`annotation_radiology.csv`** / **`.json`**: File esportato da Label Studio con le annotazioni (Sono presenti le coordinate dei **bounding box**).

> I file `tasks.json` e `annotation_radiology.csv` / `.json` contengono gli URL diretti alle immagini ospitate in questo repository. In questo modo è possibile visualizzare i dati in Label Studio istantaneamente, senza dover configurare storage locali o cloud esterni.

## Utilizzo
Importare uno dei seguenti file in un nuovo progetto su [Label Studio](https://labelstud.io/):
* Per visualizzare o modificare le annotazioni esistenti, importare il file  `annotation_radiology.csv` / `.json` (immagini con bounding box)
* Per creare nuove annotazioni da zero, importare il file `tasks.json`. (immagini originali senza bounding box)
