<!-- Custom Banner -->

<h1 align="center">🎬 <span style="color:#ffcc00;">Film Öneri Sistemi</span> </h1>

<p align="center">
  <i>📊 IMDB Kullanıcı Puanlarını Kullanarak Korelasyon Tabanlı Öneri Modeli</i>
</p>

<p align="center">
  <b>🐍 Python • 📚 Pandas • 🔢 NumPy • 🤖 Recommender Systems</b>
</p>

---

## ✨ <span style="color:#ff8800;">Genel Bakış</span>

Bu proje, kullanıcıların filmlere verdiği puanları analiz ederek **benzer filmleri otomatik olarak öneren** bir sistem oluşturur.  
Model, tamamen **korelasyon tabanlı işbirlikçi filtreleme** yöntemi ile çalışır.

Bu çalışma özellikle aşağıdaki konular için oldukça öğreticidir:

- ✔ Öneri sistemlerine başlangıç  
- ✔ İşbirlikçi filtreleme mantığı  
- ✔ Veri manipülasyonu, pivot tablo ve korelasyon hesaplama  
- ✔ Pandas ile veri işleme pratikleri  

---

## 🎯 <span style="color:#00b7ff;">Projenin Amacı</span>

Bu sistem:

- 🎥 Kullanıcıların benzer puanlama davranışlarına göre **filmler arasındaki benzerlikleri belirler**,  
- ⭐ Belirli bir filmi sevenlerin sevebileceği filmleri tahmin eder,  
- 🧮 Veri bilimi sürecinin temel adımlarını (ETL + analiz + modelleme) pratik olarak gösterir.  

---

## 🧠 <span style="color:#9b59b6;">Model: Item-Based Collaborative Filtering</span>

Bu projede **Filme Dayalı İşbirlikçi Filtreleme** yöntemi uygulanmıştır.

> 🧩 *Aynı kullanıcılar iki filme benzer puanlar veriyorsa, bu iki film birbirine benzerdir.*

Bu benzerlik ölçümü için:

- **Pearson Korelasyon Katsayısı** kullanılır  
- Kullanıcı–film matrisi **pivot tablo** ile oluşturulur  
- Seçilen film ile diğerleri arasındaki korelasyon hesaplanır  

Bu yöntem, içerik bilgisine ihtiyaç duymadığı için **sadece kullanıcı puanlarıyla** güçlü sonuç verir.

---

## 📁 <span style="color:#f54291;">Veri Setleri</span>

| Dosya | Açıklama |
|------|----------|
| `users.data` | Kullanıcı–film puanları (user_id, item_id, rating, timestamp) |
| `movie_id_titles.csv` | item_id ve film adı eşleştirmeleri |

Bu iki veri seti, `item_id` üzerinden birleştirilerek analiz yapılır.

---

## 🧩 <span style="color:#9961ab;">Geliştirme Fikirleri</span>

Bu projeyi daha kapsamlı bir öneri sistemine dönüştürmek için aşağıdaki geliştirme fikirlerini uygulayabilirsin:

➕ Tür (genre) tabanlı öneri ekleme

🤝 User-Based Collaborative Filtering modeli ekleme

📈 Cosine Similarity, Jaccard gibi alternatif benzerlik ölçümleri deneme

🌐 Streamlit veya Flask ile web arayüzü hazırlama

⭐ IMDB Weighted Rating (WR) formülü ile daha doğru sıralamalar

🧠 TF-IDF + Cosine Similarity ile içerik tabanlı öneri ekleme

🔄 Hibrit öneri sistemi oluşturma (CF + Content-Based)

📊 Sonuçları grafiklerle görselleştirme

🗂️ Daha büyük veri setleri (MovieLens 20M gibi) ile performansı değerlendirme

## 🛠️ <span style="color:#1abc9c;">Kullanılan Teknolojiler</span>

```text
🐍 Python 3
📚 Pandas
🔢 NumPy
📓 Jupyter Notebook
