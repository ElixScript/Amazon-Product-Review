# Analisis Sentimen Ulasan Produk Amazon
 
*Dashboard Power BI Interaktif - [Akses Dashboard](https://app.powerbi.com/view?r=eyJrIjoiZWQ4NGQ2MWYtMjNiYy00NmFjLTlhNjQtZmNlNTgxNmUwNDhjIiwidCI6ImFmMmMwNzM0LWNiNDItNDY0Zi1iNmJmLTJhMjQxYjZhZGE1NiIsImMiOjEwfQ%3D%3D)*

## 📌 Overview
Proyek ini melakukan analisis sentimen terhadap 568,454 ulasan produk Amazon menggunakan MongoDB sebagai penyimpanan data dan Python untuk pemrosesan serta pemodelan machine learning. Hasil analisis divisualisasikan dalam dashboard interaktif menggunakan Power BI.

## 📊 Dataset
- **Sumber**: Kaggle - Amazon Product Reviews
- **Jumlah Data**: 568,454 ulasan
- **Fitur**:
  - ProductId
  - UserId
  - ProfileName
  - HelpfulnessNumerator
  - HelpfulnessDenominator
  - Score (1-5)
  - Time (timestamp)
  - Summary
  - Text

## 🧠 Proses Analisis

### Preprocessing
1. Pembersihan HTML tag dan URL
2. Penghapusan tanda baca dan angka
3. Normalisasi karakter beraksen
4. Tokenisasi dan stopwords removal
5. Stemming dengan PorterStemmer
6. Feature engineering:
   - Panjang teks
   - Jumlah kata
   - Kepadatan kata
   - Polarisasi teks
   - Subjektivitas teks


## 📈 Hasil Utama

### Distribusi Sentimen

| Kategori Sentimen | Jumlah Ulasan | Persentase |
|-------------------|---------------|------------|
| Weakly Positive   | 304,220       | 53.54%     |
| Positive          | 172,781       | 30.41%     |
| Weakly Negative   | 50,800        | 8.94%      |
| Strongly Positive | 26,201        | 4.61%      |
| Neutral           | 7,797         | 1.37%      |
| Negative          | 5,305         | 0.93%      |
| Strongly Negative | 1,106         | 0.19%      |

### Performa Model
| Metric            | Nilai   |
|-------------------|---------|
| Training Accuracy | 0.9171  |
| Test Accuracy     | 0.9126  |
| F1 Score          | 0.9501  |
| AUC Score         | 0.9349  |


## 📚 Referensi
1. [TextBlob Documentation](https://textblob.readthedocs.io/)
2. [NLTK Documentation](https://www.nltk.org/)
3. [Scikit-learn Documentation](https://scikit-learn.org/)
4. [Power BI MongoDB Connector](https://learn.microsoft.com/en-us/power-query/connectors/mongodb)

## 👥 Kontributor
- Alia
- Bagus
- Ceiba
- Givari
- Kosmas
- Wibi
