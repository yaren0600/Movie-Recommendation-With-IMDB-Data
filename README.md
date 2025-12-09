# 🎬 **Film Öneri Sistemi**

<p align="center">
  <img src="https://img.icons8.com/external-flaticons-lineal-color-flat-icons/512/external-cinema-movie-theater-flaticons-lineal-color-flat-icons.png" width="140" />
</p>

<p align="center">
  <strong>📊 IMDB Kullanıcı Puanlarını Kullanarak Korelasyon Tabanlı Film Öneri Modeli</strong><br>
  <sub>Python • Pandas • NumPy • Recommender Systems</sub>
</p>

---

## ✨ Genel Bakış

Bu proje, kullanıcıların filmlere verdiği puanları analiz ederek **benzer filmleri otomatik olarak öneren** bir sistem geliştirmektedir.  
Model tamamen **korelasyon tabanlı işbirlikçi filtreleme (Item-Based CF)** prensibi ile çalışır.

Bu proje özellikle:

- ✔ Öneri sistemlerine giriş yapmak isteyenler  
- ✔ Veri analizi ve Pandas pratiği geliştirmek isteyenler  
- ✔ Basit ama etkili bir model oluşturmak isteyenler  

için ideal bir örnektir.

---

## 🎯 Projenin Amacı

Bu sistem:

- 🎥 Kullanıcıların benzer puanlama davranışlarına göre **filmler arasındaki benzerlikleri hesaplar**,  
- ⭐ Popüler bir filmi seven kullanıcılar için **benzer filmleri önerir**,  
- 🧮 Veri manipülasyonu, pivot tablo ve korelasyon hesaplama adımlarını gösterir.  

---

## 🧠 Kullanılan Yöntem: *Item-Based Collaborative Filtering*

Bu projede **Filme Dayalı İşbirlikçi Filtreleme** uygulanır.

> 🧩 *Aynı kullanıcılar iki filme benzer puanlar veriyorsa, bu iki film benzerdir.*

Kullanılan teknikler:

- 📌 Pivot tablo ile kullanıcı–film matrisi oluşturma  
- 📌 Pearson korelasyon katsayısı ile benzerlik ölçme  
- 📌 Eksik değerleri filtreleme  
- 📌 Oy sayısına göre güvenilirlik kontrolü  

---

## 📁 Veri Setleri

| Dosya | Açıklama |
|-------|----------|
| `users.data` | user_id, item_id, rating, timestamp |
| `movie_id_titles.csv` | Film ID ve film isimleri |

İki tablo, `item_id` üzerinden birleştirilerek analiz edilir.

---

## 🛠️ Kullanılan Teknolojiler

- 🐍 Python 3  
- 📚 Pandas  
- 🔢 NumPy  
- 📓 Jupyter Notebook  

---

## 🧩 Kod Akışı

1. Veri dosyalarını okuma  
2. `merge()` ile birlikleştirme  
3. Pivot tablo oluşturma  
4. Korelasyon hesaplama  
5. 100+ oy alan filmleri filtreleme  
6. En benzer filmlerin öneri listesi olarak sunulması  

---

## 🚀 Geliştirme Fikirleri

Aşağıdaki geliştirmelerle sistemi çok daha gelişmiş hâle getirebilirsiniz:

- ➕ Tür (genre) tabanlı öneri ekleme  
- 🤝 User-Based Collaborative Filtering oluşturma  
- 📈 Cosine Similarity veya Jaccard Index ile benzerlik karşılaştırma  
- 🌐 Streamlit / Flask ile web uygulaması geliştirme  
- ⭐ IMDB Weighted Rating sistemi entegre etme  
- 🧠 TF-IDF + Cosine Similarity ile içerik tabanlı öneri  
- 🔄 Hibrit öneri sistemi (Collaborative + Content-Based)  
- 📊 Sonuçları grafiklerle görselleştirme  
- 🗂️ Daha büyük veri setlerinde performans testi (MovieLens 20M gibi)  

---

## 🎉 Sonuç

Bu proje, film öneri sistemlerinin temel mantığını anlamak için harika bir başlangıçtır.  
Korelasyon tabanlı yöntem basit ama etkili sonuçlar verir ve kolayca genişletilebilir.

Daha gelişmiş sistemler için yukarıdaki fikirleri ekleyerek projeyi büyütebilirsiniz! 🚀

---

