---
id: site-ayarlari
title: Site Ayarları
---

Parametrik bir altyapıya sahip olan e-MOS'un çalışma şeklini belirleyecek olan tanımlamaların yapıldığı sayfadır.

## 1.  Sipariş Ayarları
Sipariş işlemlerinde öndeğer olarak kullanılacak olan tanımların girildiği bölümdür.

- #### Sistem 

|Alan Adı|Açıklama|
|--|--|
|Alışveriş Sepeti Temizleme Süresi|Ürünlerin sepete eklendiği fakat alışverişin tamamlanmadığı durumlarda kullanıcının sepetinde ürünlerin kaç gün kalacağını belirleyen parametredir.|
|Content Sunucu Ayaları|Ürün resim ve dokümanları siteden farklı bir sunucuda konumlandırılıyorsa bu alan kullanılır. Directory ismi ve url olarak bilgi girilir.|DirectoryName,ContentServerDomain<br>örn: downloads, http://download.site.com|
|Sunucu Cache Dakikası|Sayfaların sunucu cache'sinde kaç dakika kalacağını belirleyen parametredir.|10|
|Tasarım Doc Type|Site tasarımı için gerekli bir parametredir.||
|SSL Sayfaları|||
|Önyüzden Güncelleme İzni|||
|Mail Server|||
|Fatura Tarihi|||
|Navigasyonlu Title|||
|Kullanıcı Bloke|Kullanıcı site üzerinde belli bir süre fazla istek yaptığı durumda sistem kullanıcıya bloke işlemi uygulamaktaydı ancak bu süre tüm kullanıcılarda aynı olmak zorundaydı. Bu nedenle “Kullanıcı Bloke” işlemi “Site Ayarları”na taşınmıştır ve Site Yönetimi > Sistem Ayarları > Kullanıcı Bloke adı altında site ayarı eklenmiştir. Bu alana hiçbir değer girilmediği durumda Kullanıcı Bloke özelliği "Pasif" durumda olacaktır. Bloke işlemi aşağıda belirtilen örneğe istinaden, 30 saniye içerisinde 30 istek yapıldığında 120 saniye kullanıcıyı bloke edecektir. Bu bloke işleminin amacı siteye yapılan sahte istekleri ve sahte kullanıcıları bir süreliğine de olsa durdurma amaçlıdır. Bloke işleminin çalışmasını sağlayan durumlar olduğunda ( yani siteye 30 saniye içerisinde, 30 istek yapıldığında) kullanıcının karşısına güvenlik kodunu girmesi için bir ekran gelecek ve kullanıcı bu güvenlik kodunu kutucuğa girdiğinde bloke işleminin gerçekleştiği sayfaya geri dönecek , siteyi ziyaret etmeye devam edebilecektir.|Kullanıcı fazla istek yapınca geçici süre bloke olsun mu? 1. Parametre: Kontrol süresi, 2. Parametre: İşlem adeti, 3. Parametre: Blok süresi. <br>Örnek: 30,30,120|
|UPS API Kullanıcı Bilgileri|UPS entegrasyon sağlandığında "Satış Faturaları" ekranında otomatik olarak fatura bazlı "UPS'e Bildir" butonu aktif olmaktadır. Bu butona tıklanınca fatura bilgilerindeki ürünler, teslimat adresi ve alıcı bilgileri UPS kargo sistemine bildirilerek, alınan onay sonrası UPS sevkiyat barkodu hazırlanmaktadır. Bu barkod etiket yazıcısı üzerinden dökülebilecek formattadır.|Müşteri parametresinin doğru bir şekilde " ;" ile ayrılarak girilmesi gerekmektedir.|
|Captcha Bilgileri|Captcha kontrolü dinamik olarak çalışmaktadır. Captcha kodu sayıdan, karakterden veya hem sayı hem karakterden oluşabilmektedir <br>1. Değer = Captcha sayıdan, karakterden veya hem sayı hem karakterden oluşsun (0: Sadece Sayı, 1: Sadece karakter, 2: Hem sayı hem de karakter)<br>2. Değer = Oluşturulan Captcha kontrolünün büyük harf veya küçük harf olması (B: Büyük, K: Küçük, H: Büyük/Küçük) <br>3. Değer = Yazı fontu (Times New Roman,Arial vs.) <br>4. Değer = Yazı boyutu <br>5. Değer = Yazı rengi (White,Black,Red vs.) <br>6. Değer = Captcha arka plan rengi (White,Black,Red vs.) <br>7. Değer = Captcha genişliği <br>8. Değer = Captcha yüksekliği <br>9. Değer = Captcha desen kodu (Bkz .Tablo 1) olarak değerler girilerek captcha kontrolünün dinamikleştirilmesi sağlanır. <br>❗ _Parametre boş geçilir veya eksik değer girilir ise captcha da değişiklik olmamaktadır._|1(Sadece Karakter);H(Büyük Küçük Harf);Times New Roman(Yazı Tipi);45(Yazı Tipi Boyutu);White(Yazı Rengi);Red(Captcha Arka Plan Rengi);200(Captcha Genişliği);50(Captcha Yüksekliği);42(Captcha deseni) |

