---
id: veri-aktarimi
title: Veri Aktarımı
---

Sisteminiz için kullanılan dış kaynakları (NEBIM, LOGO, ETA, OBASE, NETSIS, API, ... ) yada Excel entegrasyonunu çalıştırarak ürün, stok, fiyat, İndirim/Hediye Kuponu, Özellik Setleri, Servis/bayi aktarımlarını bu menü üzerinden yapılabilmektedir,t.

## 1. İşlem Listesi
Veri Aktarımı sayfasına geldiğiniz zaman ilk önce üst kısımdan çalıştırılacak olan dış kaynak entegrasyonu veya excel seçilir. Entegrasyon tipi seçildikten sonra ekrana işlem listesi gelir. İşlem listesiyle ilgili detaylar aşağıdadır;

|Alan Adı|Açıklama|
|--|--|
|Kaynaktan Veri Çek|İlgili entegrasyondan Ürün, stok, fiyat, İndirim/Hediye Kuponu, Özellik Setleri, Servis/bayi lerin e-MOS ara tablosuna çekme işlemi için bu menüyü tıklamalısınız.<br><br>❗ _Eğer ilgili ara tablolar da veriler gözükmüyorsa ent. kontrol edilmelidir._ |
|Thumb oluştur|e-MOS ' a aktarılacak görsellere ait thumb ları bu menü üzerinden oluşturabilirsiniz. Thumb oluşturma işlemi için görsellerin bulunduğu FTP yolunu sayfada ki ilgili alana giriniz <br><br>❗ _Thumbların Üstüne Yaz checkbox u işaretlenirse vermiş olduğunuz klasör içersindeki tüm görsellerin thumbları tekrar oluşur. Aksi durumda sadece thumb ı olmayan görsellerin thumbları oluşacaktır._ |
|Görsel Sıkıştır|tinypng.com, compressor.io gibi 3rd party görsel sıkıştırma toollarına entegre olarak görsel sıkıştırma işlemi yapılabilmektedir. Görsel sıkıştırma yapısını kullanabilmek için ilgili 3rd party tool'un API bilgileri gerekecektir.<br><br>❗ _Belli bir limit sonrası bahsedilen 3rd party toolları ücretli olup firma tarafından görsel sayısına göre üyelik alınması gerekir._|
|Kategori Listele|Kaynaktan veri çekme işlemi sonrasında ent. ile gelen **Kategorilerin** listeleneceği ara tabloyu bu menüden görebilirsiniz.|
|Ürün Listele|Kaynaktan veri çekme işlemi sonrasında ent. ile gelen **Ürünlerin** listeleneceği ara tabloyu bu menüden görebilirsiniz.|
|Özellik Listele|Kaynaktan veri çekme işlemi sonrasında ent. ile gelen **Özelliklerin** listeleneceği ara tabloyu bu menüden görebilirsiniz.|
|Özellik Değer Listele|Kaynaktan veri çekme işlemi sonrasında ent. ile gelen **Özellik Parametrelerinin** listeleneceği ara tabloyu bu menüden görebilirsiniz.|
|Özellik Karşılık Listele|Özellik Karşılık bilgileri e-MOS içerisinde bir tabloda tutulmaktadır. Entegrasyonla ilgili olan karşılık bilgileri yönetim panelinden güncellenebilecektir.<br><br>Özellik Karşılık ile ilgili ayrtınlı bilgi için [Tıklayın](ozellik-karsilik.md)|
|Stok Liste	|Kaynaktan veri çekme işlemi sonrasında ent. ile gelen **Stokların** listeleneceği ara tabloyu bu menüden görebilirsiniz.|
|Fiyat Listele|Kaynaktan veri çekme işlemi sonrasında ent. ile gelen **Fiyatların** listeleneceği ara tabloyu bu menüden görebilirsiniz.|
|Hediye Çeki Listele|Kaynaktan veri çekme işlemi sonrasında ent. ile gelen **Hediye Çeki veya İndirim kuponlarının** listeleneceği ara tabloyu bu menüden görebilirsiniz.|
|Servis Listele|Kaynaktan veri çekme işlemi sonrasında ent. ile gelen **Servis / Bayilerin** listeleneceği ara tabloyu bu menüden görebilirsiniz.|
|Bundle Ürün Yükle|Ürünlere topluca bundle ürün bağlamak için bu bölüm kullanılabilir.<br><br>**Örnek:** Spor Ayakkabı kategorisindeki tüm ürünlerde, xyz çorap bundle olarak gösterilsin. Spor Ayakkabı kategorisindeki her hangi bir ürün detay'a bakıldığında xyz çorap bundle olarak görünecektir.<br><br>❗ _Bundle ürün gösterimi tasarıma bağlı bir süreç olup gerekli tasarım ve frontend giydirme işlemi sonrası önyüzde görünebilir hale gelir._|
|Entegrasyonu Başlat|Ara tablosu dolu olan menülerin başlıkları bu menüye tıklandığında listelenir. Ara tablo kontrolünden sonra buradan aktarmak istediklerinizi işaretleyip Entegrasyon başlat diyerek verileri e-MOS'a taşıyabilirsiniz.|


>❗  _Ara tabloya çekilen verilerin kontrolü iyi bir şekilde yapılmaldır. Entegrasyon başlat dedikten sonra ara tablolardaki tüm veriler eğer onaylılarsa direk canlı ortama yansıyacaktır._

