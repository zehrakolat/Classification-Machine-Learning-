🫀 Heart Disease Risk Prediction using Machine Learning
Bu proje, Kaggle üzerindeki yapılandırılmış tıbbi verileri kullanarak bireylerin kalp hastalığı riskini tahmin etmek amacıyla geliştirilmiştir1111. Proje kapsamında veri ön işleme, detaylı keşifçi veri analizi (EDA), temel sınıflandırma modelleri ve ileri seviye topluluk (ensemble) öğrenme teknikleri uygulanmıştır.
🚀 Proje Özellikleri
•	Kapsamlı Veri Ön İşleme: Eksik veri kontrolü, aykırı değer (outlier) analizi ve StandardScaler ile özellik ölçeklendirme.
•	Dengesiz Veri Yönetimi: Eğitim setindeki sınıf dengesizliğini gidermek için SMOTE (Synthetic Minority Over-sampling Technique) uygulaması.
•	Geniş Model Yelpazesi: * Temel Modeller: Logistic Regression, Naive Bayes, SVM.
o	Ensemble Modeller: Random Forest, Gradient Boosting (GBM), XGBoost.
•	Açıklanabilir Yapay Zeka (XAI): Model tahminlerini yorumlamak ve şeffaflık sağlamak için SHAP analizi entegrasyonu.
•	Kullanıcı Arayüzü: En başarılı model olan GBM üzerine kurulu, gerçek zamanlı tahmin yapan bir arayüz.
📊 Önemli Bulgular ve Analizler
Keşifçi Veri Analizi (EDA)
•	Korelasyon: Yaş (Age), kalp hastalığı riski ile en güçlü bağlantıya (0.29) sahip değişkendir.
•	Özellik Dağılımı: Verilerin çoğu normalleştirilmiş ölçekte -1.5 ile +1.5 arasında dağılmış olup, belirgin bir aykırı değer saptanmamıştır.
•	Karmaşıklık: Pair plot analizleri, sağlıklı ve hasta bireylerin verilerinin iç içe geçtiğini, bu nedenle basit doğrusal modellerin yetersiz kaldığını göstermiştir.
Model Performansı
Model	Accuracy (Test)	F1-Score	Karakteristik
GBM (Winner)	0.63	0.63	En dengeli sonuçlar ve en iyi genelleme yeteneği.
SVM	0.62	0.63	En tutarlı doğrusal olmayan temel model.
Logistic Reg.	0.61	0.62	Kararlı ve yorumlanabilir sonuçlar.
Random Forest	0.61	0.52	Eğitim setinde %92 F1 başarısına rağmen yüksek aşırı öğrenme (overfitting).
🛠️ Kullanılan Araçlar
•	Dil: Python 
•	Kütüphaneler: Pandas, Matplotlib, Seaborn, Scikit-learn, Imblearn (SMOTE), SHAP.

