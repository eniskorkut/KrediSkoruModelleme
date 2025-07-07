NOT : https://www.kaggle.com/c/home-credit-default-risk/overview 'den önce verileri indirin.
# Açıklanabilir Yapay Zeka (XAI) ile Kredi Skorlama Modeli

Bu proje, finans sektöründeki "kara kutu" problemini çözmeyi amaçlayan uçtan uca bir makine öğrenmesi projesidir. Yüksek performanslı bir XGBoost kredi riski modeli eğitilmiş ve SHAP kütüphanesi kullanılarak modelin kararlarının hem genel hem de bireysel bazda nasıl alındığı şeffaf bir şekilde açıklanmıştır.

## Projenin Amacı
Temel amaç, sadece riskli müşterileri tahmin etmek değil, aynı zamanda bir müşterinin başvurusunun neden reddedildiğini veya onaylandığını somut faktörlere dayanarak açıklayabilen bir sistem kurmaktır.

## Kullanılan Teknolojiler
- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- SHAP
- Matplotlib, Seaborn

## Veri Seti
Bu projede Kaggle'ın "Home Credit Default Risk" veri seti kullanılmıştır. Veri setinin büyüklüğü nedeniyle dosyalar bu repoya dahil edilmemiştir. Veri setine ulaşmak için: [Buraya Kaggle Veri Seti Linkini Ekle]

## Bulgular
- Model, %75 ROC AUC skoru ile riskli ve risksiz müşterileri ayırt etmede başarılı olmuştur.
- SHAP analizleri, modelin karar verirken en çok `EXT_SOURCE_2`, `EXT_SOURCE_3` gibi dış kredi notlarına ve müşterinin yaşına (`DAYS_BIRTH`) güvendiğini göstermiştir.
- Bireysel müşteri analizleri (force plot) ile her bir müşterinin kredi kararını etkileyen faktörler başarıyla görselleştirilmiştir.
