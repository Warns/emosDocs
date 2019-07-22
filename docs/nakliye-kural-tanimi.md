---
id: nakliye-kural-tanimi
title: Nakliye Kural Tanımı
---

Kargo kampanyalarında kullanılan kuralların belirtildiği ekrandır. Bu ekranı kullanarak özelleştirilmiş kargo kampanyaları tanımlanabilir. 

Bu ekranda oluşturulan kural "Kargo Kampanyası" olarak tanımlanır. Gelişmiş kampanya tanımı hakkında ayrıntılı bilgi almak için [Tıklayın](kampanya-tanimi.md)

Yeni bir nakliye kuralı tanımlamak için için Nakliye Kural Tanımı sayfası açıldığında **Ekle** butonuna tıklanılır. 

Bu ekranda bulunan alanlarla ilgili detaylar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Seçim Tipi* (Zorunlu Alan)|**Dahil Seçimler**<br>Bu bölümden kurgulanacak olan nakliye kural tanımının geçerli olacağı seçimler yapılır.<br>Kullanılabilir seçimler; **Tüm Mümkün Ürünler İçin, Ürün, Marka, Kategori, Tedarikçi, Ürün Sınıfı**<br><br>**Hariç (Kapsam Dışı) Seçimler**<br>Bu bölümden kurgulanacak olan nakliye kural tanımının geçerli olmayacağı seçimler yapılır.<br>Kullanılabilir seçimler; **Ürün, Marka, Kategori, Tedarikçi, Ürün Sınıfı**<br><br>**Örnek:** Dahil seçimlerden Bayan Giyim kategorisi seçildi, hariç seçimlerden ise Bayan Giyim kategorsinin altında bulunan Aksesuar kategorisi seçildi. Bu kural, aksesuar kategorisi hariç Bayan Giyim kategorisinin diğer tüm alt kategorilerinde geçerli olur.|
|Kural Seçim/Kural Seçim 2|Seçim Tipi bölümünden seçim yaptıktan sonra ilgili seçime göre kullanılır. Seçim Tipi bölümünde yapılan seçime göre bu alan değişir.<br><br>**Örnek:** Seçim tipi olarak Ürün seçildiğinde bu alandan sadece ürün seçilebilir.|
|Min. Miktar|Nakliye kural tanımının geçerli olması için sipariş içerisindeki minimum miktar.|
|Min. Tutar|Nakliye kural tanımının geçerli olması için sipariş içerisindeki minimum tutar.|
|İndirim Oranı (%)|Minimum miktar veya minimum tutar sağlandığı durumda kargo ücretine uygulanacak olan indirim oranı.|
|Tutar|Minimum miktar veya minimum tutar sağlandığı durumda kargo ücretinin tutar olarak belirlendiği alan.<br><br>**Örnek:** Bu alana 1 girildiğinde kargo ücreti 1TL olacaktır.|
|Nakliye Adı|Nakliye kural tanımının geçerli olacağı kargo firmasının seçildiği alandır.<br>Nakliye Tanımı hakkında ayrıntılı bilgi almak için [Tıklayın](nakliye-tanimi.md)|
|Fiyat Tipi|Nakliye kural tanımın geçerli olacağı fiyat tipinin seçildiği alandır. Bu alan çoklu seçim olarak çalışmakta olup birden fazla fiyat tipi seçilebilecektir.<br>Fiyat Tipi hakkında ayrıntılı bilgi almak için [Tıklayın](fiyat-tipi-tanimi.md)|
|Üye Kategori|Nakliye kural tanımının varsa, geçerli olacağı üye kategorsinin belirlendiği alandır.|
|Not|e-MOS panel kullanıcısı tarafından kullanılabilir not alanıdır. Bu alana yazılan yazı önyüzde görünmeyecektir.|
|Önyüz, kargo kampanya uyarı metni|Önyüzde nakliye kural tanımı uygulandığı durumda gösterilecek açıklama yazısına karşılık gelir.|
|Ürün Detay kargo kampanya uyarı metni|Önyüzde nakliye kural tanımıyla ilgili ürün detayda gösterilecek açıklama yazısına karşılık gelir.|
|Başlangıç/Bitiş Tarihi|Nakliye kural tanımının başlangıç ve bitiş tarihinin belirlendiği alandır.|
|Platform|Nakliye kural tanımının çalışacağı platforma karşılık gelir.  Masaüstü, mobil taryıcı, mobil uygulama (API). Bu alan çoklu seçim olarak çalışmakta olup birden fazla platform seçilebilecektir.|
|Dil|Sitenin öndeğer dili otomatik olarak bu alanda seçili olarak gelecektir.<br>Çoklu Dil yapısıyla ilgili ayrıntılı bilgi almak için [Tıklayın](coklu-dil.md)|
|Sıra|Nakliye kural tanımının sırasını belirleyen alandır.|
|Para Birimi|Nakliye kural tanımının geçerli olacağı para birimine karşılık gelir.|
|Onay|Nakliye kural tanımının durumunu belirleyen alandır. Aktif olması için bu kutucuğun seçili olması gerekir.|

> ❗ _**Min Miktar** veya **Min Tutar** alanlarının sadece birisi doldurulması gerekir. Aynı anda iki alanda da değer girilmemelidir._

> ❗ _**İndirim Oranı** veya **Tutar** alanlarının sadece birisi doldurulması gerekir. Aynı anda iki alana da değer girilmemelidir._

Nakliye kural tanımı işlemi tamamlandıktan sonra **Kaydet**'e tıklayarak kural tanımlama işlemi tamamlanır.
