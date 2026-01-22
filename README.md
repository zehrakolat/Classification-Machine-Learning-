# 🫀 Heart Disease Risk Prediction using Machine Learning

[cite_start]Bu proje, Kaggle üzerindeki yapılandırılmış tıbbi verileri kullanarak bireylerin kalp hastalığı riskini tahmin etmek amacıyla geliştirilmiştir[cite: 1013, 1563]. [cite_start]Proje kapsamında veri ön işleme, detaylı keşifçi veri analizi (EDA), temel sınıflandırma modelleri ve ileri seviye topluluk (ensemble) öğrenme teknikleri uygulanmıştır[cite: 1555].

## 🚀 Proje Özellikleri

* [cite_start]**Kapsamlı Veri Ön İşleme:** Eksik veri kontrolü, aykırı değer (outlier) analizi ve `StandardScaler` ile özellik ölçeklendirme[cite: 1064, 1158, 1245].
* [cite_start]**Dengesiz Veri Yönetimi:** Eğitim setindeki sınıf dengesizliğini gidermek için **SMOTE** (Synthetic Minority Over-sampling Technique) uygulaması[cite: 1281].
* **Geniş Model Yelpazesi:**
    * [cite_start]**Temel Modeller:** Logistic Regression, Naive Bayes, SVM[cite: 2083].
    * [cite_start]**Ensemble Modeller:** Random Forest, Gradient Boosting (GBM), XGBoost[cite: 2110].
* [cite_start]**Açıklanabilir Yapay Zeka (XAI):** Model tahminlerini yorumlamak ve şeffaflık sağlamak için **SHAP** analizi entegrasyonu[cite: 2203].
* [cite_start]**Kullanıcı Arayüzü:** En başarılı model olan **GBM** üzerine kurulu, gerçek zamanlı tahmin yapan bir arayüz[cite: 2201].

## 📊 Önemli Bulgular ve Analizler

### Keşifçi Veri Analizi (EDA)
* [cite_start]**Korelasyon:** Yaş (Age), kalp hastalığı riski ile en güçlü bağlantıya (**0.29**) sahip değişkendir[cite: 1443, 1520].
* [cite_start]**Özellik Dağılımı:** Verilerin çoğu normalleştirilmiş ölçekte -1.5 ile +1.5 arasında dağılmış olup, belirgin bir aykırı değer saptanmamıştır[cite: 1407].
* [cite_start]**Karmaşıklık:** Pair plot analizleri, sağlıklı ve hasta bireylerin verilerinin iç içe geçtiğini, bu nedenle basit doğrusal modellerin yetersiz kaldığını göstermiştir[cite: 1456, 1528].



### Model Performansı

| Model | Accuracy (Test) | F1-Score | Karakteristik |
| :--- | :---: | :---: | :--- |
| **GBM (Winner)** | **0.63** | **0.63** | [cite_start]En dengeli sonuçlar ve en iyi genelleme yeteneği[cite: 2182, 2192]. |
| **SVM** | 0.62 | 0.63 | [cite_start]En tutarlı doğrusal olmayan temel model[cite: 2096, 2182]. |
| **Logistic Reg.** | 0.61 | 0.62 | [cite_start]Kararlı ve yorumlanabilir sonuçlar[cite: 2182, 2184]. |
| **Random Forest** | 0.61 | 0.52 | [cite_start]Eğitimde %92 F1 başarısına rağmen yüksek overfitting[cite: 2182, 2413]. |



## 🛠️ Kullanılan Araçlar
* [cite_start]**Dil:** Python [cite: 1537]
* [cite_start]**Kütüphaneler:** Pandas, Matplotlib, Seaborn, Scikit-learn, Imblearn (SMOTE), SHAP[cite: 1537].

## 📈 Sınıf Dağılımı (Pre-SMOTE)
* [cite_start]**Sağlıklı (0):** 1878 örnek (%61.2)[cite: 1176].
* [cite_start]**Hasta (1):** 1191 örnek (%38.8)[cite: 1177].
