####Parametreler

**Temel Parametreler:** Tüm sayfalarda kullanılabilecek parametrelerdir. Herhangi bir ön ek içermez. Kullanımı “$PARAMETRE_ADI$” şeklindedir. İlgili parametreler aşağıdaki gibidir;

####1. Sekme (Genel Bilgiler)

|Parametre Adı|Açıklama|
|--|--|
|prmPageName:|Aktif sayfanın adını lower case(küçük harf) olarak verir. Örn: Ürün detay sayfasında “/urun_detay.aspx”, Sipariş sonuç sayfasında “/siparis/siparissonuc.aspx”.|
|prmHostName:|Aktif sitenin host bilgisini verir. Örn: www.proj-e.com sitesi için “proj-e.com” şeklinde bilgi verir.|
|prmPageProtocol:|Site üzerinde etkin olan sayfanın protocolünü verir. Örn: https’li bir sayfa için “https”, http bir sayfa için “http” bilgisini verir.|
|prmSiteType:|Aktif site üzerinde istemcinin hangi cihaz üzerinden bağlandığı bilgisini verir.(mobile, tablet ya da desktop). Örn: Mobile için “m”, Tablet için “t”, Desktop için “d” şeklinde bilgi verir.falarda header/footer içeriklerinin çalıştırılması engellenebilir.|
|Url QueryString:|Url Querystring üzerinden bir parametre alabilmek için “ $rqPARAMETRE_ADI$ ” formatı kullanılmalıdır. Örn: www.siteadi.com/default.aspx?t=123456 url’si üzerindeki “t” parametresinin değerini alabilmek için “ $rqt$ ” şeklinde yazılmalıdır. Tüm sayfalarda kullanılabilir.|
|Session:|Session üzerinde olan bir değeri alabilmek için “$ssPARAMETRE_ADI$” formatı kullanılmalıdır. Tüm sayfalarda kullanılabilir. Örn: www.siteadi.com sitesi üzerinde aktif olan üyenin ID bilgisinin “UYE_KOD” adında bir session’unda saklandığını varsayalım. Bu durumda bu bilgiye erişebilmek için “$ssUYE_KOD$” şeklinde kullanım yapılmalıdır.|

####Sayfalara Göre Kullanılabilecek Parametre Bilgileri:

Parametre isimleri birleşiktir. Herhangi bir karakter ile ayrılmaz.(alt tire, tire v.s.). Aldığı ön ek ile kullanılır. Kullanım şekli “ $ onek(s1,s2,s3,s4,s5)_PARAMETREADI $” dir.

**Anasayfa:** Anasayfa için kullanılabilecek özel bir parametre yok.

**Ürün Detay:** 2 set döndürür. 1. set ürün bilgilerini tutarken 2. set ürün özelliklerini tutar.

####Set 1 Parametreleri(s1):

|Parametre Adı|Açıklama|
|--|--|
|URNID|Aktif ürünün Ürün ID bilgisini verir.|
|URNKOD|Aktif ürünün Ürün Kodu bilgisini verir.|
|URNAD|Aktif ürünün Ürün Adı bilgisini verir.|
|URNADFILTERED|Aktif ürünün Ürün Adı bilgisini Türkçe karakterlerden arındırılmış bir şekilde verir.|
|URNFREESTOK|Aktif ürünün kullanılabilir stok bilgisini verir.|
|URNFIYAT|Aktif ürünün KDV dahil satış fiyatını verir.|
|URNFIYATKDVSIZ|Aktif ürünün Ürün Adı bilgisini verir.|
|PBSPRAD|Aktif para biriminin adını verir.(TL, USD, EUR gibi)|
|KATKOD|Aktif ürünün kategori ID bilgisini verir.|
|KATKODLAR|Aktif ürünün bağlı olduğu kategori hiyerarşisinin ID bilgilerini verir.|
|KATKATEGORILER|Aktif ürünün bağlı olduğu kategori hiyerarşisinin adlarını verir.|
|URNRESIMMEDIUM|Aktif ürünün medium olarak ürün resmini verir.|

####Set 2 Parametreleri(s2):

