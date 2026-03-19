# K-Means Clustering con OpenMP

Questo progetto implementa l'algoritmo di clustering **K-Means** utilizzando un approccio di layout dati Structure of Arrays (SoA),in linguaggio C++, parallelizzato utilizzando **OpenMP** per migliorare le prestazioni su architetture multi-core.

## Descrizione
L'algoritmo K-Means è uno dei più noti metodi di apprendimento non supervisionato per il partizionamento di un set di dati in $K$ gruppi (cluster). 
Questa implementazione sfrutta il parallelismo a livello di thread per velocizzare:
1. Il calcolo delle distanze tra punti e centroidi.
2. L'assegnazione dei punti al cluster più vicino.
3. L'aggiornamento della posizione dei centroidi.

## 🛠 Prerequisiti
Per compilare ed eseguire il progetto, è necessario avere installato un compilatore che supporti OpenMP (come `gcc` o `clang`).

### Su Linux (Ubuntu/Debian)
```bash
sudo apt update
sudo apt install build-essential
