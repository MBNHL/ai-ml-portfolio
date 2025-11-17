# AI & ML Portfolio — Progetti Principali

Questo documento presenta una panoramica di due progetti NLP sviluppati su dataset reali e scenari applicativi complessi. I progetti combinano tecniche di Machine Learning, Natural Language Processing e Data Engineering scalabile.

---

## **Progetto 1 — Multilabel Toxic Comment Classification**
### **Obiettivo**
Sviluppare un sistema automatico di moderazione dei contenuti in grado di rilevare diversi tipi di tossicità nei commenti online. Il problema è di tipo **multilabel classification**, poiché ogni testo può appartenere contemporaneamente a più categorie tossiche.

### **Tecniche e Pipeline Utilizzate**
- Preprocessing testuale (pulizia, normalizzazione, tokenizzazione)
- Gestione dello sbilanciamento tramite class weights e loss pesata
- **Multilabel classification pipeline** con algoritmi ML
- Valutazione modelli con **precision, recall, F1 per ogni classe**
- Visualizzazione **matrici di confusione per classe**
- Analisi comparativa dei modelli con ottimizzazione soglia decisionale

### **Tecnologie**
`Python · Scikit-learn · TensorFlow · Keras · NLTK · Pandas · NumPy · Matplotlib · Seaborn · WordCloud`

### **Risultati principali**
- Miglioramento significativo nella rilevazione classi minoritarie tramite class-weighting
- Ottimizzazione della soglia per bilanciare tradeoff precision/recall
- Metriche multilabel dettagliate con analisi interpretabile

### **Possibili applicazioni reali**
- Moderazione automatica di commenti
- Sistemi anti-bullismo e prevenzione linguaggio ostile
- Analisi semantica per discovery e clustering informativo

### **Possibili estensioni future**
- Modelli basati su transformer (BERT, RoBERTa)
- Interpretabilità con SHAP/LIME
- Deploy come microservizio API / demo Streamlit

---

## **Progetto 2 — Wikipedia Structured Insights Extraction (PySpark NLP Pipeline)**
### **Obiettivo**
Costruire una pipeline scalabile per estrarre insight strutturati da articoli Wikipedia, collegando categorie tematiche con distribuzioni di topic ottenuti tramite **LDA Topic Modeling**.

### **Approccio Tecnico**
- Gestione dataset di grandi dimensioni con **PySpark DataFrame API**
- Preprocessing massivo su testo: tokenizzazione, stopword removal, feature extraction
- Costruzione modello **LDA su Spark ML**
- Aggregazione distribuzioni dei topic per categoria
- Conversione selettiva a Pandas per visualizzazioni avanzate
- Costruzione **heatmap di correlazione topic–categoria** per interpretazione semantica

### **Tecnologie**
`PySpark · Spark MLlib · Pandas · Matplotlib · Seaborn · Plotly · WordCloud` 

### **Risultati principali**
- Identificazione automatica di macro‑argomenti dominanti nei contenuti Wikipedia
- Rappresentazione di insight strutturati tramite visualizzazioni topic–categoria
- Pipeline progettata per scalabilità su dataset massivi

### **Possibili applicazioni reali**
- Motori di raccomandazione per contenuti
- Creazione automatica di tassonomie / knowledge base
- Analisi semantica per discovery e clustering informativo

### **Possibili estensioni future**
- Aggiunta coherence score e tuning avanzato numero topic
- BERTopic / embeddings semantici per confronto metodologico
- Versione orchestrabile con Docker o Airflow