|Paratmetre Adı|Açıklama|
|--|--|
|URNID|Aktif olan ürünün ID bilgisini verir.|
|OPRKOD|Aktif olan ürünün özellik parametre ID bilgisini verir.|
|OPRAD|Aktif olan ürünün özellik parametre adı bilgisini verir.|
|OPSID|Aktif olan ürünün özellik parametre seçenek ID bilgisini verir.|
|PSAD|Aktif olan ürünün özellik parametre seçene adı bilgisini verir.|

**Ürün Liste:** 2 set döndürür. 1. set aktif kategori bilgilerini tutarken 2. set ürünleri tutar.

####Set 1 Parametreleri(s1):

|Parametre Adı|Açıklama|
|--|--|
|KATKOD|Aktif kategorinin kategori ID bilgisini verir.|
|KATAD|Aktif kategorinin kategori adı bilgisini verir.|
|KATKODLAR|Aktif kategorinin bağlı olduğu hiyerarşinin ID bilgilerini verir.|
|KATKATEGORILER|Aktif kategorinin bağlı olduğu hiyerarşinin kategori ad bilgilerini verir.|
|KATKODUST|Aktif kategorinin bağlı olduğu üst kategorinin ID bilgisini verir.|

####Set 2 Parametreleri(s2):
|Parametre Adı|Açıklama|
|--|--|
|URNID|Aktif satırdaki ürünün ID bilgisini verir.|
|URNKOD|Aktif satırdaki ürünün ürün kodu bilgisini verir.|
|URNAD|Aktif satırdaki ürünün adını verir.|
|URNADFILTERED|Aktif satırdaki ürünün adını Türkçe karakterlerden arındırlmış olarak verir.|
|URNFREESTOK|Aktif satırdaki ürünün kullanılabilir stok bilgisini verir.|
|URNFIYAT|Aktif satırdaki ürünün KDV dahil fiyat bilgisini verir.|
|PBSPRAD|Aktif satırdaki ürünün para biriminin adını verir.|
|KATKOD|Aktif satırdaki ürünün bağlı olduğu kategorinin ID bilgisini verir.|
|KATKODLAR|Aktif satırdaki ürünün bağlı olduğu kategori hiyerarşisinin ID bilgilerini verir.|
|KATKATEGORILER|Aktif satırdaki ürünün bağlı olduğu kategori hiyerarşisinin ad bilgileri verir.|

####Set 1 Parametreleri(s1):

|Parametre Adı|Açıklama|
|--|--|
|ALVKOD|Aktif alışveriş sepetinin ID bilgisini verir.|
|URNSAYISI|Sepetteki toplan ürün adeti bilgisini verir.|
|TOPLAM|Sepetteki toplam fiyatı verir.|
|PBSPRAD|Aktif para birimini verir.|

**Sepet:** 2 set döndürür. 1. Set sepet genel bilgilerinin tutarken 2. Set sepetteki ürünleri tutar.

####Set 2 Parametreleri(s2):
|Parametre Adı|Açıklama|
|--|--|
|ALSKOD|Sepetteki aktif ürün bilgisinin sepetteki satır ID bilgisini verir.|
|ALVKOD|Aktif alışveriş sepetinin ID bilgisini verir.|
|URNID|Aktif ürünün ID bilgisini verir.|
|URNAD|Aktif satırdaki ürünün adını verir.|
|URNADFILTERED|Aktif satırdaki ürünün adını Türkçe karakterlerden arındırlmış olarak verir.|
|URNVRGORAN|Aktif ürünün vergi oranını verir|
|URNVRGTUTAR|Aktif ürünün vergi tutarını verir.|
|URNADET|Aktif satırdaki ürünün adını verir.|
|URNBIRIMFIYAT|Aktif ürünün birim fiyatını verir.|
|URNVRGLIBIRIMFIYAT|Aktif ürünün birim fiyatını vergil ile birlikte verir.|
|URNTOPLAMFIYAT|Aktif ürünün alınan adete göre toplam fiyatını verir.|
|URNKISAAD|Ürünün kısa ad bilgisini verir.|
|URNSCDAD1|Ürünün seçenek 1 bilgisini verir.|
|URNSCDAD2|Ürünün seçenek 2 bilgisini verir.|
|MRKAD|Aktif ürünün marka adı bilgisini verir.|
|KATKOD|Aktif ürünün kategori ID bilgisini verir.|
|KATKATEGORILER|Aktif ürünün bağlı olduğu kategori hiyerarşisini verir.|
|KATAD|Aktif ürünün varsayılan kategori bilgisini verir.|
|BRMSPRAD|Aktif ölçü birimini verir.|


