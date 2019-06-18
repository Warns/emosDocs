Ürünlerin yurt içinde veya yurt dışında satışı için ödeme tiplerinin tanımlanacağı sayfadır.

**Arama :Ödeme Tipi** Adı kriteri üzerinden **ARA** butonuna tıklanarak arama işlemi gerçekleştirilir.

Ekran standartları için Tıklayınız.

- Yeni bir ödeme tipi tanımlamak için **Ekle**  butonuna tıklanılır.
- Açılan sayfadaki form doldurulur.

|Alan Adı|Açıklama|
|--|--|
|Ödeme Tip Adı|Eklenmek istenen ödeme tipi adının girildiği alandır.|
|Ödeme Tipi|Sistemde tanıtılan ödeme tiplerinden birinin seçildiği alandır.|
|Entegrasyon Kodu|Kampanyanın ticari sistemdeki karşılığıdır. Sipariş ve fatura entegrasyonu sırasında ihtiyaca göre kampanyaya giren siparişlerde bu kodun entegrasyon ile gönderilmesini sağlar.|
|Tek Ödeme||
|Onay|Ödeme tipinin geçerli olması için bu kutucuğun işaretli olması gerekir.|
|Açıklama||

**Vade Bilgileri :** Yukarıda belirtilen formu doldurduktan sonra **Ekle** butonuna tıkladığınızda açılan form vade bilgilerinin tanımlanması için doldurulur

|Alan Adı|Açıklama|
|--|--|
|Ödeme Gün|Ödenecek gün sayının girildiği alandır.|
|Ödeme Oranı%|Ödeme oranının % cinsinden yazıldığı alandır.|


Gerekli bilgileri doldurulduktan sonra **Kaydet** butonuna tıklanarak fiyat tipi tanım işlemi tamamlanır.

####PayPal Nedir?

PayPal, internet üzerinden çalışan online bir ödeme sistemidir. 
PayPal, hassas finansal bilgilerinizi online alışveriş siteleri ile paylaşmadan hızlı ve çok daha güvenli ödeme yapma şeklidir. PayPal’da, kredi kartı ve banka hesap bilgileri, kritik finansal bilgilerinizin güvenliğine çok önem verilmektedir.
e-MOS sisteminde iki şekilde paypal ödemesi alınabilmektedir. Bunlar “Express Checkout” ve “Referance Transaction”.

####Express Checkout

Üye e-MOS sisteminde ödeme şekli olarak PayPal’ı seçtikten sonra, sipariş onayı ile birlikte otomatik olarak PayPal sistemine yönlendirme yapılır. Bu sayfada kişi kendi PayPal kullanıcısı ile PayPal’a giriş yaparak, istediği ödeme şeklini belirler ve ödemeyi tamamlar. Sonrasında üye tekrar e-MOS tarafına yönlendirilir. Ödemenin başarılı ya da başarısız olmasına göre sipariş süreci olumlu / olumsuz olarak sonuçlanır.

 

####Referance Transaction

Temelde Express Checkout yapısı kullanılmaktadır. Farkı, müşteri PayPal ile ilgili sitede başarılı bir sipariş verdikten sonra referans bilgisi e-MOS da kaydedilir. Ve aynı müşterinin sonraki alışverişlerinde e-MOS daki ödeme adımında bir önceki ödeme şekli ile aynen ödeme alma işlemi yapılmak istenip istenmediği sorulacak, bu checkbox işaretli bırakılırsa sipariş onayından sonra PayPal sitesine yönlendirme yapılmadan ödeme alınacak ve sipariş sonuçlandırılacaktır. Checkbox işaretli olmadığı durumda ise üye Siparişi onayladığında Express Checkout süreci aynen çalışacaktır.

####Paypal Ödeme Tipi Tanımlama

“Tanımlar > Ödeme Tipi Tanımı”  kısmından  ‘PayPal’   adında bir Ödeme Tipi tanımlanması gerekmektedir. 
Site ayarları > Entegrasyon Ayarları > PayPal Account kısmı (PayPal için kullanılacak olan “APIUsername, APIPassword  ve APISignature”)  bilgileri virgül ile ayırarak müşteri tarafından doldurulması gereken kısımdır.