<br>
## 2. Excel Entegrasyonu

Entegrasyonda kullanılacak olan örnek excel'i bir önceki maddede belirtilen işlem listesi bazlı ilgili sayfalardan indirebilirsiniz. 

❗ _Excel aktarımı sırasında Sheet isimlerinin, indirdiğiniz şekilde kalması gerekmektedir. Örneğin Ürün entegrasyonu yapılırken sistem "PRODUCT" sheet ini arayacaktır. Bu ismin değişmiş olması durumunda hata verecektir._

❗ _Aktarım yapacağınız ilgili sol menüde olduğunuza dikkat etmelisiniz. Kategori Listele menüsündeyken Ürün yükleme yapılmaya çalışıldığında hata ile karşılaşabilirsiniz._

❗ _Fiyat ve Seçenek aktarımlarında hata ile karşılaşmamak için Site ayarları > Entegrasyon Ayarları menüsünü kontrol etmelisiniz. Site ayarları hakkında bilgi almak için Tıklayınız._

<br>
### 2.1. Ürün Yükle 
Ürün aktarımı yapmak için Product sheetinin üzerine tıklayarak aşağıdaki alanları doldurmanız gerekmektedir.

EUR_URUN_KODU (Ürün Kodu), EUR_AD (Ürün Adı), EUR_MARKA (Marka), EUR_VERGI (Vergi), EUR_RESIMLER (Resim), EUR_OZELLIK (Özellik), EUR_KAT_KODLAR (Bağlı Kategoriler), EUR_URUN_KODU_UST (Bağlı Ürün kodu), EUR_GRUP_FL (Ürün Gurubu varmı), EUR_AD_KISA (Ürün Kısa Ad), EUR_KISAACIKLAMA (Ürün Kısa Açıklama), EUR_URUN_ONYUZKODU (Önyüz Ürün Kodu), EUR_DESI (Desi), EUR_SATISKATI (Satış Katı), EUR_IMAGEZOOM_FL (Zoom), EUR_ONAY_FL (Onay), LNG_CULTURENAME (Language), EUR_OZA_AD1 (Özel Alan 1), EUR_OZA_AD2 (Özel Alan 2), EUR_METADESCRIPTION (Meta Description), EUR_SAYFABASLIK (Sayfa Başlık), EUR_SAYFAISMI (Sayfa İsmi), EUR_KISAACIKLAMA2 (Ürün Kısa Açıklama 2), EUR_URUNTIPI (Ürün Tipi), EUR_SERVIS_FL (Servis Gerektiren Ürün), EUR_STYLE (Class), EUR_KISAKOD (Kısa Kod), EUR_GUMRUKTIPI (Gümrük Tipi), EUR_ACIKLAMA2 (Açıklama 2), EUR_YENIURUN_FL (Yeni Ürün), EUR_TEKSATILAMAZ_FL (Tek Satılmaz), EUR_MAXTAKSITSAYISI (Max. Taksit Sayısı), EUR_LISTEGOSTERILMESIN_FL (Ürün Liste Gösterilmesin), EUR_MINADET (Min Adet), EUR_MAXADET (Max Adet), EUR_AGIRLIK (Net Ağırlık), EUR_OZS_KOD (Özellik Seti), EUR_TESLIMSURESI (Teslim Süresi), EUR_KEYWORD (Anahtar Kelimeler), EUR_KEYWORD_RANK (Keyword Rank)


|Alan Adı|Açıklama|
|--|--|
|EUR_URUN_KODU|Aktarılacak ürüne ait Ürün kodu bu alana girilmelidir.|
|EUR_AD|Aktarılacak ürüne ait Ürün adı bilgisi bu alana girilmelidir.|
|EUR_MARKA|Aktarılacak ürünü bağlamak istediğiniz marka entegrasyon kodunu bu alana yazmalısınız.<br><br>❗ _Eğer Daha önce oluşturulmamış bir entegrasyon kodu yazarsanız. Buraya yazacağınız bilgi ile yeni bir marka oluşturulacaktır. Marka Tanımları hakkında bilgi almak için [Tıklayın](marka-tanimi.md)._|
|EUR_VERGI||
|EUR_RESIMLER||
|EUR_OZELLIK||
|EUR_KAT_KODU||
|EUR_KODU_UST||
|EUR_GRUP_FL||
|EUR_AD_KISA||
|EUR_KISAACIKLAMA||
|EUR_URUN_ONYUZKODU||
|EUR_DESI||
|EUR_SATISKATI||
|EUR_IMAGEZOOM|
|EUR_ONAY_FL||
|LNG_CULTURENAME||
|TEDARIKCI_KOD||
|EUR_OZEL_AD1||
|EUR_OZEL_AD2||

Bu alanları doldurup dosyayı seçtikten sonra, Ürün Listele sol menüsü üzerindeki yükle butonu ile ürünleri ara tabloya yükleyebilirsiniz.

<br>
### 2.2. Fiyat Aktarımı
Fiyat aktarımı yapmak için Price sheetinin üzerine tıklayarak aşağıdaki alanları doldurmanız gerekmektedir.

|Alan Adı|Açıklama|
|--|--|
|EFY_STOKKODU||
|EFY_FIYATTIPI||
|EFY_PARABIRIMI||
|EFY_FIYAT||
|EFY_FIYAT_INDIRIMLI||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||
|||