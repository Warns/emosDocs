---
id: kategori-tanimi
title: Kategori Tanımı
---

##Kategori Tanımı 

![image.png](https://snag.gy/YnOfcA.jpg)

e-MOS her ürünün en az bir kategoriye bağlı olacağı kabulü ile hareket etmektedir. Bu yüzden herhangi bir ürün girişi yapılmadan önce ürüne bağlanacak kategorilerin tanımlanması gerekmektedir. Kategori tanımları sistem içerisinde sınırsız sayıda ve alt kategoride yapılabilmektedir.

- Ekle, Sil, Onay, Onay Kaldır butonlarından ürünü ekleme, silme, onaylama, onay kaldırma işlemlerini yapabilirsiniz.
![image.png](https://snag.gy/oAlvEg.jpg)

> ❗️ _Bir kategoriye onay verildiğinde sadece o kategori onaylanır, onay kaldırıldığında altındaki tüm kategorilerle beraber onayı kalkar._

Yeni bir kayıt oluşturmak için **Ekle** butonu kullanılır. Mevcut kayıtları düzenlemek için ise ilgili satırın üzerine tıklamak yeterlidir.

|Alan Adı|Açıklama|Örnek|
|--|--|--|
|Ulaşım Url|Bu kategoriye erişim önyüzden erişim sağlamak için kullanılacak url bilgisidir. Sayfa ismi girildiğinde ulaşım URL bilgisi bu bilgiyle aynı olur. Sayfa ismi boş bırakıldığında sistemin default çağırım sayfası URL olarak kullanılır.|/yatak-odası-dekorasyon.html?ref=0&ozs=0|
|Kategori Adı|Kategorinin adının girildiği alandır. ( ' " % &) gibi karakterler kategori adında kullanılmamalıdır. Kategori ismi tüm kategori ağacı için tekil olmalıdır.|Bilgisayar|
|Bağlı Kategori|Alt kategori tanımlamak için   butona tıklayarak bağlı olduğu kategori seçilir. Bu alan boş bırakılırsa girilen kategori ana kategori olarak kaydedilir.|Elektronik|
|Sayfa Başlığı|Bu kategoriye önyüzden tıklandığında açılan sayfanın başlığında görüntülenecek metnin yazıldığı alandır. Bu kısmın düzgün doldurulması Arama Motoru Optimizasyonu (SEO) için önemlidir.|Dizüstü Bilgisayarlar ve Tablet PC'ler|
|Sayfa İsmi|Bu alana kategoriyle ilişkili kelimelerden oluşan bir link bilgisi girilebilir. Bu linkin amacı kategori sayfasının arama motorlarında girilen link kelimeleri ile ilgili olarak daha üst sıralarda yer almasını sağlamaktadır.<br><br> ❗️ _Sayfa ismi tanımlanırken karakterlerin arasında boşluk bırakılmamalı, dile özgü karakterler kullanılmamalıdır. Sayfa ismi sistem bazında tekil olmalıdır._|yatak-odası-dekorasyon.html veya <br>/yatak-odasi/nevresim|
|Menü İcon|**Sayfa Yerleşim Düzenleme** ekranında **Header Menüsü** modülünde yeralan kategorileri ve çıkacak resimlerini belirler. Bu alanda resim seçildiğinde, kayan menüde bu kategorinin yer alacağı anlamına gelir.<br><br>❗️ _Kategorilerde ikon göstermek tasarıma bağlı bir özelliktir._|/UPLOAD/menuIcon/bilgisayar.jpg|
|Kategori Resim|Kategoriye bir resim eklendiğinde eklenen resim Alt Kat. Gösteriminde **Alt Kategorileri Yalnız Resimleri ile Göster** veya **Alt Kategorileri Resim ve Ürünleri ile Göster** seçimlerinden biri seçildiğinde kullanılacaktır. Yeni bir resim eklemek hakkında bilgi almak için lütfen [Tıklayın](/docs/resim-ve-dosya-yukleme.md). <br><br>❗️ _Kategorilerde resim göstermek tasarıma bağlı bir özelliktir._|/UPLOAD/menuImg/notebook.jpg|
|Özellik Seti|Daha önceden tanımlanmış olan özellik setlerinden biri  butonu yardımıyla ilgili kategoriye bağlanabilir. Böylece ön yüzden özellik seti seçilmiş kategoriye girildiğinde içerisindeki ürünlerin bu özellik seti uyarınca kıyaslanması sağlanır. Bu kategoride farklı özellik setine bağlı ürünler olduğu takdirde, bu ürünler önyüzden kıyaslanmak için seçilemeyecektir. Özellik setleri hakkında bigi bilgi almak istiyorsanız lütfen Tıklayınız.|Fotoğraf makinesi özellik seti|
|Alt. Kat. Gösterimi|Yanındaki butonuna tıkladığınızda size **Alt Kategorileri Listelenmesin**, **Alt Kategorileri Yalnız Resimleri ile Göster**, **Alt Kategorileri Resim ve Ürünleri ile Göster** seçeneklerini sunar. Bu seçim ürün kategori listelerinde yalnız alt kategori resimlerinin, alt kategori resimleri ile birlikte liste şeklinde içindeki ürünlerin veya resimleri ile birlikte tek tek ürünlerin listelenerek gösterilmesini sağlar.<br><br>❗️ _Alt kategorisi olmayan kategorilerde o kategoriye girildiğinde seçilen gösterim şekli kendisi için çalışacaktır. Yani alt kategorisi olmadığından kendisini seçilen gösterim şekli ile gösterecektir._||
|Ürün Liste Gösterimi|Yanındaki butonuna tıkladığınızda size **Ürünler Gösterilmesin**, **Katalog Şeklinde Göster**, **Liste Şeklinde Göster** seçeneklerini sunar. Ürün kategori listelerinde önce kategori gösterimi uyarınca kategoriler, altında ise ürün liste gösterimi uyarınca ürünler yerleşir.||
|Robots Meta Tag|Bu alanı kullanarak ilgili kategorinin SEO index ve follow tag'leri yönetilebilir. Dropdown menüde bulunan seçenekler: **"index, nofollow"**, **"noindex, follow"**, **"noindex, nofollow"**.||
|Platform|Bu alanı kullanarak ilgili kategorinin hangi platformda çalışacağı belirtilebilir. Dropdown menüde bulunan seçenekler: **Tablet(API)**, **Telefon(API)**, **Mobil**, **Masaüstü**||
|En Çok Satanlar|Bu alan, en çok satanlar yapısının kategori bazlı çalışması için kullanılır. Bu alan boş bırakıldığında en çok satanlar kurgusu Site Yönetimi > Temel Ayarlar > Site Ayarları > Diğer kısmındaki En Çok Satanlar ayarına göre çalışır. <br><br>❗️ _En üst seviye kategoride bu doldurulduğunda ilgili kategorinin tüm alt kategorileri için de geçerli olur. Aynı zamanda bu ayar ürünün bağlı olduğu ana kategori için geçerlidir._|45;10<br>Örnek olarak bu şekilde bir ayar girildiğinde son 45 güne bakar ve bu süre içerisinde bu kategoriden minimum 10 satış yapılmış ise bu kategorideki ürünleri en çok satanlar listesine ekler|
|Onay|Kategorinin geçerlilik veya geçersizlik durumunu belirler. Onaysız kategoriler önyüzde görüntülenmeyecektir. ||
|Breadcrumbs'da Gösterilmesin|Bu kutucuk işaretli olduğu durumda on yüzde ürün listede (kategori sayfalarında) üst kısımdaki breadcrumbs navigasyonunda ilgili kategori görünmeyecektir.||
|Google Kategori ID|Bu alan, Google kategori ağacı (Google Taxonomy) ile e-MOS'taki kategorileri eşleştirmek için kullanılır. Bu alan kullanıldığında Merchant XML çıktısında da bu kategori ID bilgisi yer alacaktır.||
|Açıklama|Açıklama alanı arama motorlarının arama sonuçları listesinde gösterdiği metnin girildiği kısımdır (meta description). Bu kısıma ilgili sayfayı tanımlayan bir yada iki cümlelik bilgi girilmelidir.<br><br>❗️ _Bu açıklama içerisinde kategori ile ilgili önemli kelimeleri kullanmanız arama motorları tarafından önem taşımaktadır._|Çocuk ayakkabı ve botlarında en sağlıklı, eğlenceli son moda bol çeşitle alışveriş imkanı yeşil’de.|
|Anahtar Kelime|Bu alan, arama motorlarının anahtar kelime etiketine karşılık gelir (keyword tag). Bu alanı kullanarak ilgili kategori için en önemli olan sözcüklerin (anahtar kelimeleri) girilmesi önerilir. Aynı zamanda **Keyword Rank** alanını kullanarak **Anahtar Kelimeler** bölümüne girilen kelimelerin önemini 1-10 arasında bir önem derecesi belirtilebilir|Çocuk, eğlenceli, renkli, bot, ..|
|Sıra|Kategorilerin görüntülenme sırasının belirlendiği alandır.||
|Ent. Kodu|Entegrasyon kodu müşterinin kullandığı ticari sistemdeki kategori kodu bilgisidir. Ticari sistem ile e-MOS arasındaki ilişkiyi sağlar ve entegrasyonlar bu koda göre yapılır.||
|Class|Kategoriler arasında tasarımsal farklılık oluşturulması için kullanılan sitil bilgisi bu alana girilir.||
|Min.Satış Mik.<br>ve<br>Max.Satış Mik.|Bu alanları kullanarak kategori bazında minimum ve maksimum satış miktarı belirtilebilir. Sepet onayı sırasında, kategori bazında minimum, maximum ürün sayısı kontrol edilir. <br><br>❗️ _Bir ürün iki farklı kategoride tanımlanmış ise ve iki kategorinin minimum ve/veya maksimum adetleri birbirinden farklı ise, karışıklık olmaması adına ürün tanımlanırken seçilen ilk "ön değer" kategorisinin minimum ve/veya maksimum adet değeri baz alınır._|Nevresim kategorisinde minimum miktar 10 ve maksimum miktar 15 olarak belirtildiğinde sepet onayı sırasında nevresim kategorisinden en az 10 ve en fazla 15 adet ürün olması gerekir (renk, beden vb. değerlerden bağımsız olarak).|

>❗️ _Hızlı alt kategori açabilmek için, ana kategorinin yanındaki kutucuk işaretlendikten sonra **Ekle** butonuna tıklanmalıdır._

>❗️ _Bir kategorinin yeri değiştirilmek isteniyorsa, bağlı kategori bilgisinin değiştirilmesi yeterli olacaktır. Yeri değişen kategorinin altındaki kategoriler de otomatik olarak taşınacaktır._