---
id: urun-tanimi
title: Ürün Tanımı
---

Sistemde kullanılacak olan ürünlerin tanımlandığı sayfadır.

Sayfanın kullanımında gerekli temel bilgilere ulaşmak için [Tıklayınız](ekran-standartlari.md).

![image.png](https://snag.gy/WZqncJ.jpg)

Ürün tanımı sayfasının üst kısmında bulunan filtre alanları ürünlere hızlıca erişim sağlamak için kullanılır. Aynı zamanda Filtre alanlarının alt kısmında bulunan seçeneklerle ürünler üzerinde toplu işlem yapmak için kullanılır. **Örnek:** Filtrelenen ürünleri bir kategoriye eklemek, excel'e aktarmak veya bir ürün tipine bağlamak vs.


Bir ürüne tıklandığında aşağıdaki gibi ürün kartı ekranı açılır; 
![pdct.png](https://snag.gy/AyxwPz.jpg)

<br>
## 1. Sekme (Genel Bilgiler) 

|Alan Adı|Açıklama|Örnek|
|--|--|--|
|Kategori|Ürünün bağlanmak istendiği kategori, ![image.png](https://snag.gy/pnQ7qP.jpg) butonuna tıklanarak seçilir. Bir ürün birden fazla kategoriye bağlanabilir.||
|Marka|Ürünün markasının markalar listesinden seçildiği alandır.||
|Ürün Kodu|Ürün kodunun yazıldığı alandır. Yeni kayıt ekleme sırasında bir ürün kodu girilmezse sistem tarafından otomatik bir kod atanacaktır. Bu ürün kodunun ön ek karakterleri **Site Yönetimi > Temel Ayarlar > Site Ayarları > Ürün Ayarları** sayfasında bulunan **Ürün Kodu Formatı** alanından belirlenebilir.|HS000134 (Burada ön ek karakteri HS olarak belirlendi)|
|Ürün|Ürün isminin girildiği alandır. Girilen isim site bazında tekil olmalıdır.||
|Sayfa Başlık|Tarayıcı sekmesinde görünecek yazıya karşılık gelir.![](https://snag.gy/bm8KC6.jpg)||
|Sayfa İsmi|Bu alana ürünle ilişkili kelimelerden oluşan bir link bilgisi girilebilir. Bu linkin amacı ürün sayfasının arama motorlarında girilen link kelimeleri ile ilgili olarak daha üst sıralarda yer almasını sağlamaktadır.<br><br> ❗️ _Sayfa ismi tanımlanırken karakterlerin arasında boşluk bırakılmamalı, dile özgü karakterler kullanılmamalıdır. Sayfa ismi sistem bazında tekil olmalıdır._ <br>_Eğer ürüne sayfa ismi girilmezse sistem tarafından ürün adını içerecek şekilde otomatik bir sayfa ismi oluşturulur._|[/adidas-performance-the-34-tight.html]()|
|Kısa Açıklama|Bu alana girilen bilgi sitede yayınlanan ürünlerin listelendiği ekranda veya ürün detayda her ürüne ait kısa bir not olarak gösterilebilir.<br><br>![](https://snag.gy/Xhgdcs.jpg)|Kadın Tayt AA0617|
|Editor Notu|Kısa açıklama alanında da olduğu gibi bu alana da yazılan yazı ön yüzde ürün listede ve/veya ürün detayda kısa bir not olarak gösterilebilir.||
|Anahtar Kelimeler|Arama motorları ve site içi aramalarda kullanılmak üzere tanımlanan kelimelerdir.||
|Keyword Rank|Anahtar Kelimeler kısmına girilen anahtar kelimelerin önem seviyesinin belirlendiği alandır||
|Meta Description|Bu alan SEO çalışamaları için kullanılmaktadır. Bu alana yazılan meta descrption arama motorları tarafından okunur ve önyüzde sayfa kaynağında görünür.||
|Ürün Tanımı|Html editörü aracılığıyla ürünün detaylı açıklamasının girildiği alandır. Bu alana girilen bilgiler, sitede ürünün detay bilgilerinin yer aldığı sayfada görüntülenir.||
|Birim|Birim, ürünün stok ve fiyatlandırma noktasında takip edileceği temel birimdir. Yani Temel ölçü birimi adet olan bir ürün için stoklar adet takip edilerek, birim fiyatı adet cinsinden girilmelidir.||
|Satış Katı|Bu alan doldurulduğunda kullanıcıların belirlenen miktarın katları şeklinde sipariş verebilmesini sağlanır.|Satış katı 3 olarak belirlendiğinde kullanıcıların 3,6,9,12... gibi 3 ün katları kadar sipariş vermesine izin verilir.|
|Min.Satış Mik.|Kullanıcıların sipariş verebileceği minimum ürün miktarını belirler.||
|Max.Satış Mik.|Kullanıcıların sipariş verebileceği maksimum ürün miktarını belirler.	||
|Koli Adedi|Koli adedi, bir ürünün koli ile satılması durumunda kolisindeki miktarı belirler. Bu bilgi girildiğinde, ürün detay ekranında Koli adedi ve birim fiyatı sistem tarafından hesaplanarak gösterilecektir.||
|Kap Adedi|Kap adedi, ürünün toplu taşıma yapılırken palet içindeki adedini belirler. Satınalma siparişi oluşturulurken, kap adedi girilmiş olan ürünler için bu adedin katı kadar sipariş açılması önerilecektir.||
|Palet Hacim (En-Boy-Yükseklik)|Ürünün palet hacmi hesabı için en, boy ve yüksekliğinin girildiği alandır.|Bir ürün paletine 8 adet ürün yerleştirilecekse, 8 ürünün toplam en, boy ve yükseklik bilgileri girilmelidir.|
|Brüt Hacim(En-Boy-Yükseklik)|Ürünün brüt hacim hesabı için gerekli olan en, boy ve yüksekliğin girildiği alandır.||
|Net Hacim(En-Boy-Yükseklik)|Ürünün net hacim hesabı için gerekli olan en, boy ve yüksekliğin girildiği alandır.||
|Brüt|Ürünün brüt ağırlığının girildiği alandır.<br><br>❗️ _Zorunlu alan olduğu için önemsiz olduğu durumda 0 girilmelidir._||
|Net|Ürünün net ağırlığının girildiği alandır.||
|Desi|Kargo fiyatlandırması genel bir birim tanımı üzerinden hareket etmektedir. Bu alana ürünle ilgili kargo fiyatlandırma birimi cinsinden miktar girilmelidir. (desi, kg, metreküp).<br><br>Sistemde desi hesabı iki şekilde yapılabilir. Ürünün hacim, ağırlık bilgileri üzerinden sistem desi bilgisini hesaplar veya ürün kartındaki desi bilgisi direkt kullanılır. Desi alanının yanındaki checkbox işaretli olduğunda, girilen desi miktarının aynen kullanılacağı anlamına gelir. İşaretlenmediği durumda ise ürün kartında girilen brüt hacim, brüt ağırlık ve kargo tanımında girilen desi çarpanı kullanılarak hesaplanır. Burada **"brüt hacim/desi çarpanı"** ile **brüt ağırlık** değerlerinden büyük olan ***desi** olarak kabul edilir.||
|Eksik Bilgi|Ürünler tanımlanırken bilgisi eksik kalanların yönetim paneli kullanıcıları tarafından takip edebilmesi amacı ile kullanılır. Eksik bilgi olarak işaretlenmiş ürünler sitede gösterilmez.||
|Takım|Ürünün takım olarak satılıp satılmayacağını belirleyen alandır. Takım kutucuğu işaretlendiğinde **Takımlar** sekmesi açılır. Takım içerisinde yer alacak ürünler ve miktarları belirlenir. Sitedeki satış fiyatı kendisini oluşturan ürünlerin "birim fiyat x adet" toplamından oluştur. Benzer şekilde takım içindeki ürünlerin en az birinde indirim olduğunda takımda indirimli gözükür.||
|Servis Gerektiren Ürün|Ürünün kurulum servisi gerektirip gerektirmediğini belirleyen alandır.
>❗ _Manuel ürün tanımlarken ürünün resimlerini, tavsiye ürünlerini ve bundle ürünlerini girebilmek, promosyon ve sipariş geçmişini izleyebilmek için kullanılacak linkler ancak ürün kaydedildikten sonra görüntülenecektir._

Ürün kaydetme işlemini tamamladıktan sonra genel bilgiler sekmesinde ürünle ilgili linkler bulunur. **(Resimler, Tavsiyeler, Promosyon Geçmişi, Siparişler, Bundle)** Bu linklere tıklayarak ürünle ilgili aşağıdaki işlemler yapılabilir.<br><br>

### a. Resimler
Sisteme yüklenmiş olan veya yeni eklenecek resimlerin ürünlere atandığı bölümdür. Resimler linkine tıklandıktan sonra açılan sayfada ürüne bağlanmak istenen resimler eklenilir. Yeni görsel eklemek için **Ekle** butonuna tıklanır. Açılan sayfada ürüne resim seçebilmek için ![](https://snag.gy/48R0Kc.jpg) butonuna tıklanır.

|Alan Adı|Açıklama|
|--|--|
|Ürün Resim|Seçim butonu ile sisteme yüklü olan resimlerden birininin seçildiği alandır. Eğer seçilecek resim kayıtlı değilse **Dosya Yükleme** butonunu kullanarak sisteme yeni bir resim yüklenebilir. |
|Referans Seçenekler|Ürünün farklı seçeneklerine farklı resimler tanımlamak için kullanılan alandır. Örneğin aynı ürünün kırmızı rengi için bir resim, mavi rengi için farklı bir resim belirlenebilir. Bu durumda sitede müşteri ürünün seçeneğini değiştirdiğinde, ürünün resmi de değişecektir.|
|Dosya Tipi|Bu alandan yeni eklenecek olan dosyanın tipi seçilir.|
|Sıra|Bu alandan yeni eklenecek olan görselin sırası belirtilir. Birden çok görselin olduğu üründe bu alanı kullanarak görsellerin sırası değiştirilebilir.|
|Öndeğer|Bu kutu işaretlendiğinde belirlenen resim önyüzde öncelikli gösterilecek resim olarak belirlenir. Ürün listelerinde, ürün detayında, promosyon ve indirim resimlerinde hep bu resim gösterilecektir.|
|Onay|Resmin geçerli olması için bu kutucuğun işaretli olması gerekir.|
|Ekleme Tarihi|Görsel sisteme eklendikten sonra bu alanda görselin ekleme tarihi yazıyor olacak.|
|Güncelleme Tarihi|Sistemde var olan bir görsel güncellendiğinde bu alanda güncelleme tarihi yazıyor olacak.|
|Not|Sadece yönetim kısmında görülebilen ve bilgi için kullanılan bir alandır.|
|Çoklu Görsel Yükleme Sekmesi|Birden fazla ürün resminin aynı ekrandan seçilebilmesini sağlayan sekmedir.|

Gerekli bilgileri girdikten sonra **Kaydet** butonuna tıklanır ve  resim yükleme işlemi tamamlanır. Sayfadan çıkmadan yeni bir resim yüklenmek isteniyorsa ![](https://snag.gy/W4qmna.jpg) butonuna tıklanır.

> ❗️ _Herhangi bir ürün resimi eklendiğinde sistemde tasarım sırasında belirlenen diğer resim boyutlarını (sepetteki küçük resim, ürün listelerindeki resim, ürün detayındaki resim, vb) kendisi otomatik olarak oluşturacaktır. Otomatik resimler, resim/dosya seçme modülü tarafından ilgili klasöre girildiğinde yapılır._

<br>
### b. Dokümanlar
Sisteme yüklenmiş olan veya yeni eklenecek dokümanların ürünlere atandığı bölümdür. Dokümanlar linkine tıklandıktan sonra açılan sayfada ürüne bağlanmak istenen dokümanlar eklenilir. Yeni doküman eklemek için **Ekle** butonuna tıklanır. Sayfa açıldığında ürüne doküman seçebilmek için ![](https://snag.gy/1L3zat.jpg) butonuna tıklanır.

|Alan Adı|Açıkalam|
|--|--|
|Doküman Adı|Dokümanın isminin girildiği alandır. Buraya girilen bilgi sitede doküman adı olarak görüntülenecektir.|
|Tipi|Dokümanların gruplanmasını sağlayan alandır. (Ör : Kullanım Klavuzu, Teknik Çizim, Ürün Sürücüleri vb.|
|Doküman|Seçim butonu ile sisteme yüklü olan dokümanlardan birininin seçildiği alandır. Eğer seçilecek doküman kayıtlı değilse **Dosya Yükle** butonunu kullanarak sisteme yeni bir doküman yüklenebilir. Dosya Yükleme hakkında ayrıntılı bilgi almak için [Tıklayınız](resim-ve-dosya-yukleme.md).|
|Dosya Boyutu|Dokümanın boyutu biliniyorsa bu alana girilir. Girilen bilgi sitede doküman boyutu olarak görüntülenecektir. (Örnek: 15 MB)|
|Onay|Dokümanın geçerli olması için bu kutucuğun işaretli olması gerekir.|
|Çoklu Doküman Yükleme Sekmesi|Birden fazla ürün dokümanının aynı ekrandan seçilebilmesini sağlayan sekmedir.|

Gerekli bilgileri girdikten sonra **Kaydet** butonuna tıklanır ve  doküman yükleme işlemi tamamlanır. Sayfadan çıkmadan yeni bir doküman yüklenmek isteniyorsa ![](https://snag.gy/W4qmna.jpg)butonuna tıklanır.

<br>
### c. Tavsiyeler
Ürünler ile birlikte satışı tavsiye edilecek diğer ürünlerin belirlendiği bölümdür. Yeni bir ürün tavsiye edebilmek için **Tavsiyeler** butonuna tıklandıktan sonra **Ekle** butonu ile açılan sayfayı doldurmak yeterlidir.

|Alan Adı|Açıklama|
|--|--|
|Tavsiye Ürün|Ürünün yanında tavsiye edilecek ürünün seçildiği alandır. Tavsiye ürünü daha rahat seçebilmek için **Kategori, Ürün Kodu, Ürün adı ve Barkod** alanlarından arama yapılabilmektedir.|
|Grup|Tavsiye ürünleri ayrı ayrı gruplara ayırmak için kullanılır. Aynı zamanda tavsiye ürünleri aynı tek bir grup içerisine dahil ederek isteğe bağlı sıralama yapılabilir.|
|Sıra|Tavsiye edilen ürünlerin gösterildiği alanda ürünün görüntülenmesini istediğiniz sıra numarasını yazabilirsiniz.|
|Onay|Onaylı olan satırlar sitede tavsiye ürün olarak gösterilecektir.|

Gerekli bilgileri doldurduktan sonra **Kaydet** butonuna tıklayarak tavsiye ürün tanımlama işlemini tamamlayabilirsiniz.

**Toplu Tavsiye:** Toplu tavsiye linkine tıklayıp birden çok ürün tek seferde  tavsiye olarak belirlenebilir. Bunun için **Toplu Ürün Tavsiye** sekmesine tıklayarak açılan formu doldurmak yeterlidir.

|Alan Adı|Açıklama|
|--|--|
|Tavsiye Ürün|Tavsiye edilecek ürünlerin toplu olarak seçildiği alandır.|
|Onay|Seçilen ürünlerin sitede gösterilip gösterilmeyeceğini belirleyen kutucuktur.|

<br>
### d. Promosyon Geçmişi
Promosyon Geçmişi linkine tıklanıldığında açılan sayfada ürünle ilgili tanımlanmış tüm indirim ve promosyonlar görüntülenir. Açılan listedeki bir satırın üzerine tıklanıldığı zaman promosyon veya indirimin detay bilgilerine ulaşılır.

<br>
### e. Siparişler
Siparişler linkine tıklanıldığı zaman ürünle ilgili verilmiş tüm siparişler görüntülenir. Açılan listedeki bir siparişin üzerine tıklayarak siparişin detay bilgilerine ulaşılır.

<br>
### f. Bundle
Ana ürünlerle birlikte sunulması istenen yan ürünlerin belirlendiği bölümdür. e-MOS'ta bundle ürünler aynı zamnda birer ürün olarak tanımlanır, bundle ürün tek başına da bir ürün olarak satılabilir. Bundle yapısında bundle ürünü ana ürün ile birlikte satın alındığında normal fiyatından indirimli olarak satılabılır. **Örnek:** X cep telefonuyla birlikte bundle olarak cep telefonu kılıfı satın alındığında 20TL yerine 15TL.

Ürüne yeni bir bundle ürün bağlamak için için **Bundle** butonuna tıklandıktan sonra **Ekle** butonu ile açılan sayfayı doldurmak yeterlidir.

|Alan Adı|Açıklama|
|--|--|
|Bağlı Ürün|Bağlamak istenen bundle ürün bu alanı kullanarak seçilir.|
|Fiyat Tipi|Bu alanı kullanarak sadece belli bir fiyat tipine bağlı olan kullanıcıların bundle ürünleri görmesi sağlanabilir.|
|Adet|Seçilen bundle ürün adedinin belirlendiği alandır.|
|Satış Fiyatı (KDV'siz)|Bu alana girilen fiyat bundle ürününün satış fiyatı haline gelir. Bundle ürünün kendi fiyatından daha indirimli bir fiyat belirlenmek istendiğinde bu alan kullanılır.|Başlangıç Tarihi|Bundle ürününün devreye gireceği tarihin belirlendiği alandır.|
|Bitiş Tarihi|Bundle ürününün devreden çıkacağı tarihin belirlendiği alandır.|
|Grup|Bundle ürünleri ayrı ayrı gruplara ayırmak için kullanılır. Aynı zamanda bundle ürünleri aynı tek bir grup içerisine dahil ederek isteğe bağlı sıralama yapılabilir.|
|Sıra|Bundle ürünlerin gösterildiği alanda ürünün görüntülenmesini istediğiniz sıra numarasının belirlendiği alandır.|
|Ent.Kodu|Bundle ürünler bir ERP sisteminden besleniyorsa ilgili entegrasyon kodunun girildiği alandır.|
|Class|Front-end ekibi tarafından bundle ürünler arasında tasarımsal farklılık oluşturulması için kullanılan sitil bilgisi bu alana girilir.|
|Öndeğer Şekil|**Seçimli:** Bu seçenek kullanıldığında bundle ürünler checkbox yapısı gibi seçmeli olarak sunulur.<br>**Öndeğer:** Bu seçenek kullanıldığında öndeğer olarak ilgili bundle ürün seçili olarak gelir.<br>**Takım:** Bu alan, zorunlu olarak birlikte alınacak ana ürün ve bundle ürün yapısı için kullanılır. Bundle ürünün fiyatı ana ürünün fiyatına eklenir ve toplu olarka tek fiyat gösterilir.|
|Onay|Bundle ürününün aktif olması (önyüzde görünmesi) için bu alanın seçili olması gerekir.|
|Ana Ürün Tek Alınabilir|Bu alan seçili olduğunda bundle ürün zorunluluğu ortadan kalkar ve ilgili ana ürün tek olarak satın alınabilir hale gelir.|

Gerekli bilgileri doldurduktan sonra **Kaydet** butonuna tıklayarak bundle ürün tanımlama işlemini tamamlayabilirsiniz.

<br>
## 2. Sekme (Ürün Yönetim)
Ürünle ilgili yönetimsel düzenlemelerin yapıldığı ekrandır. Bu ekranının içeriği, **Tanımlar > Ürün Tanımı > Ürün Yönetimi** güncelleme ekranı ile aynıdır.

|Alan Adı|Açıklama|Örnek|
|--|--|--|
|Ürün|Ürünün ilk sekmede girilen adının bilgi olarak gösterildiği alandır.||
|Stok Durumu|Ürünün stoktaki durumunun belirlendiği alandır. Sitede ürün stok durumu ile ilgili ikon bilgisi gösterilecektir. Temin edilebiliyor ve Temin edilemiyor durumlarının bir ikon karşılığı yoktur. Temin edilemiyor olarak belirlenen bir ürün için **Sepete Ekle** yerine **Gelince Haber Ver** seçeneği oluşacaktır.|Temin Edilebiliyor, Aynı Gün Kargo, Stoklarla Sınırlı, Sipariş Üzerine Temin vb.|
|Ana Tedarikçi|Ürünün tedarikçi bilgisinin belirlendiği alandır.||
|Satış Vergi Tipi|Satış vergi oranlarının bazı ülkelerde ülke, il ve posta kodları bazında farklılık gösterebilmesinden dolayı ürün kartında satış vergi tipi tanımlanmaktadır. Tanımlanan tipe ait vergi oranları Tanımlar menüsü altındaki vergi tanımları ekranından belirlenebilir.||
|Alış Vergi Oranı|Ürün alışındaki vergi oranının tanımlamasının yapıldığı alandır.||
|Min Adet|Ürünlerin minimum stoklama miktarı, temel ölçü birimi cinsinden girilebilir. Satınalma siparişi açılması sırasında, sistem öngörü olarak minimum sipariş adetlerini de göz önünde bulundurarak tavisyede bulunacaktır.||
|Max Adet|Ürünlerin maksimum stoklama miktarı, temel ölçü birimi cinsinden girilebilir. Satınalma siparişi açılması sırasında, sistem öngörü olarak maksimum miktara tamamlayacak şekilde göz önünde bulundurarak tavisyede bulunacaktır.||
|Para Birimi|Ürünlerin listelendiği kısımlarda ve ürün detay bölümünde bilgi olarak gösterilecek para birimidir. Ürün detay kısmında ve sepet sonrası tüm ekranlarda ürün fiyatları sitenin resmi para birimine dönecektir.||
|Özellikli Ürün|Bu alanda bulunan seçenekler **Tanımlar > Diğer > Diğer Tanımlar** ekranından tanımlanır. Ürünlerle ilgili varsa özel bir durum bu alanı kullanarak belirlenir.||
|Maliyet|Bu alan Pazaryeri modülüne özel olup ürünün pazaryerinde minimum satış fiyatını belirler.|Bu alana 100 girildiğinde ürün fiyatı pazaryerinde herhangi bir indirimden dolayı 100TL'nin altına düştüğünde ilgili ürün pazaryerinde satışa kapatılır.|
|Ürün Tipi|Bu alanda bulunana seçenekler **Tanımlar > Diğer > Diğer Tanımlar** ekranından tanımlanır. Ürün tipini kullanarak ürünleri gruplayabilir ve farklı yapılarda kullanılabilir.|Belli bir ürün tipine bağlı ürün grubunu bir kampanyaya bağlayabilir veya önyüzde ayrı bir sayfa haline getirerek ilgili ürün tipine bağlı ürünler listelenebilir. **Örnek:** Anneler Gününe Özel sayfası.|
|Adres Tipi|Öndeğer olarak bu alan **Bireysel** olarak çalışır. **Kurumsal** seçeneği ise adres seçerken ikinci bir adres tipi olarak son kullanıcıya sunulur. ||
|Platform|Bu alanı kullanarak ilgili ürünün satışı istenen platforma göre kısıtlanabilir. Herhangi bir seçim yapılmadığında ilgili ürün tüm platformlarda satışa sunulur.||
|Onay|Ürünün aktif olması için (önyüzde görünmesi) için bu alanın seçili olması gerekir.<br><br>❗️ _Onay'ı olmayan herhangi bir ürün önyüzde görünmez._||
|Stoklu|Ürünün stoklu veya stoksuz olarak satılabilme durumunun belirlendiği alandır.<br><br> Bu seçenek işaretlenmiş olan ürünler stokta yoksa sistem ürünün satışına izin vermez. Stoklu olarak işaretlenmemiş olan ürünlerde stokta olsun veya olmasın satışa izin verilir.<br><br> Stoklu olarak işaretlenmiş bir ürün için ancak stoktaki miktar kadar sipariş alınmasına izin verilir. Örneğin stokta 5 adet varsa ve önyüzde müşteri 6 adet sipariş vermek isterse sepette uyarı verilerek ancak 5 adet sipariş verilebileceği belirtilir.<br><br> ❗️ _Ürünün stok durumu "Temin Edilemiyor" olarak seçildiğinde stokta varsa bile satışına izin verilmez._||
|Yeni Ürün|Ürünün sitede "yeni ürünler" kısmında görünmesi için bu kutucuğun işaretlenmesi gereklidir. Aynı zamanda bu alan ürünler üzerinde Yeni ikonunun görünmesini sağlamak için kullanılır.||
|Öne Çıkan Ürün|Bu alan, belli bir ürün grubunu ana sayfada göstermek için kullanılır. Front-end ekibi bu gösterimi sağlamak için bu alanı kullanır. Bu alanın seçili olduğu ürünler önyüzde ilgili alanda gösterilir.||
|Ürün Listede Gösterilmesin|Bu alan, kategori sayfalarında (ürün liste sayfalarında) herhangi bir ürünün görünmemesini sağlamak için kullanılır.||
|Site İçi Arama Sonuçlarında Gösterilmesin|Bu kutucuk işaretli olduğu zaman ilgli ürün site içi yapılan aramalarda çıkmayacaktır.||
|Max. Taksit Sayısı|Bu alanı kullanarak ilgili ürünün dahil olabileceği maksimum taksit sayısı belirlenebilir.||
|Mağazadan Teslim Ürünü|Bu alan, mağazalardan teslimat sürecinin bulunduğu firmalarda kullanılır. Bu kutucuğun işaretli olduğu ürünler mağazadan teslim sürecine dahil edilir.||
|Ana Sayfada Gösterilsin|Bu alan, belli bir ürün grubunu ana sayfada göstermek için kullanılır. Front-end ekibi bu gösterimi sağlamak için bu alanı kullanır. Bu alanın seçili olduğu ürünler önyüzde ilgili alanda gösterilir.||
|Kritik Seviyede Uyar|Ürünün stok miktarı minimum adet kutusunda girilen değerin altına düştüğü anda admine uyarı maili atılması için bu alanın işaretlenmesi gerekir.||
|Ürün Detaya Gidilmesin|Eğer bu ürün sadece liste sayfalarında görünsün, detay bilgileri görünmesin isteniyorsa bu kutucuk işaretlenir.||
|Ürün Tek Satılmaz|Bir ürünün tek başına sepete atılması istenmiyorsa, bu durumu önlemek için bu alanın işaretlenmesi gerekir. Bu seçenek işaretlendiğide, eğer ürün herhangi bir kampanya kapsamında değil ise sepette tutulmaz.||
|API'den Stok ve Fiyat Güncellenebilir|Bu alan, API servisi üzerinden e-MOS'ta bulunan ürünlerin stok ve fiyat bilgisini güncellemek için kullanılır. Bu kutucuğun seçili olduğu ürünlerin stoğu ve fiyatı API üzerinden değiştirilebilir hale gelir.||

> ❗️ _Çoklu fiyat girişli olarak kurulmuş sitelerde ürünlere satış fiyatı girebilmek için öncelikle ürün kartı kaydedilmelidir. Daha sonra Ürün Yönetim sekmesindeki ürün fiyatları kısmında ![](https://snag.gy/1L3zat.jpg) butonuna basarak seçilecek fiyat tiplerindeki fiyatlar belirlenir._
