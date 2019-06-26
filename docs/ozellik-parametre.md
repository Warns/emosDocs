---
id: ozellik-parametre
title: Özellik Parametre
---

### Parametre Tanımlama

Özellik setlerine ait parametrelerin tanımlandığı sekmedir.

Ürün Özellik Tanımı sayfasındaki sol menüden Özellik Parametre linki ile açılan sayfada **Ekle** butonuna tıklanarak açılan form doldurulur.

> ❗ _Özellik parametrelerinin girişini daha hızlı yapabilmek için **Ekle** butonuna basmadan önce **Özellik Seti** ve **Özellik Grubu** kriterlerinden arama işlemi yapılmalıdır. Bu sayede açılan formda bu alanlar seçili olarak gelir. Her yeni kayıt eklendiğinde bu alanları tekrar seçme işlemi ortadan kalkmış olur._

|Alan Adı|Açıklama|
|--|--|
|Özellik Seti|Özelliklerin ekleneceği özellik setinin seçildiği alandır.|
|Özellik Grubu Adı|Özelliklerin ekleneceği özellik grubunun seçildiği alandır. Özellik seti seçilmeden özellik grubu seçilemez.|
|Parametre|Parametre adının girildiği alandır.|
|Parametre Açıklama|Ziyaretçiye parametre hakkında bilgi verilmek istenildiğinde kullanılır. Bu alan doldurulduğunda sitede parametrenin yanında bir ikon belirir, imleç ikonun üzerine getirildiğinde açıklama metni görüntülenir.|
|Parametre Şekli|Bu alan parametre tipinin seçildiği kısımdır.<br><br>**Fiyat Script:** Girilecek fiyat aralığı ile sitede filtre yapılmasını sağlayan parametre tipidir.<br>**Kelime ile Filtre:** Bu alana, önyüzden manuel olarak girilen sözcüğü filtre olarak uygular.<br>**Seçenekli:** Çoktan seçmeli filtreleme yöntemine uygun parametre tipidir.<br>**Elle Giriş:** Parametre değerinin elle girileceği durumlarda kullanılan parametre tipidir.<br>**Fiyat Aralığı:** Ürünlerin fiyat gruplarına göre filtrelenmesini sağlayan parametre tipidir.<br>**Ürün Seçeneği:** Ürünlerin renk, beden vb. özellikleri ile filtrelenmesini sağlayan parametre tipidir.<br>**Markalar:** Ürünlerin marka bazında filtrelenmesini sağlayan parametre tipidir.<br>**Çoklu Seçim:** Çoklu seçim olarak kullanılabilecek filtreler için uygulanır. Örn. Renk filtresinde birden çok seçim yapılabilmesi için|
|Class|Filtreyle ilgili önyüzde frontend ekibi tarafından bir özelleştirme yapılacağı zaman kullanılacak alandır.|
|Sıra|Girilen özelliğin özellik grubu içerisinde yer alacağı sıranın belirlendiği alandır.|
|Liste Sıra|Parametrenin, ürün listeleme sayfasında görüntülenen özet parametre alanındaki sırasının belirlendiği alandır.|
|Filtre Sıra|Parametrenin sitede filtre menüsündeki sırasının belirlendiği alandır.	|
|Filtre Kapalı Gelsin|Filtre menüsündeki parametrelerin açık ya da kapalı görünmesinin belirlendiği alandır.|
|Filtre Görünsün|Filtrenin önyüzde görünüp görünmeyeceğini belirler.|
|Filtre Kolon Sayısı|Filtre menüsündeki parametre değerlerinin kaç sütun halinde görüntüleneceğinin belirlendiği alandır.|
|Ent. Kodu|Entegrasyonuna bağlı olarak çalışan özellik parametresi için kullanılır.|
|Sayfa Index Tipi|Özellik parametre bazında sayfaya noindex meta tag eklenmesi için kullanılır<br><br>**Index:** Bu opsiyon ön değer olarak seçili gelmektedir. Bu opsiyon seçili olduğu zaman, bu sayfa, arama motorları tarafından indexlenecek aynı zamanda canonical bilgisi de yer alacaktır.<br>**Noindex:** Bu opsiyon seçili olduğu zaman ön yüzde filtre kısmında ilgili parametreye ait bir seçim yapıldığı andan itibaren sayfaya noindex ve nofollow meta tag’i eklenecek ve canonical bilgisi sayfadan kaldırılacaktır.<br>**Çoklu seçim noindex:** Bu opsiyon seçili olduğu zaman ön yüzde filtre kısmında ilgili parametreye ait birden fazla seçim yapıldığı andan itibaren sayfaya noindex ve nofollow meta tag’i eklenecek ve canonical bilgisi sayfadan kaldırılacaktır.|