- #### Diğer

|Alan Adı|Açıklama|
|--|--|
|İndirim Yüzdesi|Önyüzde indirimli ürünler menüsü altında görülmesini istediğiniz ürünler için minimum indirim oranı girilir. Bu değerin altında indirim oranı tanımlanmış ürünler, indirimli ürünler listesinde gözükmeyecektir.||
|Promosyon Görünme Süresi|Ürünlerin önyüzde listelendiği kısımda promosyonların bitmesine belirli bir gün kaldığında uyarı çıkarılması sağlanabilir. ("Son 5 Gün!" gibi) Bu uyarının promosyonun bitiş tarihine kaç gün kaldığının çıkarılacağını Promosyon Görünme süresi parametresi belirlenir.<br>❗  _Promosyon bitiş tarihi girilmeyen promosyonlarda, bu parametre geçerli olmayacaktır._||
|Session Timeout|Üyenin kullanıcı adı ve şifreyle giriş yaptıktan sonra hiçbir işlem yapmadan kalabileceği zaman sınırlandırmasının girildiği alandır. (dakika)||
|Otomatik Paket İçeriği Aktif*** | Sipariş Takibinde **Ödendi** kutucuğu işaretlendiğinde otomatik olarak paketleme işlemlerinin yapılmasını istenilirse bu değer 1 yapılır. Eğer bu işlem manuel olarak yapılmak istenirse 0 girilir.<br>❗  _Otomatik paketleme 1 yapıldığında, sipariş fatura güncelleme sayfasında paketleme işlemine giden bir link oluşacaktır._||
|Mail Aktivasyonun Aktif mi|Üyelerin üyeliklerin onaylanması işleminde mail aktivasyonunun kullanılması için 1 , kullanılmaması için 0 yapılmalıdır. 0 yapıldığında üyelik bilgilerini giren her üye aktif üye olarak sisteme dahil olur.<br>❗ _SMS ayarları içerisindeki SMS aktivasyonu yapılabilmesi için mail aktivasyonunun aktif olması gereklidir. Çünkü mail ile gönderilen linke tıklandığında açılan sayfa üzerinde gelen SMS onay kodu girilmektedir._|1 , 0|
|Yıllık Finansman Oranı|Maliyetlendirmede ürünler üzerine uygulanacak Yıllık Finansman Oranının girildiği alandır.||
|Maliyet Başlangıç Tarihi|Bir sonraki maliyet çalıştırıldığında hesaplamanın başlayacağı tarihin girildiği alandır.|01.01.2008|
|Maliyet Tipi|Stok maliyet çalıştırma şekli Ortalama Maliyet=1,FIFO Maliyet=2 şeklinde girilicek olan alandır.|1|
|Yapı Kredi Ek Taksit Tutarı|Yapı Kredi Bankası Ek Taksit Kampanyalarından faydalanmak için girilen minimum tutardır. 0 TL üzerinde çalışır.||
|Sepete Atma İşlemi|Sepete Atma işlemi sırasında ziyaretçinin otomatik olarak sepet görüntüleme sayfasına yönlendirilip yönlendirilmeyeceğinin belirlendiği alandır.|1 yönlendir, 0 yönlendirme|
|Üye Login Hatırlama|Login olan bir ziyaretçinin bir sonraki ziyaretinde hatırlanıp hatırlanmayacağının belirlendiği alandır.||1 hatırla, 0 hatırlama
|En Çok Satanların Süresi|En çok satan ürünlerin son kaç gün için geçerli olduğununun belirlendiği alandır.||
|Üyelik İptal|Ziyaretçilerin üyeliklerini siteden iptal edip edemeyeceklerinin belirlendiği alandır.|1 edebilir, 2 edemez|
|Kategori Süzülsün mü?|Yeni ürünler, indirimdekiler ve en çok satanlar gruplarındaki ürünlerin kategori ağacına göre süzülüp süzülmeyceğinin belirlendiği alandır.|1 süzülsün, 0 süzülmesin|
|Merkez Bankasından Kurlar Otomatik Alınsın mı?|Merkez Bankası'ndan güncel kurların otomatik olarak alınmayacağına karar verilen alandır.|1 alınsın, 0 alınmasın|

