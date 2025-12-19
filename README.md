🤖 AI-Powered Resume Screening & Job Category Classification


📌 Proje Özeti

Bu proje, özgeçmiş (CV) metinlerini otomatik olarak analiz ederek adayları en uygun iş kategorisine atayan yapay zeka destekli bir Resume Screening sistemidir.

Sistem;

Metin ön işleme (NLP)

TF-IDF tabanlı özellik çıkarımı

Çoklu makine öğrenmesi modelleri

Web tabanlı Flask arayüzü

kullanarak uçtan uca bir AI uygulaması olarak geliştirilmiştir.

🎯 Projenin Amacı

İnsan kaynaklarında manuel CV inceleme süresini azaltmak

CV’leri objektif ve tutarlı şekilde sınıflandırmak

Gerçek dünya NLP problemlerini makine öğrenmesi ile çözmek

🧠 Kullanılan Yöntemler
🔹 1. Veri Ön İşleme (Text Cleaning)

CV metinleri aşağıdaki adımlarla temizlenmiştir:

URL’lerin kaldırılması

Hashtag ve mention temizleme

Noktalama işaretleri ve özel karakterlerin silinmesi

Gereksiz boşlukların azaltılması

📌 Amaç: Gürültüyü azaltarak model performansını artırmak

🔹 2. Etiketleme (Label Encoding)

İş kategorileri (ör. Data Scientist, Java Developer, Advocate)
sayısal etiketlere dönüştürülmüştür.

📌 Makine öğrenmesi modellerinin metin yerine sayısal veri ile çalışabilmesi için gereklidir.

🔹 3. TF-IDF (Text Vectorization)

CV metinleri TF-IDF yöntemi ile sayısal vektörlere dönüştürülmüştür.

TF-IDF Avantajları:

Önemli kelimeleri vurgular

Çok sık geçen anlamsız kelimelerin etkisini azaltır

Metinleri makine öğrenmesine uygun hale getirir

🤖 Kullanılan Modeller
🔸 K-Nearest Neighbors (KNN)

Benzer CV’leri mesafeye göre sınıflandırır

One-vs-Rest yaklaşımı ile çok sınıflı problem çözülür

🔸 Naive Bayes (MultinomialNB)

Metin sınıflandırma problemleri için hızlı ve etkili

TF-IDF ile yüksek performans sağlar

🔸 Support Vector Classifier (SVC)

Yüksek boyutlu metin verilerinde güçlü performans

Projede ana tahmin modeli olarak kullanılmıştır

📊 Model Değerlendirme

Her model için:

Accuracy

Confusion Matrix

Classification Report (Precision, Recall, F1-score)

hesaplanmıştır.

Modeller karşılaştırılarak en stabil ve başarılı yapı seçilmiştir.

🌐 Web Uygulaması (Flask + Ngrok)

Proje, Flask kullanılarak web arayüzüne dönüştürülmüştür.

Kullanıcı Akışı:

Kullanıcı CV metnini girer

Metin temizlenir

TF-IDF ile vektörleştirilir

Modeller tahmin yapar

Sonuçlar ekranda gösterilir

📌 Ngrok ile uygulama dış dünyaya açılmıştır.

🖥️ Arayüz Özellikleri

Modern ve responsive tasarım (Tailwind CSS)

Aynı CV için birden fazla model sonucu

Model doğruluk oranlarının gösterimi

Kullanıcı dostu ve sade UI

🛠️ Kullanılan Teknolojiler

Python

Pandas, NumPy

Scikit-learn

TF-IDF

Flask

Ngrok

📂 Proje Yapısı

Resume-Screening-AI/
│
├── data/
│   └── UpdatedResumeDataSet.csv
│
├── models/
│   ├── tfidf.pkl
│   ├── svc_model.pkl
│   ├── nb_model.pkl
│   ├── knn_model.pkl
│   └── encoder.pkl
│
├── app.py
├── README.md
└── static/
    └── banner.png

🚀 Neden Bu Proje?

Bu proje;

NLP & Machine Learning bilgisini

Gerçek dünya insan kaynakları problemlerine uygulamayı

Model eğitimi + deployment sürecini

Full-stack AI yaklaşımını

tek bir projede uygulamaktadır.


<img width="978" height="499" alt="resim" src="https://github.com/user-attachments/assets/a1ffc2df-bcfd-4845-8701-ba4b6b975d04" />




