# 🎗️ Makine Öğrenmesi ile Göğüs Kanseri Teşhisi

Bu proje, tıbbi veri setleri üzerinde makine öğrenmesi tekniklerini kullanarak **Göğüs Kanseri (Breast Cancer)** teşhisi ve sınıflandırması yapmaktadır. Çalışma kapsamında hücre özelliklerine dayalı olarak tümörlerin **İyi Huylu (Benign)** veya **Kötü Huylu (Malignant)** olarak ayrıştırılması hedeflenmiştir.

---

## 📝 Proje Hakkında
Bu çalışma, bir teknik eğitim sürecinin parçası olarak geliştirilmiştir ve veri bilimi metodolojilerini uçtan uca kapsamaktadır. Projenin temel amacı, teşhis süreçlerinde insan hatasını minimize edebilecek yüksek doğruluklu bir tahmin modeli oluşturmaktır.

## 📊 Veri Seti Detayları
Projede **UCI Machine Learning Repository** üzerinden sağlanan "Breast Cancer Wisconsin (Diagnostic)" veri seti kullanılmıştır.
* **Örnek Sayısı:** 569.
* **Öznitelik Sayısı:** 30 (Yarıçap, doku, çevre, alan vb.).
* **Hedef Değişken:** Tanı (M/B).

## 🛠️ Kullanılan Teknolojiler
Proje geliştirilirken aşağıdaki teknik araçlar ve kütüphaneler kullanılmıştır:
* **Python**: Temel programlama dili.
* **Pandas & NumPy**: Veri işleme ve matris operasyonları.
* **Matplotlib & Seaborn**: Veri görselleştirme ve korelasyon analizleri.
* **Scikit-Learn**: Model eğitimi, veri ölçeklendirme ve performans metrikleri.

## 📈 Uygulama Adımları
1. **Veri Ön İşleme:** Eksik verilerin kontrolü ve `StandardScaler` ile verilerin normalize edilmesi.
2. **Keşifçi Veri Analizi (EDA):** Tümör özelliklerinin birbirleriyle olan ilişkilerinin heatmap üzerinden incelenmesi.
3. **Model Eğitimi:** Lojistik Regresyon, Random Forest ve SVM gibi algoritmaların uygulanması.
4. **Değerlendirme:** Karmaşıklık matrisi (Confusion Matrix) ve sınıflandırma raporları ile modelin test edilmesi.

## 📊 Model Performansı
Yapılan testler sonucunda elde edilen başarı oranları aşağıdaki gibidir:

| Metrik | Değer |
| :--- | :--- |
| Doğruluk (Accuracy) | %XX |
| Hassasiyet (Precision) | 0.XX |
| Duyarlılık (Recall) | 0.XX |
| F1-Skoru
