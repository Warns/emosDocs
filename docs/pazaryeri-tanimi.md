---
id: pazaryeri-tanimi
title: Pazaryeri Tanımı
---

e-MOS sistemi üzerinde tanımlı olan ve satılabilen ürünlerin herhangi bir aracı entegratör firmaya ihtiyaç olmadan pazaryerlerine gönderilebilmesini ve pazaryerlerinde oluşan siparişlerin e-MOS sistemine aktarılarak sipariş sürecinin e-MOS üzerinde yönetilebilmesini sağlar.

## 1. Pazaryeri Tanım Ekranı
Pazar yeri ekleme sayfasında 4 farklı sekme yer almaktadır. Bu sekmeler ve açıklamaları aşağıdaki gibidir;

### 1.1. Genel Bilgiler
Pazaryeri için kullanılacak fiyat tipi, ödeme tipi, nakliye şekli, entegrasyon bağlantı bilgileri (api key, api secret v.s.) temel bilgilerinin yer aldığı alandır. Hangi pazaryeri için hangi alanın doldurulacağı pazaryeri seçimi yapıldıktan sonra otomatik olarak aktif olur.

|Alan Adı|Açıklama|
|--|--|
|Pazaryeri|Hangi pazaryeri için konfigürasyon yapılacaksa o pazaryerinin seçildiği alandır.|
|Fiyat Tipi|Pazar yerinden sipariş çekildiğinde hangi fiyat tipinde e-MOS sistemine aktarılacağının ve ürün bildiriminde ürün fiyatlarının hangi fiyat tipine göre alınıp pazar yerine aktarılacağının belirtildiği alandır.  Pazaryeri özelinde  bir fiyat üzerinden satış yapılması isteniyorsa burada girilecek fiyat tipi değer önem arz etmektedir.<br><br>**Örnek:** Kargo ücreti dahil fiyat ile satılması veya ürününü ilgili pazaryeri için %10 indirimli satılması gibi senaryolar fiyat tipi konfigürasyonuna göre belirlenebilir.<br><br>Fiyat tipi hakkında ayrıntılı bilgi almak için [Tıklayın](fiyat-tipi-tanimi.md)|
|Ödeme Tipi|Pazaryerinden gelen siparişin ödeme tipinin belirlendiği alandır. Burada belirtilen ödeme tipine göre sipariş e-MOS sistemine aktarılacaktır.|
|Nakliye Şekli|Pazaryerinden gelen siparişin nakliye şeklinin belirlendiği alandır. Burada belirtilen nakliye şekline göre sipariş e-MOS sistemine aktarılacaktır.|
|Depo|Pazaryerinden gelen siparişin depo bilgisinin belirlendiği alandır. Burada belirtilen depo bilgisine göre sipariş e-MOS sistemine aktarılacaktır.|
|Pazaryeri Kargo|Müşterinin anlaşmalı kargo bilgisinin girildiği alandır. Buradaki kargo bilgisine göre ürünler pazaryerinde açılacaktır. Bu alan her pazarı yeri için doldurulmak zorun değildir.|
|Kargo Şubesi|Müşterinin anlaşmalı kargo şubesinin girildiği alandır. Buradaki kargo şubesine göre ürünler pazaryerinde açılacaktır. Bu alan her pazarı yeri için doldurulmak zorun değildir.|
|Yayın Süresi|Gönderilen ürünlerin pazaryerinde ne kadar süreyle listeleneceğinin belirtildiği alandır. Buraya rastgele bir değer girilememektedir. İlgili pazaryerinin yayın süre aralığı temin edilip müşteriyle anlaşmalı olan yayın süresi girilmelidir. Bu alan her pazarı yeri için doldurulmak zorun değildir.|
|Kullanıcı|Pazaryeri tarafından, pazaryerine entegre olacak firmaya verilen kullanıcı bilgisinin girildiği alandır. Bu alan her pazarı yeri için doldurulmak zorun değildir.|
|Şifre|Pazaryeri tarafından, pazaryerine entegre olacak firmaya verilen şifre bilgisinin girildiği alandır. Bu alan her pazarı yeri için doldurulmak zorun değildir.|
|Tedarikçi Kodu|Pazaryeri tarafından, pazaryerine entegre olacak firmaya tekil id bilgisinin girildiği alandır. Bu alan her pazarı yeri için doldurulmak zorun değildir.|
|API Key|Pazaryeri tarafından, pazaryerine entegre olacak firmaya verilen api key bilgisinin girildiği alandır. Bu alan her pazarı yeri için doldurulmak zorun değildir.|
|API Secret|Pazaryeri tarafından, pazaryerine entegre olacak firmaya verilen api secret bilgisinin girildiği alandır. Bu alan her pazarı yeri için doldurulmak zorun değildir.|
|Şablon Adı|Pazaryerinde öncelikle bir şablon oluşturup ürünleri bu şablon altında aktarılması gerekebiliyor. Bu şablon bilgisinin girildiği alanı temsil etmektedir.|
|Öndeğer Tes.Süresi|Pazaryerine gönderilen ürünün teslimat süresinin belirtildiği alandır.|
|Marketplace ID|Amazonda mevcut pazar (Örneğin: amazon.com.tr)|
|Authorization Token|Belirli bir Amazon satıcısının belirli bir uygulama geliştiricisine ait yetkiyi temsil eder. Sadece web uygulamaları ve 3rd party geliştirici yetkilendirmelerinde kullanılır.|
|Onay|Pazaryeri tanımının durumunu gösteren alandır. Aktif etmek için işaretlenmesi gerekir.|
|Yalnız Ana Resim Ver|Pazaryerine ürün görselini bildirirken sadece ana görseli bildirmek için kullanılır.|
|Kendi Kargo Kodumu Kullanacağım|Pazaryerinin anlaşmalı olduğu kargo anlaşması üzerinden değil, müşterilerimizin kendi kargo anlaşması üzerinden ilerlemek istemesi durumunda bu özellik aktif edilir. Böylece pazaryerinden sipariş ile birlikte bir kargo kodu e-MOS'a alınmayarak, e-MOS'ta kargo kodu oluşturulur.|
|Barkod Kırılımlı Çalışsın|Barkod bazında bildirim yapılabilen pazaryerlerinde bedenli/seçenekli ürün bildirimi yapılırsa kullanılır.  (Hepsiburada, Morhipo, Trendyol)|
|HepsiExpress Aktif Mi|Sadece Hepsiburada pazaryeri için geçerlidir. Kargo olarak HepsiExpress'i aktif etmek için kullanılır.|

