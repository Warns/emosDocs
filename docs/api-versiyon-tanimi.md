---
id: api-versiyon-tanimi
title: API Versiyon Tanımı
---

Sayfanın en üst kısmında yer alan filtreler ile **Versiyon, İşletim Sistemi, Versiyon Durumu** kriterleri üzerinden **Ara** butonuna tıklayarak arama işlemi gerçekleştirebilirsiniz.

Yeni bir versiyon kaydı eklemek için **Ekle** butonu tıklanır. Var olan bir kayıt üzerinde değişiklik yapmak için de ilgili kaydın üzerinde tıklayarak yeni bir sayfa açılır.

Açılan sayfada bulunan alanlarla ilgili detaylar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Versiyon|Versiyon bilgisinin belirlendiği alandır.<br>**Örnek:** 1.8.1|
|İşletim Sistemi|Versiyonun kullılacağı işletim sisteminin seçildiği alandır.|
|Versiyon Durum|Versiyon durumunun seçildiği alandır.<br>**Geçerli:** Güncel ve geçerli olan versiyon anlamına gelir.<br>**Güncellemeye Zorla:** mobil uygulama tarafından güncellemeye zorlayacak seçim anlamına gelir.|
|Kaydı Ekleyen|Versiyon tanımı kaydını ekleyen admin panel kullanıcısının görüntülendiği alandır.|
|Kayıt Tarihi|Versiyon tanım kaydının yapıldığı tarihe karşılık gelir.|
|Son Güncelleyen|Son hangi admin paneli kullanıcısı tarafından güncellendiğine karşılık gelir.|
|Son Güncelleme Tarihi|Son güncelleme tarihine karşılık gelir.|

>❗ _API üzerinden ilgili metoda versiyon bilgisi göndererek, versiyon farkı varsa ona göre uygulamayı güncellemeye zorlayacak şekilde ilgili fonksiyonu tetikler._