- #### Bonus Ayarları

Bonus kullanımı ve kazanma oranlarının tanımlanabilineceği yerdir.

|Alan Adı|Açıklama|
|--|--|
|SİTE BONUS Görüntülenme Sınırı	|Müşterinin bonus hesabında kullanabileceği tutarı görebilmesi için sahip olması gereken minimum bonus tutarı bu parametre ile belirlenir.|
|BANKA BONUS Görüntülenme Sınırı	|Üyenin kredi kartında biriken bonus para görüntülenebilmesi için gerekli alt sınırın belirlendiği alandır. Eğer üyenin bonusu bu değeri geçerse siparişlerinde kullanma hakkını kazanacaktır.|
|Reklam Bonus Uyarı Sınırı	|Tavsiye Raporunda kazanılan bonus için bu değerden büyük olanların yönetim panelinde rengi farklı olarak görüntülenir. Değer TL olarak girilmelidir.	|
|Üye Yorum Kazanılan Bonus Miktarı	|Kullanıcının ürünlere yorum yaptığında kazanacağı bonus miktarının girileceği alandır.	|

- #### Ürün Ayarları

|Alan Adı|Açıklama|
|--|--|
|Küçük Sepet Ürün Adeti	|Sepet içeriğinin ürün detaylı olarak görüntülenebileceği max. ürün adedinin belirlendiği alandır. Bu değerin üzerine çıkıldığında ürün bilgisi gösterilmez, sepetteki toplam ürün adedi ve tutarı güncellenir.<br>❗ _Satın alma işlemine geçildiğinde görüntülenen sepet için bu parametre geçerli değildir, sepet içerisindeki tüm ürünler gösterilir._ ||
|Paket Ürün Kodu Formatı	|Paket ürün koduna eklenmek istenilen ön ekin girildiği alandır.	|PKT --> PRI000023|
|Ürün Kodu Formatı	|Yeni ürün tanımlarken oluşturulan ürün koduna eklemek istenen ürün kodu formatı girildiği alandır.|MYU girilirse ürün kodu MYU00001 şeklinde oluşur.|
|Promosyonlu Ürün Kodu Formatı	|Yeni Promosyon ya da indirim tanımlarken oluşturulan promosyon-indirim koduna eklenmek istenilen ön ekin girildiği alandır.	|PRI --> PRI000123|
|Banka Taksit Kolon Sayısı	|Taksitlerin gösteriminde yan yana kaç banka görüntüleneceğinin belirlendiği alandır.	||
|Sepette Maximum Ürün Adedi****	|Ürün sınıfı bazında satın alınabilecek maksiumum ürün adedinin beirlenbdiği alandır.||
|Ürün Rating	|Ürünleri oylamak için yorum yazmanın zorunlu olup olmadığının belirlendiği alandır.	|1: zorunlu, 0: zorunlu değil|
|Ürün Açıklama Alanları Aktif/Pasif	|Sitede uzun ve kısa açıklama alanlarının bulunup bulunmayacağının belirlendiği parametredir.	|UA = Uzun Açıklama, KA = Kısa Açıklama, 0 pasif 1 aktif. Örn:UA1:1;UA2:1;KA1:1;KA2:1|
|Vitrin Kategori Görünsün mü	|Kategori ağaç yapısının en üst kısmında **indirimli ürünler, paket ürünler, promosyonlu ürünler, yeni ürünler, vitrin ürünler** başlıklarının görüntülenip görüntülenmeyeceğinin belirlendiği alandır.<br>❗ _Yapılan değişikliğin görülebilmesi için sayfanın yenilenmesi yerine kapatılıp tekrar açılması gerekmektedir._|1: görüntülensin, 0: görüntülenmesin|