**Sepet’e Ürün Ekle :** 2 set döndürür. 1. Set, eklenen ürün ile bilgileri tutarken 2. Set sepetteki ürünleri tutar.

####Set 1 Parametreleri(s1):

Ürün Detay için kullanılan parametreler bu aşama için de geçerlidir.

####Set 2 Parametreleri(s2):

**- ALVKOD**
**- URNID**
**- URNKOD**
**- URNADET**
**- URNFIYAT**
**- PBSPRAD**
**Sipariş Sonuç(Başarılı Sipariş Oluşturma):** 2 set döndürür. 1. Set siparişin genel bilgilerini içerirken 2. set siparişteki ürünleri tutar.

####Set 1 Parametreleri(s1):

**- SSMID**
**- SSMNO**
**- TOPLAM**
**- TOPLAMKARGOSUZ**
**- OPLAMKARGOSUZKDVSIZ**
**- VERGITOPLAM**
**- KARGO**
**- URNADETTOPLAM**
**- PBSPRAD**
**- UYEKOD**
**- UYEEMAIL**
**- UYECINSIYET**
**- UYESEHIR**
**- UYESIPARISSAYISI**

####Set 2 Parametreleri(s2):

**- SSMID**
**- SSMNO**
**- URNID**
**- URNKOD**
**- RNAD**
**- URNADFILTERED**
**- URNBIRIMFIYAT**
**- URNTOPLAMFIYAT**
**- URNTOPLAMFIYATKARGOSUZKDVSIZ**
**- URNADET**
**- KATKOD**
**- KATAD**
**- KATKATEGORILER**
**- KATKODLAR**

**Üye Login:** 1 set döndürür. 1. set üye ile ilgili bilgileri tutar.

####Set 1 Parametreleri(s1):

**- UYEID**
**- UYEEMAIL**
**- UYEFACEBOOKID**
**- UYEAD**
**- UYESOYAD**
**- UYEADSOYAD**
**- UYETELEFON**
**- UYECEPTELEFON**
**- UYEDOGUMTARIHI**
**- UYEDOGUMTARIHIGUN**
**- UYEDOGUMTARIHIAY**
**- UYEDOGUMTARIHIYIL**
**- UYECINSIYET**
**- UYELOKASYON**
**- FTPKOD**
**- ULKADI**
**- UMSSPRAD**
**- UYOSPRAD**

**Üye Kayıt(Başarılı):** 1 set döndürür. 1. set üye ile ilgili bilgileri tutar.

####Set 1 Parametreleri(s1):

Üye login için kullanılan tüm parametreler bu aşama için de geçerlidir.

**Üye Profil Güncelleme:** 1 set döndürür. 1. set üye ile ilgili bilgileri tutar.

####Set 1 Parametreleri(s1):

Üye Login için kullanılan tüm parametreler bu aşama için de geçerlidir.

**Üye Adres Ekleme & Güncelleme:** 1 set döndürür. 1. set eklenen/güncellen adres ile ilgili bilgileri tutar.

####Set 1 Parametreleri(s1):

**- UYEADSOYAD**
**- UYEFATAD**
**- UYEFATSOYAD**
**- UYEEMAIL**
**- UYEFATAD**
**- UYECEPTELEFON**
**- UYETELEFON**
**- UYATCKIMLIKNO**
**- UYEPOSTAKODU**
**- UYEADSOYAD**
**- ULKADI**
**- ULKKOD**
**- SHRADI**
**- SHRDIGER**
**- ILCADI**
**- MHLADI**

**İçerik:** 2 set döndürür. 1. set içerik ile ilgili genel bilgileri tutarken 2. set hiyerarşi bilgisini tutar.

####Set 1 Parametreleri(s1):

**- ICRID**
**- ICRAD**
**- ICRADLAR**
**- ICRKODLAR**

####Set 2 Parametreleri(s2):

**- ID**
**- SAYFAAD**
**- HIYERARSI**
**- KATSAYFAISMI**
**- SAYFARAPORAD**
**- KAT**
**- KATUST**
**- KATFL**

**Arama:** Sayfaya özel bir parametresi bulunmamaktadır.

**Tüm Diğer Sayfalar:** Sayfaya özel bir parametresi bulunmamaktadır.

