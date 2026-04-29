# makina-öğrenmesi
gögüs kanseri tahmini 

Bu proje, hücre özelliklerine dayanarak tümörlerin Kötü Huylu (Malignant) veya İyi Huylu (Benign) olup olmadığını tahmin etmeyi amaçlamaktadır. Projede veri ön işleme, ölçeklendirme ve temel makine öğrenmesi sınıflandırma algoritmaları (Logistic Regression ve Random Forest) kullanılmış, modellerin performansları karşılaştırılmıştır.

Kullanılan Teknolojiler ve Kütüphaneler
Dil: Python
Geliştirme Ortamı: Google Colab / Jupyter Notebook
Veri Manipülasyonu: Pandas
Görselleştirme: Matplotlib, Seaborn
Makine Öğrenmesi: Scikit-Learn

Proje Adımları (İş Akışı)
Veri Ön İşleme (Data Preprocessing): * Modeli yanıltmaması adına hedef değişkenle ilgisi olmayan id ve boş olan Unnamed: 32 sütunları veri setinden çıkarıldı.
Hedef değişken olan diagnosis (teşhis) sütunundaki kategorik veriler sayısallaştırıldı: Kötü huylu (M) 1, iyi huylu (B) 0 olarak etiketlendi.
Veri Görselleştirme: Hedef değişkenin sınıflar arası dağılımı Seaborn kullanılarak görselleştirildi.
Özellik Ölçeklendirme (Feature Scaling): Farklı birimlerdeki verilerin modeli domine etmesini engellemek için StandardScaler kullanılarak veriler standartlaştırıldı.

Model Eğitimi: Veri seti %80 Eğitim (Train) ve %20 Test olacak şekilde ikiye ayrıldı. Logistic Regression ve Random Forest algoritmaları kullanılarak modeller eğitildi.

Sonuçlar ve Performans Karşılaştırması
İki farklı makine öğrenmesi modeli test verisi üzerinde değerlendirilmiş ve aşağıdaki sonuçlar elde edilmiştir:

Logistic Regression:

Doğruluk (Accuracy): %97.37
Random Forest:
Doğruluk (Accuracy): %96.49
Kesinlik (Precision): %97.56
Duyarlılık (Recall): %93.02
F1-Score: 0.9524

Her iki model de veriyi sınıflandırmada çok başarılı sonuçlar vermiştir. Lojistik Regresyon genel doğruluk oranında çok küçük bir farkla öne çıkarken, Random Forest modelinin Karmaşıklık Matrisi (Confusion Matrix) incelendiğinde yanlış negatif (gerçekte hasta olup sağlıklı denilen) sayısının sadece 3 olduğu görülmüştür.
