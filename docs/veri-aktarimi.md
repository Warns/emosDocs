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

|Alan Adı|Açıklama|
|--|--|
|EUR_URUN_KODU|Aktarılacak ürüne ait Ürün kodu bu alana girilmelidir.|
|EUR_AD|Aktarılacak ürüne ait Ürün adı bilgisi bu alana girilmelidir.|
|EUR_MARKA|Aktarılacak ürünü bağlamak istediğiniz marka entegrasyon kodunu bu alana yazmalısınız.<br><br>❗ _Eğer Daha önce oluşturulmamış bir entegrasyon kodu yazarsanız. Buraya yazacağınız bilgi ile yeni bir marka oluşturulacaktır. Marka Tanımları hakkında bilgi almak için [Tıklayın](marka-tanimi.md)._|
|EUR_VERGI|Aktarılacak ürüne bağlamak istediğiniz Vergi Tipi adını bu alana yazmalısınız.|
|EUR_RESIMLER|Aktarılacak ürüne bağlamak istediğiniz görsellerin FTP deki yollarını bu alana yazmalsınız. Birden fazla görsel yolunu virgül ile ayırmalısınız.|
|EUR_OZELLIK|Aktarılacak ürüne ait Açıklama metnini bu alana girmelisiniz. Bu alanda html kullanabilirsiniz.|
|EUR_KAT_KODU|Aktarılan ürüne bağlamak istediğiniz kategori ent. kodunu bu alana girebilirsiniz. Birden fazla kategori için virgül kullanmalısınız.|
|EUR_KODU_UST|Eğer aktarılacak ürün, Bir Grup Ürünü ise EUR_GRUP_FL alanı TRUE olan bir grup ürün kodunu bu alana girmeliyiz. Değilse Boş bırakabiliriz.	|
|EUR_GRUP_FL|Eğer tanımlanan ürün bir Ürün Grubu ise Bu alanın TRUE olması gerekiyor aksi durumda FALSE girilmelidir.<br><br>Ürün Grubu Tanımı hakkında ayrıntılı bilgi almak için [Tıklayın](urun-grubu-tanimi.md)|
|EUR_AD_KISA|Grup ürün kurgusundaki ürünleri birbirinden ayıran alt isimlerdir. Eğer grup ürün aktarmıyorsanız boş geçebilirsiniz.|
|EUR_KISAACIKLAMA|Bu alan Ürün Tanımındaki Kısa Açıklamaya denk gelmektedir.<br><br>Ürün Tanımı hakkında ayrıntılı bilgi almak için [Tıklayın](urun-tanimi.md)||
|EUR_URUN_ONYUZKODU|Ürüne ait ürün kodu bu alana girilir.|
|EUR_DESI|Ürüne ait desi miktarı buraya yazılmalıdır.<br><br>Nakliye Tanımı hakkında ayrıntılı bilgi almak için [Tıklayın](nakliye-tanimi.md)||
|EUR_SATISKATI|Ürüne ait satış katları bu alana girilmelidir.|
|EUR_IMAGEZOOM|Ürün Görsellerinde imagezoom özelliği aktif edilecekse bu alana TRUE aksi durum için FALSE girilmelidir.|
|EUR_ONAY_FL|Ürünün Onayı için TRUE/FALSE değer girilmelidir.<br><br>❗ _Excel aktarımı tamamlanıp, entegrasyon çalıştırıldığında eğer ürünün Onayı varsa direk önyüze yansıyacaktır.<br>İlk olarak onaysız bir şekilde aktarılmasını öneriyoruz. Ara bir kontrolden sonra toplu olarak Ürün Yönetimi sayfasından onaylarını verebilirisiniz._|
|LNG_CULTURENAME|Aktarılan ürünün hangi dilde aktarıldığını bu alan belirleyecektir.<br><br>❗ _Eğer bir ürünü birden fazla dilde tanımlamak istiyorsanız bu işlemi yeni bir satırda gerçekleştirebilirsiniz. Virgülle ayrım burada işe yaramayacaktır._|
|TEDARIKCI_KOD|Eğer Ürüne ait tedarikçi aktarımı olacaks Tedarikçiye ait Tedarikçi id bilgisini bu alana girmelisiniz.<br><br>Tedarikçi tanımı hakkında ayrıntılı bilgi almak için [Tıklayın](tedarikci-tanimi.md)|
|EUR_OZEL_AD1|Sistem işleyişinde ürün için özel bir kurgu ile bu alanlar kullanılıyorsa, bu alana ilgili metni girmelisiniz. Örn. daha önce çalıştığımız bir firmada ürünlere Yayın Evi ve Yazarlar bağlamak için Özel Alan 1 ve 2 kullanılmıştık. Eğer bu şekilde özel bir durum söz konusu değilse bu alanları boş bırakabilirsiniz.|
|EUR_METADESCRIPTION|SEO (Search Engine Optimization) arama motorları için kullanılan meta description alanına karşılık gelir.|
|EUR_SAYFABASLIK|Ürünün adının yazılacağı alana karşılık gelir. Aynı zamanda internet tarayıcısı üzerinde de bu başlık görünür.|
|EUR_SAYFAISMI|Ürün URL'ine karşılık gelir. <br><br>❗ _Ürün URL'leri "/" veya ".html" ile bitmesi gerekir._|
|EUR_URUNTIPI|Ürün tipine karşılık gelir.<br><br>❗ _Ürün Tipi hakkında ayrıntılı bilgi almak için [Tıklayın](diger-tanimlar.md#urun-tipi) |
|EUR_SERVIS_FL|Servis (Kurulum, monte vs) gerektiren ürüne karşılık gelir.|
|EUR_STYLE|Frontend ekibi tarafından önyüzü özelleştirmek için kullanılan Class alanına karşılık gelir.|
|EUR_KISAKOD|Ürünün kısa koduna karşılık gelir. Kısa kod ürün kodundan farklı olabilir. Ön yüzde farklı bir gösterim için de kullanılabilir.|
|EUR_GUMRUKTIPI|Gümrük tipine karşılık gelir. |
|EUR_ACIKLAMA2|Ürünün detaylı açıklama alanına karşılık gelir. Bu alana HTML kod da eklenebilir.|
|EUR_YENIURUN_FL|Ürünün yeni olup olmadığını belirtir. Entegrasyonda bu gibi bir ayar eklendiyse her yeni ürün geldiğinde bu alanın otomatik olarak seçilmesi ayarlanabilir.|
|EUR_TEKSATILAMAZ_FL|Ürün tek satılamaz. Birlikte satılan veya birden çok parçaya sahip ürünler için geçerlidir.|
|EUR_MAXTAKSITSAYISI|Alışveriş yaparken ilgili üründen maksimum yaralanabilecek taksit sayısına karşılık gelir.|
|EUR_LISTEGOSTERILMESIN_FL|Herhangi bir ürünü ürün listede görünmemesini sağlamak için kullanılır.|
|EUR_MINADET|Üründen tek seferde satın alınabilecek minimum ürün adedi.|
|EUR_MAXADET|Üründen tek seferde satın alınabilecek maksimum ürün adedi.|
|EUR_AGIRLIK|Ürünün ağırlık bilgisnin belirtildiği alandır.
|EUR_OZS_KOD|Ürüne ait Özellik Setinin belirtildiği alandır.|
|EUR_TESLIMSURESI|Ürünün teslim süresine karşılık gelir. Gün olarak çalışan bu alan, Pazaryeri modülü için de kullanılabilir.<br><br>❗ _Sağlıklı çalışması için bu alan kargo firmasıyla anlaşmalı olarak belirtilmeli_|


Bu alanları doldurup dosyayı seçtikten sonra, Ürün Listele sol menüsü üzerindeki yükle butonu ile ürünleri ara tabloya yükleyebilirsiniz.

<br>
### 2.2. Fiyat Aktarımı
Fiyat aktarımı yapmak için Price sheetinin üzerine tıklayarak aşağıdaki alanları doldurmanız gerekmektedir.

|Alan Adı|Açıklama|
|--|--|
|EFY_STOKKODU|Stok kodu|
|EFY_FIYATTIPI|Fiyat tipi|
|EFY_PARABIRIMI|Para birimi|
|EFY_FIYAT|Fiyat|
|EFY_FIYAT_INDIRIMLI|İndirimli fiyat|
