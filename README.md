# progettoLAB-IA
Progetto finale e tesi di laurea del corso Laboratorio di intelligenza artificiale.

- Yolo v4 object detection model trained on cloud in Google Colab.
- OCR performed by both EasyOCR and Pytesseract with comparison between the two.
- Credits:
    Training a custom Yolo v4 object detection model on cloud: https://github.com/theAIGuysCode/YOLOv4-Cloud-Tutorial
    Running a pre-trained custom object detection model: https://github.com/theAIGuysCode/tensorflow-yolov4-tflite

# ANPR.ipynb
-Versione del progetto che non utilizza machine learning ma esclusivamente computer vision. I risultati sono sicuramente meno accurati e spesso il modello fallisce riconoscimenti a prima vista molto semplici, tuttavia ho ritenuto interessante mostrare anche questa versione in quanto copre molti argomenti svolti nella prima parte del corso.

# OCRonly.ipynb
-Notebook realizzato con lo scopo di effettuare solo la fase di OCR di immagini di targhe già pronte (Ottenute magari effettuando object detection in locale su video e/o webcam)

# YOLOv4_Training.ipynb
-Notebook Colab utilizzato per addestrare il modello, nonostante fosse possibile scaricare e far girare la versione del modello per le targhe ho preferito addestrarlo personalmente, anche per non effettuare un semplice copia-incolla della versione del tutorial. L'addestramento ha richiesto all'incirca 3 ore utilizzando una GPU messa a disposizione da Colab e un "Trick" per non essere espulsi dalla sessione per inattività. La precisione del modello, basandosi sull'ultimo checkpoint, è di circa 89%.

# finalVersion.ipynb
-Notebook colab che unisce la fase di object detection a quella di optical character recognition. Quest'ultima fase è stata implementata totalmente da me e prevede l'utilizzo e il confronto di due diverse librerie EasyOCR e Pytesseract. Sfortunatamente non è possibile far girare l'object detector in modalità video e webcam all'interno del notebook ma bisognerà farlo in locale.

# commands.txt
-File di testo contenente i 4 comandi da eseguire in una shell "conda" dopo l'attivazione del virtual enviroment "yolov4-gpu", con lo scopo rispettivamente di attivare il modello YOLO v4 nell'enviroment convertendo i pesi addestrati in cloud nel formato tensorflow e far girare quest'ultimo su immagini, video e webcam.