- #### Resim Ayarları

Siteye eklenilen resimlerle ilgili genel ayarların yapılacağı sayfadır.

>❗ _Ürün resimlerinin gönderilmesi iki şekilde yapılabilir. Upload modülü ve FTP. 
Upload ile ürünün resmi eklendiğinde, düzenlenmesi gereken diğer boyutları thumb klasörü içerisinde anında oluşturulur. Burada dikkat edilmesi gereken nokta, resmin diğer boyutları için sistem otomatik isimler üretir. (mama_kabi.jpg için, mama_kabi_small.jpg gibi) Eğer ürünün thumb resimleri daha önceden oluşturulduysa örnekteki mama_kabi_small.jpg zaten var olduğundan sistem yeniden bu resmi oluşturmayacaktır. mama_kabi_small.jpg thumb klasöründen silinirse ve upload modülünde ana resmin eklendiği klasöre giriş yapılırsa sistem yeniden oluşturacaktır. 
FTP ile resim gönderildiğinde de aynı şekilde thumbların oluşması için upload modülü ile resmin gönderildiği klasöre giriş yapılmalıdır._

|Alan Adı|Açıklma|
|--|--|
|Resim Arka Plan Rengi |Resmin arka plan rengi olarak görüntülenmesi istenilen rengin RGB kodu yazılır. (beyaz için "#ffffff")	|#ffffff|
|Zoom ImageSize |Ürünün detay resminde Zoom Image modülü kullanılıyor ise, resmin gerçek boyutları, aralarında virgül koyularak genişlik ve yükseklik şeklinde tanımlanır.|1772,1772|
|Image Size	|Ürünün sitede görüntülenecek en büyük boyutu belirlenir. Bu boyutun üzerindeki değerlerde resim verildiğinde sistem bu boyuta küçültecektir. Aynı şekilde bu boyuttan daha küçük bir resim verildiğinde, "Resim Arka Plan Rengi" parametresi kullanılarak verilen resim maksimum boyutların ortasına oturtulacak ve arka plan rengi verilen parametreye göre düzenlenecektir.|400,400|
|WaterMark Url|Siteden yüklediğiniz resimlerin çalınmasın engellemek için thumb ı oluşturulacak her resme koyulacak hafif saydam bir resim belirlenir. Bu resmin url bilgisi parametre olarak tanımlanmalıdır.<br>❗ _WaterMark resminin Image size boyutları ile aynı olması faydalı olacaktır. O boyutlarda resmin içeriği nereye oturtulduysa, üzerine işlenen ürün resimlerinde de aynı yerden oluşacaktır._|/images/waterMark.gif|
|Flash Image Size	|Flash Popup Boyutlarının belirlendiği alandır.|512,284|
|Zoom Tipi|Ziyaretçinin ürün fotoğrafarını hangi yaklaştırma yöntemi ile göreceğinin belirlendiği alandır.|1: Klasik Zoom, 2: Cloud Zoom|
|Thumb Küçük Image Genişlik|Sitede gösterilecek küçük boydaki resimlerin genişliği tanımlanır. Yükseklik değeri, Image Size parametresinde verilen orana göre otomatik olarak hesaplanacaktır.|110|
|Thumb Orta Boy Image Genişlik|Sitede gösterilecek orta boydaki resimlerin genişliği tanımlanır. Yükseklik değeri, Image Size parametresinde verilen orana göre otomatik olarak hesaplanacaktır.|220|
|Lazy Load Aktif mi?	|Lazy Load, yüklenecek nesnelerin tamamını yüklemek yerine kullanıcıyla etkileşime gireceği anda yada kısa bir süre önce hafızaya yüklemek demektir. Örnek olarak; Ürün liste sayfasında bulunan ürün görsellerinin sayfayı scroll ettikçe açılması.|0: Pasif, 1: Aktif|

