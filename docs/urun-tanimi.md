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
### a. Dokümanlar
Sisteme yüklenmiş olan veya yeni eklenecek dokümanların ürünlere atandığı bölümdür. Dokümanlar linkine tıklandıktan sonra açılan sayfada ürüne bağlanmak istenen doküman eklenilir. Sayfa açıldığında ürüne doküman seçebilmek için ![](https://snag.gy/1L3zat.jpg) butonuna tıklanır.

|Alan Adı|Açıkalam|
|--|--|
|Doküman Adı|Dokümanın isminin girildiği alandır. Buraya girilen bilgi sitede doküman adı olarak görüntülenecektir.|
|Tipi|Dokümanların gruplanmasını sağlayan alandır. (Ör : Kullanım Klavuzu, Teknik Çizim, Ürün Sürücüleri vb.|
|Doküman|Seçim butonu ile sisteme yüklü olan dokümanlardan birininin seçildiği alandır. Eğer seçilecek doküman kayıtlı değilse **Dosya Yükle** butonunu kullanarak sisteme yeni bir doküman yüklenebilir. Dosya Yükleme hakkında ayrıntılı bilgi almak için [Tıklayınız](resim-ve-dosya-yukleme.md).|
|Ref.Doküman Seç||
|Dosya Boyutu||
|Dil||
|Onay||