Gerekli bilgileri girdikten sonra **Kaydet** butonuna tıklanır ve  parametre tanımlama işlemini tamamlanır.

> ❗ _Olası seçenek ve filtrelerin tanımlanabilmesi için öncelikle parametrenin kaydedilmiş olması gerekmektedir._


### Parametre Seçenek Tanımlama

Özellik setlerine ait parametrelerin seçeneklerinin tanımlandığı yerdir. (Örnek: Piksel Parametresine 1 megapiksel, 2 megapiksel, 3 megapiksel seçenekleri tanımlama).

Parametre kaydedildikten sonra aşağıdaki seçenekler bölümünde  **Ekle** butonuna tıklanır. Açılan sayfadaki alanlar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Parametre Seçenek|Parametre seçenek adının girildiği alandır.|
|Seçenek Açıklama|Ziyaretçiye parametre seçeneği hakkında bilgi verilmek istenildiğinde kullanılır. Bu alan doldurulduğunda sitede parametre seçeneğinin yanında bir ikon belirir, imleç ikonun üzerine getirildiğinde açıklama metni görüntülenir.|
|Ent. Kodu|Entegrasyona bağlı olarak çalışan parametre seçenek için kullanılır.|
|Sıra|Ekleyeceğiniz seçeneğin görüntülenme sırasının belirlendiği alandır.|

Gerekli bilgileri girdikten sonra **Kaydet** butonuna tıklanır ve seçenek tanımlama işlemini tamamlanır.

### Parametre Seçenek Filtreleri Tanımlama

Oluşturulan parametrelere filtre tanımlamak için;
Parametre güncelleme sayfasında Filtre kısmında **Ekle** butonuna tıklanır. Açılan sayfadaki alanlar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Filtre Adı|Fitlre adının girildiği alandır.|
|Seçenekler|Girilen filtrenin hangi seçenekleri kapsayacağının belirlendiği alandır.|
|Desen|Sitede filtre seçeneklerinin yanında görüntülenecek ikonların belirlendiği alandır.|
|Seçili Desen|Filtre seçeneği seçildikten sonra ikonunun alacağı görüntünün belirlendiği alandır.|
|Ent. Kodu|Entegrasyona bağlı olarak çalışan seçenek filtre için kullanılır.|
|Class|Seçenek filtreyle ilgili önyüzde frontend ekibi tarafından bir özelleştirme yapılacağı zaman kullanılır.|
|Sayfa İsmi|Filtre seçeneğin linkine karşılık gelir.|
|Sayfa Başlık|Filtre seçeneğin tarayıcı üzerinde yazacak başlığa karşılık gelir.|
|Açıklama|Filtre seçeneğiyle ilgili önyüzde kullanılabileçek açıklama alanına karşılık gelir|
|Sıra|İlgili filtre seçeneğinin sırasını belirleyen alandır.|

Gerekli bilgileri girdikten sonra **Ekle** butonuna tıklayarak filtre tanımlama işlemi tamamlanır.

>❗ _Özellik setlerinin önyüzde aktif olması için hem ilgili kategoride hem de o kategorideki ürünlerin Özellik Seti alanlarının seçilmiş olması gerekmektedir._<br><br>_Özellik filtrelerinin önyüzde görüntülenebilmesi için Tasarım Yönetimi sayfasından filtre kutusunun ilgili sayfaya yerleştirilmiş olması gerekmektedir. Tasarım yönetiminden filtre kutusu eklendiği  halde önyüzde görüntülenmiyorsa sayfada görüntülenen ürünlere bir özellik setleri tanımlanmamış demektir._<br><br>_Özellik seti tanımlandıktan sonra önyüzde ilgili kategoride filtre kutucuğu görünecektir. 1-4 megapiksel filtresine tıklanılırsa sadece 1,2,3 ve 4 megapiksel özelliği olan ürünler görüntülenecektir._