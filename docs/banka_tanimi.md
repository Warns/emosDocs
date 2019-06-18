Üyelerin önyüzden alışveriş yapmak için kullanacakları bankaların tanımlandığı sayfadır.

Ekran Standartları için Tıklayınız.

- Yeni bir banka tanımlamak için **Ekle**  butonuna tıklanılır.
- Açılan sayfadaki form doldurulur.

|Alan Adı|Açıklama|
|--|--|
|Banka Adı |Sisteminizde kullanacağınız banka isimlerinin girildiği alandır.|
|Para Birimi |Para biriminin tanımlandığı alandır.	|
|Havale Hesap No |Havale yapılacak alışverişlerde kullanılacak girilen bankaya ait olan havale hesap numarası girildiği alandır. <br> ❗ _Havale hesap nosu dolu olan bankalar havale ile ödemede banka olarak çıkacaktır. Eğer ilgili banka ile sadece kredi kartı ile alışveriş kabul edilecekse bu alan boş bırakılmalıdır._|
|Hesap No (Fatura için) |Faturalarda çıkacak olan havale numarasının girildiği alandır.|
|İlgili Kişi |Bankalarda işlemlerle ilgilenen kişinin adı girilir. Hatırlama amaçlı kullanılan bir alandır.	|
|İlgili Kişi Telefon |İlgili kişinin telefon numarası girilir.|
|IBAN|Yurt içi rara transferi işlemlerinde kullanılan hesap numarasıdır.	|
|Swift Kodu|Yurt dışı bankaları için girilmesi gerekli olan banka kodudur.|
|Adres|Kişi adres bilgisinin girildiği alandır.|
|Not||
|Onay|Bankanın aktif olarak kullanılabilmesi için kutucuk işaretlenir.|
|Default Banka|Tanımlanan bankanın sistemde varsayılan banka olarak kullanılması için bu kutucuk işaretlenir. <br> ❗ _Diğer Banka Kartları seçeneği ile yapılan siparişlerin işlemi default olarak tanımlanan bankadan yapılacaktır._|
|Tek Çekimi Kendinden Çek|Eğer BIN numarası tanındıysa tek çekimi default bankadan değilde kendi bankasından çekecektir.|
|Entegrasyon Kodu|Kampanyanın ticari sistemdeki karşılığıdır. Sipariş ve fatura entegrasyonu sırasında ihtiyaca göre kampanyaya giren siparişlerde bu kodun entegrasyon ile gönderilmesini sağlar.|
|Sıra|Taksit seçeneklerinde ve kredi kartı alışverişlerinde bankanın müşteriye hangi sıra ile gösterileceğinin girildiği alandır.|

Gerekli bilgiler girildikten sonra **Kaydet** butonuna tıklanarak banka kayit işlemi tamamlanır.


>❗ _Kredi Kartı POS işlemi sonrasında bankadan dönen hata mesajları sistem tarafından yorumlanıp önuyüz kullanıcısına anlaşılır bir şekilde iletilir. Banka hata mesajlarının ve yorumlanmuş karşılık metinlerinin görüntülenmesi için sağ üst köşedeki Hata Mesajları butonuna tıklanmalıdır._

####**Taksit tanımı:**

- Banka kayıt işlemi tamamlandıktan sonra **TAKSIT TANIMI** bölümündeki  **Ekle** butonuna tıklanılır.
- Açılan sayfadaki form doldurulur.

|Alan Adı|Açıklama|
|--|--|
|Taksit Sayıs|Uygulanacak taksit sayısı girilir. <br>❗ _Bu alana **1 Taksit** olarak tanımlanan değer önyüzde **Peşin** olarak görüntülenecektir. 1 Taksit tanımlanmazsa önyüzde peşin satış yapılamaz._|
|Fiyat Tipi|Girilen taksit sayısı için belirlenen konisyon oranlarının hangi fiyat tipinde geçerli olacağının seçildiği alandır. Bu alan boş bırakılırsa oranlar tüm fiyat tipleri için geçerli olur.|
|% Faiz Banka|Bankanın siteye uygulayacağı faiz oranının girildiği alandır.|
|% Faiz Biz|Sitenin üyeye uygulayacağı komisyon oranının girildiği alandır.|
|% Faiz Biz 2|Sepet toplamı belli bir rakamı geçtiği zaman müşteriye uygulanan komisyon oranının girildiği alandır.|
|Sepet Toplam|Faiz 2 oranı hangi toplamda devreye gireceğinin belirlendiği alandır.|
|Entegrasyon Kodu|Kampanyanın ticari sistemdeki karşılığıdır. Sipariş ve fatura entegrasyonu sırasında ihtiyaca göre kampanyaya giren siparişlerde bu kodun entegrasyon ile gönderilmesini sağlar.|
|Not||

- Gerekli bilgiler girildikten sonra  **Kaydet**  butonuna tıklanarak  kayıt işlemi tamamlanır.
- Diğer taksit seçenekleri de aynı şekilde tanımlanır.

####Sanal Pos bilgilerinin Tanımlanması:

Taksit tanımının sağ tarafındaki alanlar bankadan alınan bilgilerle doldurulur.

>❗ _Sitede kredi kartı ile alışveriş yapılabilmesi için bankadan alınan **Sanal POS kullanıcı bilgileri** ilgili banka kaydına girilmelir.
Sanal pos bilgileri için sistem her banka için o bankaya özel bilgilerin doldurulmasını isteyecektir._

**Örnek :** Aşağıdaki örnekte **Garanti Bankası** için istenen POS Kullanıcı bilgileri yer almaktadır. Farklı banka için farklı bilgiler istenecektir.

|Alan Adı|Açıklama|
|--|--|
|API Kullanıcı Adı|Bankanın verdiği Sanal POS kullanıcı adının girildiği alandır.|
|Şifre|Bankanın  verdiği şifrenin girildiği alandır.|
|Üye İşyeri ID|Bankanın verdiği müşteri numarasının girildiği alandır.|
|Terminal ID	|Bankanın verdiği POS numarasının girildiği alandır.|
|Store Key	|3D Security kullanımı için bankanın verdiği anahtar bilgisinin girildiği alandır.|

Gerekli bilgiler girildikten sonra **Kaydet** butonuna tıklanır.