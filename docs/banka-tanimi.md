---
id: banka-tanimi
title: Banka Tanımı
---

## 1. Banka Tanımı

Üyelerin önyüzden alışveriş yapmak için kullanacakları bankaların tanımlandığı ekrandır.

Yeni bir banka tanımlamak için **Ekle**  butonuna tıklanılır. Açılan sayfadaki alanlarla ilgili detaylar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Banka Adı|Sitenizde kullanacağınız banka isminin girildiği alandır.|
|Para Birimi |Para biriminin tanımlandığı alandır.|
|Fiyat Tipi|Banka tanımının hangi fiyat tipinde geçerli olacağının seçildiği alandır. Bu alan boş bırakılırsa ilgili banka tüm fiyat tipleri için geçerli olacaktır.|
|Havale Hesap No|Havale yapılacak alışverişlerde kullanılacak girilen bankaya ait olan havale hesap numarası girildiği alandır. <br> ❗ _Havale hesap numarası dolu olan bankalar havale ile ödemede banka olarak çıkacaktır. Eğer ilgili banka ile sadece kredi kartı ile alışveriş kabul edilecekse bu alan boş bırakılmalıdır._|
|Hesap No (Fatura için)|Faturalarda çıkacak olan havale numarasının girildiği alandır.|
|Yetkili|Banka işlemlerinde ilgilenen kişinin adı girilir. Hatırlama amaçlı kullanılan bir alandır.|
|Yetkili Telefon|Yetkili kişinin telefon numarası.|
|IBAN|Yurt içi para transferi işlemlerinde kullanılan hesap numarasıdır.|
|Swift Kodu|Yurt dışı bankaları için girilmesi gerekli olan banka kodudur.|
|Entegrasyon Kodu|Kampanyanın ticari sistemdeki karşılığıdır. Sipariş ve fatura entegrasyonu sırasında ihtiyaca göre kampanyaya giren siparişlerde bu kodun entegrasyon ile gönderilmesini sağlar.|
|Adres|Kişi adres bilgisinin girildiği alandır.|
|Not|e-MOS panel kullanıcısı tarafından kullanılabilir not alanıdır. Bu alana yazılan yazı önyüzde görünmeyecektir.|
|Kampanya Metni|Banka tarafından ödemelerde bir kampanya sağlanıyorsa, kampanyayla ilgili metin bu alana girilir ve tasarıma bağlı olarak önyüzde gösterilir.|
|Onay|Banka tanımının durumunu belirler. Banka tanımının aktif olması için bu kutucuk işaretli olması gerekir.|
|Default Banka|Tanımlanan bankanın sistemde varsayılan banka olarak kullanılması için bu kutucuk işaretlenir. <br> ❗ _Diğer Banka Kartları seçeneği ile yapılan siparişlerin işlemi bu kutucuğun işaretli olduğu default olarak tanımlanan bankadan yapılacaktır._|
|Tek Çekimi Kendinden Çek|Tek çekim ödemelerde eğer ilgili kartın BIN numarası sistem tarafından tanındıysa tek çekimi default bankadan değil kendi kartın bankasından çekecektir.|
|Banka Puan Kullanımı Aktif|Ödeme işlemlerinde kart bilgileri girildikten sonra banka puanının kullanımına izin verilip verilmemesini belirler. Bu kutucuk işaretli olduğunda ilgili banka tanımına ait kart kullanıldığında hesapta bulunan puan bilgisi gösterilir ve kullanımına izin verilir.|
|CVC'siz İşlem Yetkisi Var Mı?|CVC bilgisi girilmeden işleme devam edilip edilemeyeceğini kontrol eder. Bu kutucuk işaretli olduğunda CVC bilgisi girilmeden ödeme işlemine devam edilebilir.|
|Sıra|Taksit seçeneklerinde ve kredi kartı alışverişlerinde bankanın müşteriye hangi sıra ile gösterileceğinin girildiği alandır.|
|POS Aktif|İlgili bankanın sanal POS kullanımının açık olup olmadığını belirler. Bu kutucuk işaretli olduğunda kredi kartı, banka kartı gibi ödemelerde bankanın sanal POS'u kullanılacaktır.|
|3D Aktif|3D ödemenin aktif olup olmadığını belirler. Bu kutucuk işaretli olduğunda 3D ile ödeme seçeneği de önyüzde gösterilecektir. İsteğe bağlı olarak sadece 3D ile ödeme seçeneğinin çıkması sağlanabilir.|

