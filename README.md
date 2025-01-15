# Forecasting_WWTP

1) Matlab, contiene:
	-Corr_Reali.m codice per l'analisi di correlazione del Dataset Reale
	-Corr_Simulato.m  codice per l'analisi di correlazione del Dataset Simulato
	-Grafici_lab_real_soft.m Confronto Predizioni, Sensori e laboratorio
	-PCA_Biowin.m Prove di PCA per capire quali erano le migliori grandezze per stimare COD e TSS
	-PB_outlier_remove.mlx codice per rimuovere gli outlier dal Dataset reale su COD e TSS
	-PESCHIERA_LAB_4.xlx Dataset misure laboratorio
	-PESCHERIA_BORROMEO_ANN_last.xlsx Dataset reale senza outlier Rimossi
	-Biowin simulated data.xlsx Dataset Simulato
	-Dati_reali_stimati.xlsx contiene il dato Stimato dalla rete MLT (se non sbaglio) per fare confronto tra lab, probe e reti

2)Test_MLT_Training_Diversi Contiene i risultati di addestramento e test fatti con 1000 campioni, 1200, 1400 ... sulla rete MLT e il codice matlab per ricavare i vari indici statistici.

3) Codici_reti contiene tutte le ultime reti implementate sia su dataset simulato, reale, Mlt e LSTM, con input anche l'NNOX
	-Se c'è scritto Forecasting è LSTM
	-NNOX nel nome indica che si è usato l'NNOX come input
	-Se c'è scritto reale nel nome significa che usa il dataset reale
	-Gli ultimi codici con cui ho fatto prove sono quelli con pedice Nick
	-PESCHERIA_BORROMEO_ANN_seconda.xlsx contiene una maggiore rimozione di outlier su TSS rispetto agli altri