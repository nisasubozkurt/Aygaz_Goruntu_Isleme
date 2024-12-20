# 🎯 Aygaz Görüntü İşleme Bootcamp

## Proje Adı - Aygaz Görüntü İşleme Bootcamp

## Kaggle :https://www.kaggle.com/code/subozkurt/aygaz-goruntu-isleme-bootcamp

## 1. Proje Hakkında
Bu proje, bir Convolutional Neural Network (CNN) modeli kullanarak belirli hayvan sınıflarının doğruluğunu test etmeyi ve farklı veri manipülasyonları altında model performansını değerlendirmeyi amaçlamaktadır. CNN modeliyle, "collie", "dolphin", "elephant" gibi 10 farklı hayvan türü arasında sınıflandırma yapılmış ve çeşitli manipülasyonlar üzerinden model performansı analiz edilmiştir.

## 📊 Kullanılan Teknolojiler ve Kütüphaneler
- **Python 3.x**: Projenin temel dilidir.
- **Keras ve TensorFlow**: CNN modeli oluşturulup eğitimi için kullanıldı.
- **OpenCV**: Resim manipülasyonu ve işleme adımları için.
- **Sklearn**: Veri setini bölmek ve analizler yapmak için.
- **Matplotlib ve Seaborn**: Veri görsel hale getirmek için.

## 🧑‍💻 2. Veri Setinin Hazırlanması
### 2.1 Veri Setinin Filtrelenmesi
Bu adımda veri seti filtrelenerek 10 farklı hayvan sınıfı için dengeli bir şekilde 650 görüntü seçilmiştir.

### 2.3 Veriyi Eğitim ve Test Seti Olarak Ayırma
Veriler %70 eğitim ve %30 test oranında rastgele ayrılmış, ayrıca veri artırma teknikleri uygulanmıştır.

## Veri Setinin Ayrılması ve Veri Artırımı
- **Resim Yeniden Boyutlandırma**: 224x224 boyutuna.
- **Normalizasyon**: Tüm pikseller [0,1] aralığına getirilmiştir.
- **Veri Artırma**: Döndürme, bulanıklaştırma, gürültü ekleme gibi tekniklerle veri çeşitliliği artırılmıştır.

## 🧠 CNN Modelinin Oluşturulması ve Eğitilmesi
CNN modelinin yapısı şu katmanlardan oluşmaktadır:
- **Konvolüyon Katmanları**: Özellik çıkarma.
- **Havuzlama (Pooling)**: Boyut azaltma.
- **Dropout**: Aşırı uyumun önlenmesi.
- **Fully Connected Katmanlar**: Sınıflandırma.

## 🔧 Modeli Derleme
Kullanılan kayıp fonksiyonu ve optimizer:
- Kayıp Fonksiyonu: `categorical_crossentropy`
- Optimizer: Adam.

## 🔬 Model Performansını Görselleştirme
Eğitim ve test sırasında elde edilen kayıp ve doğruluk değerleri grafiklerle görünür hale getirilmiştir.
![image](https://github.com/user-attachments/assets/d92c7e88-9299-4e86-866f-f7462c56205f)

## 🎨 Manipüle Edilmiş Test Seti ile Modeli Test Etme
Manipüle edilmiş resimlere aşağıdaki teknikler uygulanarak model performansı test edilmiştir:
- Işık koşullarının değiştirilmesi.
- Renk manipülasyonları.
 ![image](https://github.com/user-attachments/assets/890fb9a6-016a-49f6-b059-b117bac656d7)
 ![image](https://github.com/user-attachments/assets/67740993-8350-4284-9c54-af2fef7c1aa0)



## 💖 Renk Sabitliği Algoritması Uygulama ve Test Etme
Manipüle edilmiş resimlere renk sabitliği algoritmaları uygulanarak test edilmiştir. Bu adım, model performansını arttırmaya yönelik bir iyileştirme sağlamıştır.
![image](https://github.com/user-attachments/assets/3c0d6aa7-3933-4f63-bc67-299632bc3b37)
![image](https://github.com/user-attachments/assets/444c0755-ada9-401a-af10-89e22ba6c1fc)



## 📉 Model Test Edilmesi ve Analizi
Test sonuçlarından elde edilen başarı oranları analiz edilmiş ve çözüm önerileri tartışmıştır.



## ⚡ Sonuçlar
Manipüle edilmiş verilerde performans düşümü yaşamış, renk sabitliği algoritması kısmen performans artışı sağlamıştır. Ancak, bu artış her hayvan sınıfı için aynı düzeyde olmamıştır. Gelecek çalışmalar için daha karmaşık renk sabitleme teknikleri ve çoklu manipülasyon testleri önerilmektedir.
![image](https://github.com/user-attachments/assets/306dad36-d5a1-4f72-9c2d-1feafab24aa6)



