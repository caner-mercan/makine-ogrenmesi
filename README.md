# makina-öğrenmesi
gögüs kanseri tahmini 

## Proje Özeti
Bu proje, hücre özelliklerine dayanarak tümörlerin **Kötü Huylu (Malignant)** veya **İyi Huylu (Benign)** olup olmadığını tahmin etmeyi amaçlamaktadır. Projede veri ön işleme, ölçeklendirme ve temel makine öğrenmesi sınıflandırma algoritmaları (Logistic Regression ve Random Forest) kullanılmış, modellerin performansları karşılaştırılmıştır.

## Kullanılan Teknolojiler ve Kütüphaneler
* **Dil:** Python
* **Geliştirme Ortamı:** Google Colab / Jupyter Notebook
* **Veri Manipülasyonu:** Pandas
* **Görselleştirme:** Matplotlib, Seaborn
* **Makine Öğrenmesi:** Scikit-Learn

## Proje Adımları (İş Akışı)
1. **Veri Ön İşleme (Data Preprocessing):** Modeli yanıltmaması adına hedef değişkenle ilgisi olmayan `id` ve boş olan `Unnamed: 32` sütunları veri setinden çıkarıldı. Hedef değişken olan `diagnosis` (teşhis) sütunundaki kategorik veriler sayısallaştırıldı: Kötü huylu (M) `1`, iyi huylu (B) `0` olarak etiketlendi.
2. **Veri Görselleştirme:** Hedef değişkenin sınıflar arası dağılımı Seaborn kullanılarak görselleştirildi.
3. **Özellik Ölçeklendirme (Feature Scaling):** Farklı birimlerdeki verilerin modeli domine etmesini engellemek için `StandardScaler` kullanılarak veriler standartlaştırıldı.
4. **Model Eğitimi:** Veri seti %80 Eğitim (Train) ve %20 Test olacak şekilde ikiye ayrıldı. Lojistik Regresyon ve Random Forest algoritmaları kullanılarak modeller eğitildi.

## Sonuçlar ve Performans Karşılaştırması
İki farklı makine öğrenmesi modeli test verisi üzerinde değerlendirilmiş ve aşağıdaki sonuçlar elde edilmiştir:

* **Logistic Regression:**
  * **Doğruluk (Accuracy):** %97.37
* **Random Forest:**
  * **Doğruluk (Accuracy):** %96.49
  * **Kesinlik (Precision):** %97.56
  * **Duyarlılık (Recall):** %93.02
  * **F1-Score:** 0.9524

## Nasıl Çalıştırılır?
Projeyi kendi bilgisayarınızda veya yerel ortamınızda çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

1. **Projeyi Klonlayın:**
   git clone https://github.com/caylak36-oss/makina-renmesi.git

2. **Gerekli Kütüphaneleri Kurun:**
   Projeyi sorunsuz çalıştırabilmek için Python ortamınızda temel veri bilimi kütüphanelerinin yüklü olması gerekir. Terminal veya komut satırınıza şu kodu yazarak kurulum yapabilirsiniz:
   pip install pandas scikit-learn matplotlib seaborn

3. **Projeyi Açın ve Çalıştırın:**
   * İndirdiğiniz klasörün içindeki `gögüs_kanseri.ipynb` dosyasını Jupyter Notebook, JupyterLab veya Google Colab üzerinden açın.
   * Eğer Google Colab kullanıyorsanız, projede kullanılan veri setini çalışma ortamına yüklemeyi unutmayın.
   * Kod hücrelerini baştan sona sırasıyla çalıştırarak model sonuçlarını ve grafikleri kendi ekranınızda inceleyebilirsiniz.
