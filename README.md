# 🧬 **Göğüs Kanseri Teşhisi: Makine Öğrenmesi Yaklaşımı**
### *Yapay Zeka Destekli Erken Teşhis ve Akıllı Sınıflandırma Sistemi*

<p align="center">
  <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">
</p>

<div align="center">

[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Status](https://img.shields.io/badge/Durum-Tamamland%C4%B1-success?style=for-the-badge)](https://github.com/caner-mercan)

</div>

---

## 📖 **Proje Hakkında**
Bu çalışma, tıp dünyasındaki en kritik konulardan biri olan göğüs kanseri teşhisini, **veri bilimi ve makine öğrenmesi** yöntemleriyle optimize etmeyi amaçlayan profesyonel bir projedir. Teknik bir eğitim sürecinin parçası olarak hazırlanan bu çalışma, veriden anlamlı sonuçlar çıkarma ve sınıflandırma yetkinliklerini bir araya getirmektedir. Hücre çekirdeği ölçümlerinden yola çıkarak, tümörlerin patolojik durumunu (**Malignant** / **Benign**) yüksek doğruluk oranıyla tahmin etmek hedeflenmiştir.

---

## 📊 **Veri Seti ve Değişken Analizi**

Projenin temelini oluşturan veri yapısı ve parametreler aşağıdaki tablolarda detaylandırılmıştır:

### **1. Veri Seti Genel Özeti**
| Parametre | Detay |
| :--- | :--- |
| **Toplam Örnek Sayısı** | 569 |
| **Özellik (Feature) Sayısı** | 30 |
| **Hedef Sınıflar** | Malignant (Kötü Huylu), Benign (İyi Huylu) |
| **Veri Kaynağı** | Breast Cancer Wisconsin (Diagnostic) |

### **2. İncelenen Hücre Özellikleri**
| Kategori | İncelenen Değişkenler |
| :--- | :--- |
| **Geometrik Veriler** | Yarıçap (Radius), Çevre (Perimeter), Alan (Area) |
| **Dokusallık** | Pürüzsüzlük (Smoothness), Doku (Texture) |
| **Karmaşıklık** | İçbükeylik (Concavity), Fraktal Boyut (Fractal Dimension) |

---

## 🧪 **Modelleme ve Performans Karşılaştırması**

En doğru teşhis sonucuna ulaşmak için farklı algoritmalar titizlikle test edilmiştir. Elde edilen başarı metrikleri şöyledir:

| Algoritma | Accuracy (Doğruluk) | Precision (Keskinlik) | Recall (Duyarlılık) | F1-Skoru |
| :--- | :---: | :---: | :---: | :---: |
| **Logistic Regression** | **%97.2** | 0.97 | 0.98 | 0.97 |
| **SVM (Linear Kernel)** | %96.5 | 0.96 | 0.97 | 0.96 |
| **Random Forest** | %95.8 | 0.95 | 0.96 | 0.95 |
| **K-Nearest Neighbors** | %94.4 | 0.94 | 0.95 | 0.94 |

> **📌 Kritik Not:** Tıbbi teşhislerde en hayati metrik **Recall** değeridir. Bu projede, gerçek hastaların yanlışlıkla "sağlıklı" olarak etiketlenmemesi (False Negative) için modeller bu yönde optimize edilmiştir.

---

## 🛠️ **Teknoloji ve Mimari Stack**
Projenin teknik altyapısı, veri analizi ve makine öğrenmesi odaklı modern kütüphaneler üzerine inşa edilmiştir:

* 🚀 **Dil:** `Python 3.x`
* 📊 **Veri Analizi:** `Pandas`, `NumPy`
* 🎨 **Görselleştirme:** `Matplotlib`, `Seaborn`
* 🧠 **ML Motoru:** `Scikit-Learn`
* 💻 **Geliştirme Ortamı:** `Jupyter Notebook`

---

## ⚙️ **Nasıl Çalıştırılır?**

Projeyi yerel bilgisayarınızda kurup çalıştırmak için aşağıdaki adımları sırasıyla uygulayın:

1. **Depoyu Klonlayın:** `git clone https://github.com/caner-mercan/makine-ogrenmesi.git`
   
2. **Bağımlılıkları Yükleyin:** `pip install pandas numpy matplotlib seaborn scikit-learn jupyter`
   
3. **Notebook'u Başlatın:** `jupyter notebook göğüs_kanseri.ipynb`

---

## 👨‍💻 **Geliştiriciler**

Bu proje, bir ekip çalışması olarak akademik standartlarda geliştirilmiştir:

| Geliştirici | Rol | Bağlantı |
| :--- | :--- | :--- |
| **Caner Mercan** | Veri Bilimi & ML Geliştirici | [GitHub](https://github.com/caner-mercan) |
| **Hamza Uludağ** | Veri Bilimi & ML Geliştirici | [GitHub](https://github.com/hamza-uludag) |

<p align="center">
  <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%">
</p>

<p align="center">
  <i>Bu proje, veri biliminin tıp alanındaki dönüştürücü gücünü keşfetmek amacıyla hazırlanmıştır.</i> <br>
  <b>© 2026 Caner Mercan & Hamza Uludağ</b>
</p>
