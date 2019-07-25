---
id: sayfa-yerlesim-duzenleme
title: Sayfa Yerleşim Düzenleme
---

Sayfa Yerleşim Düzenleme, sitedeki sabit içerikli ya da dinamik, bütün sayfaların yerleşim düzeni anlamında değiştirildiği kısımdır. SYD’de sağ üstteki listeden ***SS*** , değişiklik yapmak istediğimiz sayfayı seçerek, o sayfada işlem yapabiliriz. Sayfa seçimini yaptıktan sonra karşımıza, o sayfanın kolon ve satırlardan oluşan sayfa düzeni gelmektedir. Burada iki farklı yapı bulunmaktadır; 

## Modül
Sistemin sahip olduğu hazır yapılardır. Bu yapılara sadece tasarımsal anlamda müdahale edilebilmektedir. (**Örnek:** Arama Kutusu, Chat Kutusu, vb.) 

<br>
## Banner
Kullanıcı tarafından oluşturulan ve sayfaya HTML, CSS, Javascript gibi eklemeler yapmayı sağlayan yapılardır.

Bu yapılar, sağ taraftan sol tarafa sürüklenip bırakılarak, seçilen sayfanın içine eklenebilmektedir. 

<br>

### Banner Yapısı
Listedeki bannerler üzerinde bulunan **Büyüteç** ikonuna tıklayarak ilgili bannerin detay sayfası görüntülenebilmektedir. İçeriğin üst kısmında, Tarih (bannerın oluşturulma tarihi), Banner Yeri (bannera verilen ad), Yerleşim Yeri (bannerın kullanılacağı sayfa), Açıklama gibi, bannerla ilgili bilgiler yer almaktadır.

>❗️ _Farklı özellikleri olan bazı bannerlere tıklandığında sağ tarafta **Özellikler** sütunu altında ilgili bannerin diğeer özellikleri görünür. **Örnek:** Ürün Liste banner yapısında her sayfa kaç adet ürün gösterilsin._

Alt kısımda ise, o bannera ait içeriklerin bulunduğu kısım yer almatadır. Buradaki **Ekle** buttonu ile yeni bir içerik eklenebilir ya da **Sil** buttonu ile önceden oluşturulmuş bir içerik silinebilir. Eğer herhangi bir içeriği silmeden sadece görünmesine engel olmak istiyorsak, sadece **Onay Kaldır** buttonu ile veya içeriğin sol tarafındaki flag (til işareti) ikonuna tıklayarak onayını kaldırmamız yeterli olacaktır.

Bannera yeni bir içerik eklemek istediğimizde karşımıza aşağıdaki gibi alanlar çıkmaktadır;

|Alan Adı|Açıklama|
|--|--|
|Tarih|Oluşturulma tarihinin gösterildiği alandır. İstenirse değişiklik yapılabilir.|
|Banner Yeri|İçeriğin ekleneceği bannerın belirleneceği alandır.|
|Yerleşim Yeri|Sitede ekleneceği yerin seçildiği alandır.|
|Açıklama|Banner ile ilgili açıklamaların girileceği alandır.|
|Onay|Bannerın sitede aktif olması için onay kutusunun işaretli olması gerekir.|
|Ent. Kodu||

>❗️ _Bannerlerin içerisindeki alanlar özelleştirilebilir olup, proje bazlı değişmektedirler._

<br>
### Banner Türleri

#### 1. Image

**"Banner Türü"** kısmında **Image** seçeneği işaretlenmişse, aşağıdaki kısımlar yer alır.

- **Banner Target Link :** Image'a tıklandığında gidilecek url ve bu işlemin aynı sayfada mı yoksa farklı sayfada mı yapılacağı bilgisi,
- **Banner Align :** Bannerın hizalanma bilgisi,
- **Banner Kaynağı :** Banner olarak eklenmek istenen image dosyasının seçimi,
- **Banner Etiketi :** Image banner ile ilgili kısa bilgi

#### 2. Video

**Banner Türü** kısmında **Video** seçeneği işaretlenmişse, aşağıdaki kısımlar yer alır.

**Banner Align:** Bannerın hizalanma bilgisi
**Banner Kaynağı:** Banner olarak eklenmek istenen video dosyasının seçimi
**Video URL:** Eklenecek olan video online bir video ise, ilgili videonun linkinin girildiği alandır.

#### 3. URL

**Banner Türü** kısmında **URL** seçeneği işaretlenmişse, aşağıdaki kısımlar yer alır.

**Banner Target Link:** linke tıklandığında gidilecek url ve bu işlemin aynı sayfada mı yoksa farklı sayfada mı yapılacağı bilgisi
**Banner Align:** Bannerın hizalanma bilgisi
**Banner Yazısı:** 

#### 4. HTML

**Banner Türü** kısmında **HTML** seçeneği işaretlenmişse, aşağıda HTML içeriklerin girilebileceği bir editör kısmı yer almaktadır.

#### 5. Ürün

**Banner Türü** kısmında **Product** seçeneği işaretlenmişse, ilgili bannerde ürün gösterimi sağlanabilecektir.

>❗️ _Bahsi geçen temel banner türlerine ek olarak proje bazlı özelleştirilen ve geliştirilmiş farklı banner türleri de frontend ekibi tarafından yapılabilmektedir._




