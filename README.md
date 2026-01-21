# Radiology Masterclass Dataset

Dataset di quiz radiologici estratto da [Radiology Masterclass](https://www.radiologymasterclass.co.uk/).

## Struttura
- 📁 **`images_clean`**    Immagini originali dei quiz con singola radiografia.
- 📁 **`images_annotation`**    Immagini con singola radiografia corredate da soluzioni e annotazioni grafiche.

- 📁 **`images-2rx_clean`**    Immagini originali dei quiz che presentano due radiografie per caso, unite in un’unica immagine.
- 📁 **`images-2rx_annotation`**    Immagini con doppia radiografia unite in un’unica immagine, comprensive di soluzioni e annotazioni grafiche.

- 📄 **`tasks.json`**    File pronto per l’importazione in **Label Studio**, contenente domande, riferimenti e soluzioni per i quiz con singola radiografia.
- 📄 **`tasks_2rx.json`**    File pronto per l’importazione in **Label Studio**, contenente domande, riferimenti e soluzioni per i quiz con doppia radiografia.

### Risultati finali
- 📁 **`labelled`**    Directory contenente i file di annotazione esportati da Label Studio.
  - 📄 ** `annotation_radiology.csv` / `.json` / `.zip`  (YOLO with img)      Annotazioni strutturate con coordinate dei **bounding box** per le immagini a singola radiografia.
  - (**TODO**)📄 ** `annotation_radiology_2rx.csv` / `.json` / `.zip`  (YOLO with img)      Annotazioni per le immagini con doppia radiografia (**in preparazione**).


> I file contengono gli URL diretti alle immagini ospitate in questo repository. In questo modo è possibile visualizzare i dati in Label Studio istantaneamente, senza dover configurare storage locali o cloud esterni.

## Utilizzo
Importare uno dei seguenti file in un nuovo progetto su [Label Studio](https://labelstud.io/):
* Per visualizzare o modificare le annotazioni esistenti, importare il file  `annotation_radiology.csv` / `.json` / `.zip  (YOLO with img)`
* Per creare nuove annotazioni da zero, importare il file `tasks.json`

## TODO
Non è stato ancora prodotto annotation_radiology per i quiz che presentano due radiografie per caso, unite in un’unica immagine.
