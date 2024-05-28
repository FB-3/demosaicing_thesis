# Demosaicizzazione mediante algoritmi di Interpolazione

Codici di Jupyter Notebook (Python) per Tesi di Laurea sulla demosaicizzazione.

## harmonic_interpolation.ipynb

Il Notebook contiene un algoritmo di *inpainting* basato sull'interpolazione 
delle equazioni differenziali di Laplace (*harmonic interpolation*).

Il *main* prende in input l'immagine $\verb|images/monet_adresse.jpg|$ e ne 
rende il 50% NaN (Not a Number). Dopodiché applica l'algoritmo sopracitato e
un algoritmo di demosaicizzazione semplice tramite pattern di Bayer.

In più, il codice calcola i tempi di esecuzione dell'algoritmo, 
il *mean_squared_error* (MSE) e il *structural similarity index
measure* (SSIM).

## python_interpolation.ipynb

In questo codice vengono applicati le routine di Python di interpolazione
per ogni layer di colore delle immagini:

* Interpolazione Lineare
* Interpolazione Nearest-Neighbors
* Interpolazione Nearest-Natural (Cubica)

Le immagini utilizzate provengono da un dataset di 24 immagini RAW Kodak:
> https://www.math.purdue.edu/~lucier/PHOTO_CD/

Il programma calcola i tempi di esecuzione dell'algoritmo, 
il *mean_squared_error* (MSE) e il *structural similarity index
measure* (SSIM).

## demosaicing.ipynb

Il programma applica il pattern di Bayer e l'algoritmo di demosaicizzazione
semplice al dataset delle 24 immagini RAW di Kodak.