- #### Sms Ayarları
Siteden sms gönderebilmek için yapılması gereken ayarların tanımlandığı sayfadır.

|Alan Adı|Açıklama|
|--|--|
|SMS aktivasyon aktif mi?	|Üyelik işlemlerini sms aktivasyonu ile gerçekleştirmek isteniliyorsa bu değer 1 yapılır. Aktivasyon işlemi sms ile yapılmak istenmiyorsa bu değer 0 yapılmalıdır.<br>❗ _SMS ayarları içerisindeki SMS aktivasyonu yapılabilmesi için mail aktivasyonunun aktif olması gereklidir. Çünkü mail ile gönderilen linke tıklandığında açılan sayfa üzerinde gelen SMS onay kodu girilmektedir._|
|Kargo verildi Sms'i aktif mi ?	|Ürün durumu kargoya verildi seçeneği işaretlendiği zaman müşteriye Siparişiniz kargoya verildi SMS mesajı gitmesi isteniliyorsa bu değer 1, istenilmiyorsa bu değer 0 yapılır.|
|SMS Sağlayıcı : ***	|Sms sağlayıcınızın url bilgisi girilir. Sistemde şu anda CMFCELL firması ile entegrasyon mevcuttur. Bu firma için link [http://app.cmfcell.com/httppost/requestxml.aspx] olmalıdır. SMS kontör satın alma işlemi [http://www.cmfcell.com] adresinden yapılabilmektedir.|
|Kullanıcı Adı |SMS sağlayıcınızdan alınan kullanıcı adının girildiği alandır.|
|Şifre|SMS sağlayıcınızdan alınan şifrenin girildiği alandır.|
|Sipariş alındı Sms'i aktif mi?	||

- #### Merkez Yönetim
Siteden sms gönderebilmek için yapılması gereken ayarların tanımlandığı sayfadır.

|Alan Adı|Açıklama|
|--|--|
|Ürün Merkezi Tanım Olsun ||
|Taşıyıcı Mekezi Olsun ||
|Ödeme Tipi||
|Gider Tanımı||

- #### Entegrasyon Ayarları

Entegrasyon bilgilerinin girildiği alandır.

|Alan Adı|Açıklama|
|--|--|
|Paro İşyeri Kodu |Paro Entegrasyonunda kullanılacak İşyeri kodunun girileceği alandır.|
|Paro Pc ID|Paro Entegrasyonunda kullanılacak PC id bilgisinin girileceği alandır.|
|Paro Şube Kodu|Paro Entegrasyonunda kullanılacak Şube kodunun girileceği alandır.|
|Paro Web Service URL|Paro Entegrasyonunda kullanılacak Web Service URL ' inin girileceği alandır.|
|Paro Yetkili Kodu|Paro Entegrasyonunda kullanılacak Yetkili kodunun girileceği alandır.|
|Sip. İptal Web Service URL|Sipariş iptal talebi sırasında kullanılacak dış sistem web servisine ait url bilgisinin girileceği alandır.|
|Sip. Onay Web Service URL|Sipariş onay sırasında kullanılacak dış sistem web servisine ait url bilgisinin girileceği alandır.|
|Sip. Rezervasyon Web Service URL |Sipariş Rezervasyonu sırasında kullanılacak dış sistem web servisine ait url bilgisinin girileceği alandır.|
|Stok Sorgu Web Service URL|Stok sorgu sırasında kullanılacak dış sistem web servisine ait url bilgisinin girileceği alandır|
|FTP_KOD1|Entegrasyonda kullanılacak 1.fiyat tipine ait fiyat tipi kodunun girileceği alandır.Not: Fiyat Tipine ait kodu, Tanımlar menüsü altında Fiyat Tipi Tanımı bölümünden alabilirsiniz.|
|FTP_KOD2|Entegrasyonda kullanılacak 2.fiyat tipine ait fiyat tipi kodunun girileceği alandır.Not: Fiyat Tipine ait kodu, Tanımlar menüsü altında Fiyat Tipi Tanımı bölümünden alabilirsiniz.|
|FTP_KOD3|Entegrasyonda kullanılacak 3.fiyat tipine ait fiyat tipi kodunun girileceği alandır.Not: Fiyat Tipine ait kodu, Tanımlar menüsü altında Fiyat Tipi Tanımı bölümünden alabilirsiniz.|
|ENT_FIYATTIPI1|Entegrasyonda kullanılacak 1.fiyat tipi adının girileceği alandır.Not: Fiyat Tipi adını, Tanımlar menüsü altında Fiyat Tipi Tanımı bölümünden alabilirsiniz.|
|ENT_FIYATTIPI2|Entegrasyonda kullanılacak 2.fiyat tipi adının girileceği alandır.Not: Fiyat Tipi adını, Tanımlar menüsü altında|
|ENT_FIYATTIPI3|Entegrasyonda kullanılacak 3.fiyat tipi adının girileceği alandır.Not: Fiyat Tipi adını, Tanımlar menüsü altında Fiyat Tipi Tanımı bölümünden alabilirsiniz.|
|SCM_KOD1|Entegrasyonda kullanılacak stok kodu1(renk) bilgisinin girileceği alandır.|
|SCM_KOD2|Entegrasyonda kullanılacak stok kodu2(beden) bilgisinin girileceği alandır.|
|ENT_URUNDUZENLE_FL|Entegrasyon ürün düzenle çalışacak mı? Bilgisinin girileceği alandır.|
|CepBank_Id_MerchantId_Password	|Cepbank bilgilerinin( Cepbank_Id, MerchantId, Password) girileceği alandır. Not:CepBank için Id, MerchantId, Password numaralarını virgül ile ayırarak giriniz|
 
- #### Sosyal Ağ Ayarları
Sosyal ağ ayarları bilgisinin girildiği alandır.

|Alan Adı|Açıklama|
|--|--|
|Facebook App Id|Facebook tarafında oluşturulan uygulamanın App ID değerinin girileceği alandır.|
|Facebook App Message|Facebook tarafında oluşturulan uygulamanın App Message değerinin girileceği alandır.|
|Facebook App Name|Facebook tarafında oluşturulan uygulamanın App Name değerinin girileceği alandır.|
|Facebook Return Url|Facebook tarafında oluşturulan uygulamanın Return URL değerinin girileceği alandır.|
|Google App Name |Google tarafında oluşturulan uygulamanın App Name değerinin girileceği alandır.|
|Windows Live|Windows Live tarafında oluşturulan uygulamanın ID değerinin girileceği alandır.|
|Windows Live Secret|Widows Live tarafında oluşturulan uygulamanın Secret değerinin girileceği alandır.|
|Yahoo! Consumer Key|Yahoo tarafında oluşturulan uygulamanın Consumer Key değerinin girileceği alandır.|
|Yahoo! Consumer Secret|Yahoo tarafında oluşturulan uygulamanın Consumer Secret değerinin girileceği alandır.|
|Sözleşme onaylı Facebook Login|Kullanıcı siteye ilk kez Facebook ile giriş yapmak istediğinde karşısına pop-up içerisinde sözleşme metni çıkacaktır. Kullanıcı bu sözleşme metnini onayladıktan sonra siteye Facebook ile girişini tamamlamış olacaktır.|

- #### Thumbnail Tanımlama

Yeni kayıt ekleme aşamasında Dizin Adı ve Resim Boyutu alanı girilmesi zorunlu alanlardır. Bu alanlar doldurulmadan kayıt eklenemez. **Alt Dizin İçin Geçerli Mi?** alanı işaretlenmez ise otomatik olarak false kabul edilmektedir. Sıra alanı boş geçilirse otomatik olarak son sıranın bir üzerini sırayı vererek ekler. 

Örneğin;

***Buraya screenshot gelicek***