<br>
### 1.2. Ürün
Pazaryerine belli başlı markalara ait ürünlerin, kategorilere ait ürünler gönderilmesi istenebilir. Bu ürün filtre ihtiyacı duyulduğunda bu sekmede ilgili tanımlar yapılarak istek karşılanabilir.

|Alan Adı|Açıklama|
|--|--|
|Markalar (Dahil/Hariç)|Pazaryerine gönderilmesi veya gönderilmemesi istenen markaların seçildiği alandır. Sistem seçilen markaların gönderip göndermeme kararını markalar seçimin hemen sağ tarafında yer alan “Dahil/Hariç” seçimine göre karar vermektedir.|
|Kategoriler (Dahil/Hariç)|Pazaryerine gönderilmesi veya gönderilmemesi istenen kategorilerin seçildiği alandır. Sistem seçilen kategorilerin gönderip göndermeme kararını kategoriler seçimin hemen sağ tarafında yer alan “Dahil/Hariç” seçimine göre karar vermektedir.|
|Min. Stok Miktarı|Ürünün mevcut stoğundan ne kadar düşülerek pazaryerine gönderileceği bilgisinin girildiği alandır.<br><br>**Örnek:** X ürünün 5 adet stoğu mevcut. Bu alana da 2 değeri girildi. Pazaryeri görevi çalıştığında X ürünü için 3 adet stok bilgisi gönderilecektir.|
|Max. Stok Miktarı|Ürünün mevcut stoğundan pazaryerine maksimum gönderilecek stoğunu belirler.<br><br>**Örnek:**X ürünün 10 stoğu mevcut ve maximum stok alanına 5 girildi. Eğer stok 5'ten büyükse 5 gönderir değilse o anki stoğu gönderecek şeklinde kontrol işlemi yapılır.|
|Stok Dağıtım Oranı|Toplam stoğun pazaryerine gönderilecek stok oranının bilgisini belirler.|

<br>
### 1.3. Marka Eşleme
Pazaryeri bazında markalar servisten çekilerek e-MOS sistemine işlenmektedir. e-MOS sisteminde yer alan mevcut markalar ile pazar yerinde yer alan markalar eşleştirilerek ürünün pazaryerine aktarılması sağlanmaktadır.

**Marka Eşleştir Butonu:** e-MOS sisteminde yer alan marka ile pazar yerinden çekilen marka isim olarak birbiriyle aynıysa marka eşleştir butonuna basılarak hızlı bir eşleme işlemi yapılabilmesi sağlanmaktadır.

Yeni bir marka ve pazaryerindeki karşılığını eklemek için **Ekle** butonu kullanılır. Ekle butonuna tıkladıktan sonra aşağıdaki gibi yeni bir sayfa açılır;

