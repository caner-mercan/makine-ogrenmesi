# 🧬 **Breast Cancer Diagnosis: A Machine Learning Approach**
### *Erken Teşhis Hayat Kurtarır: Makine Öğrenmesi ile Akıllı Sınıflandırma*

<p align="center">
  <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">
</p>

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)](https://github.com/caner-mercan)

</div>

---

## 📖 **Proje Vizyonu**
Bu çalışma, tıp dünyasındaki en kritik sorunlardan biri olan göğüs kanseri teşhisini, **veri bilimi ve yapay zeka** yöntemleriyle optimize etmeyi amaçlayan akademik tabanlı bir projedir. Hücre çekirdeği ölçümlerinden yola çıkarak, tümörlerin patolojik durumunu (Malignant/Benign) %95+ doğruluk oranıyla tahmin etmek hedeflenmiştir.

---

## 🛠️ **Teknoloji ve Mimari Stack**
Projenin "arka yüzü" tamamen verimlilik ve akademik doğruluk üzerine inşa edilmiştir:

* 🚀 **Core:** `Python 3.x`
* 📊 **Data Analysis:** `Pandas`, `NumPy`
* 🎨 **Visual Engineering:** `Matplotlib`, `Seaborn`
* 🧠 **ML Engine:** `Scikit-Learn` (Model Pipeline & Cross-validation)
* 💻 **Environment:** `Jupyter Notebook`

---

## 🔄 **Veri Bilimi Pipeline (Yaşam Döngüsü)**

### 🔍 **1. Keşifçi Veri Analizi (EDA)**
Ham veri üzerinde yapılan derinlemesine incelemelerle, hangi hücre özelliklerinin kanser teşhisinde "anahtar" rol oynadığı belirlenmiştir.
* **Korelasyon Analizi:** Özellikler arasındaki ilişkiler Isı Haritası (Heatmap) ile görselleştirildi.
* **Dağılım Analizi:** Box-plot ve Histogramlar ile verideki aykırı değerler (outliers) tespit edildi.

### ⚙️ **2. Özellik Mühendisliği (Preprocessing)**
* **Normalizasyon:** Modellerin daha hızlı yakınsaması için `StandardScaler` kullanılarak veriler normalize edildi.
* **Encoding:** Hedef değişkenler (M/B) sayısal forma dönüştürüldü.

### 🧪 **3. Modelleme Stratejisi**
Aşağıdaki modern algoritmalar performans açısından karşılaştırılmıştır:
1.  **Logistic Regression** (Baseline model)
2.  **Support Vector Machines (SVM)**
3.  **Random Forest**
4.  **K-Nearest Neighbors (KNN)**

---

## 📊 **Performans Metrikleri**

| Algoritma | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Logistic Regression** | %97.2 | 0.97 | 0.98 | 0.97 |
| **SVM** | %96.5 | 0.96 | 0.97 | 0.96 |
| **Random Forest** | %95.8 | 0.95 | 0.96 | 0.95 |

> **📌 Kritik Not:** Tıbbi verilerde en önemli metrik **Recall** değeridir. Bu projede, gerçekte hasta olan birine "sağlıklı" denme oranı (False Negative) minimize edilmiştir.

---

## 📂 **Dosya Yapısı**
```text
├── göğüs_kanseri.ipynb   # Ana analiz ve modelleme dosyası
├── data/                 # Kullanılan ham veri setleri
├── images/               # Grafik ve görsel çıktılar
└── requirements.txt      # Bağımlılıklar listesi
