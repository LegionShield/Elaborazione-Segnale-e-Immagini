# Elaborazione delle Immagini - Algoritmi e Script

Benvenuto in questa repository! Qui troverai una raccolta di script sviluppati in MATLAB/Octave dedicati all'elaborazione dei segnali e alle tecniche fondamentali di **Image Processing**.

## 📌 Contenuti del Progetto

Il codice esplora diverse tecniche matematiche e di manipolazione delle immagini, divise nelle seguenti aree principali:

### 1. Analisi in Frequenza (FFT)
* Calcolo della Trasformata di Fourier Veloce (FFT) di un segnale nel dominio del tempo.
* Gestione dell'aliasing e definizione dell'asse delle frequenze (Frequenza di Nyquist).
* Centratura dello spettro delle frequenze tramite `fftshift` per una corretta visualizzazione.

### 2. Cross-Correlazione a Basso Livello
* Implementazione del **Template Matching** tramite cross-correlazione normalizzata (`normxcorr2`).
* Ricerca delle coordinate assolute di un pattern (template) all'interno di un'immagine più grande e calcolo dell'offset esatto.

### 3. Operatori Puntuali (Ottimizzati con LUT)
Applicazione di filtri per la modifica dell'intensità dei pixel. Tutti gli script utilizzano le **Look-Up Table (LUT)** e la vettorializzazione per garantire prestazioni massime ed evitare cicli lenti sull'intera immagine.
* **Negativa:** Inversione dei valori dei pixel.
* **Stretching:** Espansione lineare del contrasto tra un nuovo minimo e massimo.
* **Binarizzazione:** Divisione netta in bianco e nero in base a un valore di soglia.
* **Clamping:** Taglio dei valori fuori da un range specifico (min/max).
* **Trasformazione Logaritmica:** Compressione della gamma dinamica per far risaltare i dettagli scuri.
* **Trasformazione di Potenza (Gamma Correction):** Regolazione non lineare per schiarire o scurire l'immagine.

## 🚀 Tecnologie Utilizzate
* MATLAB / GNU Octave

## 👤 Autore
* **legion**