<br>
### 1.1. Sanal POS Bilgilerinin Tanımlanması

Sitede kredi kartı ile alışveriş yapılabilmesi için bankadan alınan **Sanal POS kullanıcı bilgileri** ilgili banka kaydına girilmesi gerekir.

Kullanıcı bilgileriyle ilgili alanlar ve detayları aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|API Kullanıcı Adı|Bankanın verdiği Sanal POS kullanıcı adının girildiği alandır.|
|Şifre|Bankanın  verdiği şifrenin girildiği alandır.|
|Üye İşyeri ID|Bankanın verdiği müşteri numarasının girildiği alandır.|
|Store Key|3D Security kullanımı için bankanın verdiği anahtar bilgisinin girildiği alandır.|


>❗ _Kredi Kartı POS işlemi sonrasında bankadan dönen hata mesajları sistem tarafından yorumlanıp önuyüz kullanıcısına anlaşılır bir şekilde iletilir. Banka hata mesajlarının ve yorumlanmış karşılık metinlerinin görüntülenmesi için sağ üst köşedeki **Hata Mesajları** butonuna tıklayabilirsiniz._

Tüm bilgileri doldurduktan sonra **Kaydet** butonuna tıklayarak banka tanımı kayıt işlemi tamamlanır. Banka tanımını Kaydettikten sonra bir sonraki bölümde anlatılan Taksit Tanımı kısmı kullanılabilir hale gelir.

### 1.2.Taksit Tanımı

Yeni taksit kaydı eklemek için **Ekle** butonuna tıklanır. Açılan sayfada bulunan alanlarla ilgili detaylar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Taksit Sayıs|Uygulanacak taksit sayısı girilir. <br>❗ _Bu alana **1 Taksit** olarak tanımlanan değer önyüzde **Peşin** olarak görüntülenecektir. 1 Taksit tanımlanmazsa önyüzde peşin satış yapılamaz._|
|Fiyat Tipi|Girilen taksit sayısı için belirlenen komisyon oranlarının hangi fiyat tipinde geçerli olacağının seçildiği alandır. Bu alan boş bırakılırsa oranlar tüm fiyat tipleri için geçerli olur.|
|% Faiz Banka|Bankanın siteye uygulayacağı faiz oranının girildiği alandır.|
|% Faiz Biz|Sitenin üyeye uygulayacağı komisyon oranının girildiği alandır.|
|Sepet Toplam|Faiz 2 oranı hangi toplamda devreye gireceğinin belirlendiği alandır.|
|% Faiz Biz 2|Sepet toplamı belli bir rakamı geçtiği zaman müşteriye uygulanan komisyon oranının girildiği alandır.|
|Banka Ek Taksit|Banka tarafından sağlanan ek taksit varsa bu alana girilir.|
|Not|e-MOS panel kullanıcısı tarafından kullanılabilir not alanıdır. Bu alana yazılan yazı önyüzde görünmeyecektir.|
|Ent. Kodu|Kampanyanın ticari sistemdeki karşılığıdır. Sipariş ve fatura entegrasyonu sırasında ihtiyaca göre kampanyaya giren siparişlerde bu kodun entegrasyon ile gönderilmesini sağlar.|
|Min. Tutar|Taksit seçeneğinin aktif olması için gerekli olan minimum tutarın belirtildiği alandır.|
|Class|Önyüzde frontend ekibi tarafından bir özelleştirme yapılacaksa kullanılacak alandır.|
|Onay|Taksit tanımının durumunu belirleyen alandır. Taksit tanımının aktif olması için bu kutucuğun işaretli olması gerekir.|

Gerekli bilgiler girildikten sonra  **Kaydet**  butonuna tıklayarak  kayıt işlemi tamamlanır.
Diğer taksit seçenekleri de aynı şekilde tanımlanır.

Gerekli tüm bilgiler girildikten sonra banka tanım ekranında **Kaydet** butonuna tıklayarak banka kayıt işlemi tamamlanır.