![](https://snipboard.io/2VScJP.jpg)

|Alan Adı|Açıklama|
|--|--|
|Marka|e-MOS sisteminde yer alan markaların seçildiği alandır.|
|Karşılık Marka|Pazar yerinden çekilen markaların seçildiği alandır.|
|Onay|Marka eşlemesinin durumunun belirtildiği alandır.|

<br>
### 1.4. Kategori Eşleme
Pazaryeri bazında kategoriler servisten çekilerek e-MOS sistemine işlenmektedir. e-MOS sisteminde yer alan mevcut kategoriler ile pazaryerinde yer alan kategoriler eşleştirilerek ürünün pazar yerine aktarılması sağlanmaktadır.

Yeni bir kategori ve pazaryerindeki karşılığını eklemek için **Ekle** butonu kullanılır. Ekle butonuna tıkladıktan sonra aşağıdaki gibi yeni bir sayfa açılır;

![](https://snipboard.io/Lu4oBM.jpg)

|Alan Adı|Açıklama|
|--|--|
|Kategori|e-MOS sisteminde yer alan kategorilerin seçildiği alandır.|
|Karşılık Kategori|Pazaryerinden çekilen kategorilerin seçildiği alandır.|
|Kategori Tipi|Amazon kategori tipi yapısına özel bir alandır.|
|Onay|Kategori eşlemesinin durumunun belirtildiği alandır.|

> ❗️ _Burda dikkat edilmesi gereken nokta eşlemelerin ürünlerin default kategorisi üzerinden yapılmasıdır. e-MOS'ta ürün birden fazla kategoriye bağlı olabilir ancak default kategorisi bir tanedir. Örnek: Default kategorisi Mineraller olan ürünlerin, pazaryerinde karşılık kategorisi Besin Takviyesidir. Eşlemesi yapılan kategorilere bağlı olarak ürün özellikleri değişmektedir, bu sebeple yapılan eşlemeler çok önemlidir._

<br>
## 2. Pazaryeri İçin Ürünün Aktif Edilmesi ve Özelliklerinin Girilmesi

### 2.1 Pazaryeri İçin Ürünün Aktif Edilmesi
Pazaryeri modülü aktif edildiğinde ürün kartında “Pazaryeri” sekmesi aktif olacaktır. Oluştur butonuna basıldığında sistemde bulunan tüm pazaryerleri için pasif durumda kayıt atılır. Ürün için istenilen pazaryeri aktif edilir. Ürün bildirim görevi çalıştığında ilgili ürün pazaryerine gönderilecek ürünler listesine eklenecektir.

![](https://snipboard.io/ThnLSr.jpg)

<br>
### 2.2 Pazaryeri İçin Ürün Özelliklerinin Girilmesi
N11 ve Gittigidiyor pazaryerleri için ürün bildirimi yapılmak istenildiğinde sadece yukarıdaki tanımlamaları yapmak yeterli olmamaktadır. Kategori bazında ürünler zorunlu girilmesi gereken attributeleri bulunmaktadır. İlgili pazaryeri için zorunlu attributeler aşağıdaki şekilde tanımlanır.

#### 2.2.1 Özellik Seti Tanımı
[Özellik Seti](ozellik-seti.md) sayfasından her bir pazaryeri için onaysız durumunda özellik grubu tanımlanır. 

#### 2.2.2 Özellik Parametre Tanımı
[Özellik Parametre](ozellik-parametre.md) syfasından tanımlanan özellik gruplarına istenilen özellik parametrelerin tanımı yapılır. Kategori bazında zorunlu attribute bilgisi ilgili pazaryerine ait servis ve dokümantasyon üzerinden elde edilir.

![](https://snipboard.io/V1jvhm.jpg)

#### 2.2.3 Ürün Kartında Parametre Seçimi
Ürün kartında “Özellikler” sekmesinde parametre tanımlamaları görünür. İlgili ürünün, ilgili pazar yeri için hangi özelliklerinin seçilmesi gerektiği ürünün kategorisinin hangi pazaryeri kategorisiyle eşleştirmesine bağlıdır.

**Örnek:** X ürünü A kategorisine bağlı, kategori eşleme ekranında da A kategorisi B kategorisiyle eşleştirildi. (A ⇔ B) ürün pazaryerine bildirilirken B kategorisi olarak bildirileceği için B kategorisinin sahip olduğu tüm zorunlu attribute alanlarının doldurulması gerekir.

> ❗️ _Ürün özelliklerinin eksik veya hatalı girildiği durumlarda ilgili ürünün pazaryerine aktarılmasına engel olacaktır. Pazaryerinin servisine bağlı olarak eğer bununla ilgil log tutuyorsa [Pazaryeri Log](pazaryeri-log.md) ekranında aktarılmadığının bilgisi ve nedeni görünecektir._

<br>
### 2.3 Ürün Maliyet Kontrolü
Pazaryerine gönderilecek ürün maliyetinin altında satılmasını engellemek için ürün kartında bulunan maliyet alanı kullanılır. Bu alan admin kullanıcısı tarafından manuel olarak doldurulmaktadır. Ürünün pazaryerine gönderilecek satış fiyatı, maliyet fiyatının altında olması durumunda sistem ürünü göndermeyecek ve pazaryeri log ekranında bu ürünle ilgili uyarı mesajı listeleyecektir.