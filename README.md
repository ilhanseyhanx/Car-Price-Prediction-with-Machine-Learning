# Car Price Prediction with Machine Learning

Bu proje, makine öğrenmesi algoritmalarını kullanarak araç fiyatlarını tahmin etmeyi amaçlayan bir veri bilimi projesidir. Proje, araç özelliklerini analiz ederek MSRP (Manufacturer's Suggested Retail Price) değerlerini tahmin eder.

## 📊 Proje Hakkında

Bu projede araç veri seti üzerinde kapsamlı bir veri analizi ve makine öğrenmesi modeli geliştirilmiştir. Linear Regression ve Random Forest algoritmaları kullanılarak araç fiyat tahminleri yapılmıştır.

## 🚀 Özellikler

- **Veri Temizleme**: Eksik değerlerin doldurulması ve aykırı değerlerin işlenmesi
- **Veri Ön İşleme**: Kategorik değişkenlerin dönüştürülmesi (One-Hot Encoding)
- **Özellik Mühendisliği**: Araç markalarının gruplandırılması ve boyut kategorilerinin sayısal dönüşümü
- **Model Geliştirme**: Linear Regression ve Random Forest algoritmalarının karşılaştırılması
- **Hiperparametre Optimizasyonu**: Grid Search ile en iyi parametrelerin bulunması
- **Performans Değerlendirmesi**: MSE, MAE ve R² metrikleri ile model başarısının ölçülmesi

## 📋 Veri Seti Özellikleri

Veri seti aşağıdaki özellikler üzerinde çalışır:
- **Make**: Araç markası
- **Engine HP**: Motor gücü
- **Engine Cylinders**: Silindir sayısı
- **Engine Fuel Type**: Yakıt tipi
- **Transmission Type**: Şanzıman tipi
- **Driven_Wheels**: Çekiş sistemi
- **Number of Doors**: Kapı sayısı
- **Vehicle Size**: Araç boyutu
- **Vehicle Style**: Araç stili
- **MSRP**: Hedef değişken (Fiyat)

## 🛠️ Kullanılan Teknolojiler

- **Python**: Ana programlama dili
- **Pandas**: Veri manipülasyonu ve analizi
- **NumPy**: Sayısal hesaplamalar
- **Scikit-learn**: Makine öğrenmesi algoritmaları
- **Matplotlib & Seaborn**: Veri görselleştirme

## 📈 Model Performansı

### Random Forest Modeli (En İyi Performans)
- **MSE**: 0.0127
- **MAE**: 0.0762
- **R² Score**: 0.9893

### Gerçek Değerler Üzerinde Performans
- **Gerçek MSE**: 84,015,138
- **Gerçek MAE**: 3,319.9
- **Gerçek R²**: 0.9588


## 📊 Veri Ön İşleme Adımları

1. **Eksik Değer İşleme**:
   - Engine HP: Ortalama ile dolduruldu
   - Engine Cylinders: Ortalama ile dolduruldu
   - Number of Doors: Mod ile dolduruldu
   - Market Category: "Unknown" ile dolduruldu

2. **Kategorik Değişken Dönüşümü**:
   - Make: En popüler 15 marka tutuldu, diğerleri "Other" olarak gruplandı
   - One-Hot Encoding ile tüm kategorik değişkenler sayısal hale getirildi

3. **Hedef Değişken Dönüşümü**:
   - MSRP değerlerine log1p dönüşümü uygulandı
   - Bu dönüşüm modelin performansını artırdı

## 🎯 Sonuçlar

Random Forest algoritması, Linear Regression'a göre çok daha iyi performans gösterdi. %95.88 R² skoru ile modelin araç fiyatlarını oldukça başarılı bir şekilde tahmin edebildiği görülmüştür.

## 👨‍💻 Geliştirici

**İlhan Seyhan**
- LinkedIn: [https://www.linkedin.com/in/ilhanseyhan/](https://www.linkedin.com/in/ilhanseyhan/)

---

⭐ Bu projeyi beğendiyseniz, lütfen yıldız vermeyi unutmayın!
