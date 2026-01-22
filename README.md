# Radiology Masterclass Dataset

Dataset di quiz radiologici estratto da [Radiology Masterclass](https://www.radiologymasterclass.co.uk/).

## Struttura
- 📁 **`images_clean`**    Immagini originali dei quiz con singola radiografia per domanda.
- 📁 **`images_annotation`**    Immagini con singola radiografia per domanda, comprensive di annotazioni grafiche.

- 📁 **`images-2rx_clean`**    Immagini originali dei quiz con due radiografie per domanda, unite in un’unica immagine.
- 📁 **`images-2rx_annotation`**    Immagini con due radiografie per domanda, unite in un’unica immagine, comprensive di annotazioni grafiche.

- 📄 **`tasks.json`**    File pronto per l’importazione in **Label Studio**, contenente domande, riferimenti e soluzioni per i quiz con singola radiografia.
- 📄 **`tasks_2rx.json`**    File pronto per l’importazione in **Label Studio**, contenente domande, riferimenti e soluzioni per i quiz con doppia radiografia.


**Dataset esportati da Label Studio:**
- 📁 **`labelled`**    Directory contenente i dataset esportati da Label Studio con le coordinate dei bounding-box.
  - 📁  **`annotation_radiology_1rx :`**  📄`.csv` / `.json` / `.zip` (YOLO with img)    Dataset con le coordinate dei **bounding box** per le immagini a singola radiografia.
  - 📁  **`annotation_radiology_2rx :`**  (**TODO**) 📄`.csv` / `.json` / `.zip` (YOLO with img)    Dataset con le coordinate dei **bounding box** per le immagini a  doppia radiografia (**in preparazione**).

> I dataset contengono gli URL diretti alle immagini ospitate in questo repository nelle rispettive cartelle 📁`images`. In questo modo è possibile visualizzare i dati in Label Studio istantaneamente, senza dover configurare storage locali o cloud esterni.

**Label Studio labelling interface:**
Template di esempio
  - 📄  `labelling-interface_label-studio.txt` Template per la Labelling interface in Label Studio. Il contenuto del file deve essere copiato in `Settings` / `Labeling Interface` `(code)` del nuovo progetto creato.

## Utilizzo
Importare uno dei seguenti file in un nuovo progetto su [Label Studio](https://labelstud.io/):
* Per visualizzare o modificare le annotazioni esistenti, importare il file da `labelled`
* Per creare nuove annotazioni da zero, importare il file `tasks.json` o `tasks_2rx.json`.

## TODO
Non è stato ancora prodotto annotation_radiology per i quiz che presentano due radiografie per caso, unite in un’unica immagine.
