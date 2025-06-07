# Müşteri Segmentasyonu - Makine Öğrenmesi Projesi

Bu projede, alışveriş merkezi müşterilerinin demografik bilgileri (yaş, cinsiyet, yıllık gelir, harcama skoru) kullanılarak benzer müşterilerin gruplanması amaçlanmıştır. Segmentasyon işlemi, K-Means algoritması kullanılarak gerçekleştirilmiştir.

## Veri Seti

Kaynak: https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial  
Kullanılan dosya: Mall_Customers.csv

## Proje Aşamaları

1. Veri Analizi ve Görselleştirme (EDA - Exploratory Data Analysis)  
   Yaş, cinsiyet, harcama skoru ve yıllık gelir gibi değişkenler incelenmiştir.  
   Harcama skorunun yaş ve cinsiyet ile olan ilişkisi görselleştirilmiştir.

2. Segmentasyon (Clustering)  
   K-Means algoritması kullanılarak müşteriler gruplandırılmıştır.  
   En uygun küme sayısı Elbow Yöntemi ve Silhouette Skoru ile belirlenmiştir.  
   3D görselleştirme ile segment yapısı analiz edilmiştir.

3. Değerlendirme  
   Her segmentin ortalama yaş, gelir ve harcama değerleri analiz edilmiştir.  
   İş hedeflerine göre en değerli müşteri grubu belirlenmiştir.

## Kullanılan Kütüphaneler

pandas  
numpy  
seaborn  
matplotlib  
sklearn
plotly  

## Proje Yapısı

04_Customer-Segmentation/  
├── data/  
│   └── Mall_Customers.csv  
├── notebook/  
│   └── mall_customers.ipynb  
├── images/  
│   ├── yas_gruplari_harcama_skora.png  
│   ├── cinsiyete_gore_ortalama_harcama.png  
│   └── yas_harcama_cinsiyete_gore.png  
│   └── 3d_kume_grafigi.html
│   └── sayisal_degiskenler.png
│   └── elbow_silhouette_skoru.png
├── README.md  
├── requirements.txt  
└── .gitignore

## Notlar

Bu proje, pazarlama stratejilerine destek olacak şekilde müşteri segmentasyonu yapma amacı taşımaktadır.  
Gerçek veri ile yapılan bu uygulama, müşteri analizinde makine öğrenmesinin nasıl kullanılabileceğini göstermektedir.