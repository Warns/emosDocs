İçerik Grup Tanımı, siteye eklenecek olan içerik sayfalarının oluşturulduğu kısımdır. Burada öncelikle
**Ekle** buttonu ile bir içerik grubu oluşturulur. Gelen ekranda;


|Alan Adı|Açıklama|
|--|--|
|Sayfa Grubu|Oluşturulacak İçerik Sayfa Grubunun adının girileceği alandır.|
|Sayfa Başlık|Sitede oluşturulan sayfaya girildiğinde browserın en üstünde gelecek olan başlık kısmının girileceği alandır.|
|Sayfa Açıklama|Oluşturulan sayfa hakkında kısa açıklama girilecek alandır.|
|Sayfa İsmi |Oluşturulan sayfanın linkini bu alandan belirleyebiliriz.Bu alanın boş bırakılması durumunda sistem otomatik link atayacaktır.|
|Bağlı Sayfa|Navigasyon yapısını oluşturmamızı sağlayan seçenektir. (kurumsal > hakkımızda)|
|Template Seçim|Template tanımında tanımladığımız parametreleri  HTML kodunda döngü içerisinde sayfaya bastığımız yapının seçildiği alandır.|
|Template Çoklu Seçim|Template tanımında tanımladığımız parametreleri  HTML kodunda döngü içerisinde sayfaya bastığımız yapının çoklu seçildiği alandır.|
|Onay|Oluşturulan sayfanın sitede aktif olması için onay alanının işaretlenmesi gerekmektedir.|
|Dil||
|Ters Sıra|Girilmiş olan içerik sıralamasının sayfada (ön yüzde) 1' den 9'a doğru gözükmesidir.|
|Sitemap|Siteye bağlı kategorilerin ve içerik sayfalarının gözüktüğü sayfadır. (Girilen içeriklerin Sitemap te göster Onay ının bulunması gerekiyor)|
|Login|Kullanıcıların sitede aktif olarak işlem yapabilmesi için giriş yapılan sayfadır.|
|Kaç Satırlı| Sürükle bırak yapısında ki satır sayısını ifade eder.|
|Sıra|Ön yüzde gözükmesi istenen içeriğin sıralamasının belirlendiği alandır.|


Örnek verecek olursak  **Yardım İçerik Grubu** içine **Müşteri Hizmetleri, Gizlilik ve Güvenlik , Ödeme Şekli,  Bize Ulaşın İçerikleri** tanımlanabilir.

####Template Oluşturmak

Template yapısının kullanımı yukarıda anlattıklarımızdan biraz daha farklıdır. Template yapısında "İçerik Grubu"nun kendisi bir sayfadır ve

"İçerikler" kısmına girilenler ise o sayfanın içinde yer alan, aynı özelliklere sahip ama birbirinden bağımsız nesnelerdir.

Örneğin; kampanyalarımızın bulunduğu bir sayfa oluşturmak istiyoruz. Bu sayfada birçok kampanya, aynı biçimde ve belli bir düzenle sıralanacak

ve her bir kampanyanın üzerine tıklandığında, o kampanya ile ilgili detay bilgisi verilen bir sayfaya gidecek. Bu örnek üzerinden template oluşturursak;

 

 
####İçerik Parametreleri :

 

Parametre tanımlarken;

|Alan Adı|Açıklama|
|--|--|
|Parametre Adı	|Oluşturulacak parametre adının belirlendiği alandır.|
|Parametre|HTML yapısında, parametrenin çağırılacağı değişken bilgisinin girileceği alandır. Bu alana girilen değer Template yapısında kullanılırken '$' işaretleri arasında kullanılmalıdırÖrn: $prmDeger$ gibi|
|Parametre Tipi|Tanımlanan parametre tipinin seçildiği alandır. Seçilebilecek alanlar (Rich Text : Html girişi yapılabilecek alan, Dosya Seçimi : FTP deki UPLOAD klasöründen herhangi bir dosya seçilebilecek ya da bir dosya upload edilebilecek alan, Metin : Kısa metin girişleri yapılabilecek alan, Seçenek : Çoklu seçim yapısı oluşturulabilecek alan)|
|Parametre Seçenek|Eğer Parametre tipi olarak "Seçenek" seçildiyse bu kısıma seçenek değerleri aşağıdaki şekilde girilmelidir.<br>Örn : SeçenekValue;SeçenekText, SeçenekValue2;SeçenekText2 vb.|
|Zorunlu alan|Oluşturulan parametre girişinin zorunlu olup olmadığını belirler.|


>❗  _Parametre tipi Seçenek olarak seçilip Seçenek kısmına değer girildiğinde bu parametreyi Template tarafında kullanabilmek için parametre adından sonra _text, _value eklenmelidir.
örn : Seçenek parametre adımız prmSecenek1 ise bu parametrenin text alanı için $prmSecenek1_text$, value alanı için $prmSecenek1_value$ şeklinde kullanılır._


gibi doldurulması gerekli kısımlar vardır.

Parametrelerimizi tanımladıktan sonra, bu parametrelerin kullanılacağı, html yapısını oluşturmamız gerekmektedir.


####Liste Template :

Kampanyalarımızın listelenme biçiminin (listedeki herbir kampanyanın) nasıl bir HTML yapısına sahip olacağının belirlendiği kısımdır. 


####Detay Tepmlate :

Listedeki herhangi bir kampanya üzerine tıklandığında gidilecek olan, kampanya detay sayfasındaki HTML yapısının belirlendiği kısımdır.

Oluşturduğumuz bu html yapısında, parametreleri çağırırken, "Parametre" kısmına girdiğimiz değişkeni, $ işaretleri arasına koyarak çağırmamız gerekmektedir. (Örn. <span>$prmBaslik$</span> veya <img src="$prmResim$" />, vb.

Eğer herhangi bir parametre tanımlamışsak, "İÇERİKLER" kısmından yeni bir kampanya eklemek istediğimizde gelen, içerik sayfası kısmı öncekine göre daha farklı bir yapıda gelecektir. Alt kısmında editör bulunmayan bu ekranda bizden, sayfa bilgilerinin dışında, tanımladığımız parametrelerin o kampanyaya ait değerlerinin girileceği kısımlar yer almaktadır. (Örn. Kampanya resminin seçilmesi, kampanya adının girilmesi, vb.
