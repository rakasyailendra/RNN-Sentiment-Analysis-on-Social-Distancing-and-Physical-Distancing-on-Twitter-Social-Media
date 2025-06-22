# 🧠 Sentiment Analysis on Social Distancing and Physical Distancing on Twitter using RNN  
**MATA KULIAH : KECERDASAN BUATAN (A081)**  
**Dosen Pengampu : Yisti Vita Via, S.ST. M.Kom.**

---

## 📘 Deskripsi Proyek  
Proyek ini bertujuan untuk menganalisis sentimen masyarakat terhadap istilah *Social Distancing* dan *Physical Distancing* di media sosial **Twitter** menggunakan teknik **Natural Language Processing (NLP)** dan algoritma **Recurrent Neural Network (RNN)** berbasis **LSTM**. Data yang digunakan adalah tweet berbahasa Indonesia yang dibersihkan dan diklasifikasikan menjadi sentimen **positif** atau **negatif**.

---

## 👥 Disusun oleh:
- **M. Rakha Syailendra** (23081010019)
- **Abril Berliando C.**   (23081010186) 

---

## 🛠️ Tools & Teknologi
- Python 3.x  
- TensorFlow / Keras  
- Pandas, NumPy  
- Gensim (Word2Vec)  
- Matplotlib & Seaborn  
- NLTK + Sastrawi (untuk bahasa Indonesia)  
- Twitter Dataset (CSV)  
- Wikipedia Dump untuk training Word2Vec

---

## 🧪 Proses Utama
1. **Preprocessing**: Pembersihan teks, penghapusan slang menggunakan kamus alay, normalisasi huruf besar, dan tokenisasi.
2. **Pembuatan Word Embedding**: Menggunakan data Wikipedia bahasa Indonesia untuk melatih model **Word2Vec**.
3. **Modeling**: Arsitektur model LSTM dengan layer embedding, dropout, dan output sigmoid.
4. **Evaluasi**: Menggunakan akurasi, confusion matrix, dan classification report.
5. **Prediksi Sentimen Baru**: Fungsi prediksi untuk input teks manual.
---

## 📈 Hasil Evaluasi
- Model menghasilkan akurasi cukup baik dalam klasifikasi tweet.
- Visualisasi hasil termasuk:
  - Histogram panjang tweet
  - Confusion matrix untuk data latih dan uji
  - Classification report (precision, recall, F1-score)

---

## ⚙️ Contoh Penggunaan Fungsi Prediksi
```python
text = "Social Distancing ini bikin aku jadi scroll tiktok mulu wkwkw"
label, prob = predict_new_sentiment(text)
print(f"Hasil: {label}, Probabilitas: {prob}")

