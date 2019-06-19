Farklı siteler için farklı yapılarda dinamik formların oluşturulabileceği modüldür. Oluşturulan formların önyüzden bilgi girişi yapıldığında belirlenen kişilere mail ile bilgilendirme yapılabilmesi mümkündür.

Form tipleri iki seçenekten oluşur; 

**Form:** Yeni bir form oluşturmak için kullanılır.
**Üyelik Formu:** Üyelik formuna istenilen alan ya da alanların eklenebilmesini sağlar. 

Form tipi seçilerek **ARA** butonuna tıklanır. Var olan formu güncellemek için ilgili kayda, yeni bir form oluşturmak için ekle butonuna tıklanmalıdır.

|Alan Adı|Açıklama|
|--|--|
|Form Başlık|Formun bulunduğu sayfaya form başlığı olarak gelecektir.|
|Açıklama|Form ile ilgili ön bilginin verildiği metinsel alandır. Girilen bilgi önyüzde müşteriye başlığın altında görüntülenir.|
|Mail Açıklama|Bu alana girilen bilgi, XMLForm Üye Bilgilendirme mailinin içeriği ile birlikte kullanıcıya gönderilir. Mail açıklama alanı XMLForma Üye Bilgilendirme mailindeki bir parametredir.|
|Bildirim E-mail|Bu formun içeriğinin veya form ile ilgili uyarı bildiriminin girilen mail adreslerine gönderilmesi sağlanır. Örnekte olduğu gibi noktalı virgül kullanılarak birden çok e-mail adresi girilebilir.|
|Dil|Formun oluşturulacağı dildir. ***SS*** butonuna tıklanarak dil seçimi yapılır.|
|Onay|Önyüzde formun görüntülenip görüntülenmeyeceğinin belirlendiği alandır.|
|Captcha Olsun Mu?|Bu alan işaretlendiğinde, ilgili XML form diyaznı için önyüzden bilgiler doldurulduğunda, formun gönderilebilmesi için öncelikle captcha bölümünün girilmesi zorlanır.|
|Template|Formun tasarımına ait HTML kodunun ve bunun içerisine yerleştirilen form parametrelerinin girildiği bölümdür.|


Yukarıdaki form doldurulduktan sonra **Kaydet**  butonuna tıklanarak kaydedilir ve XML Form Parametreleri bölümü aktifleşir. Yeni bir form parametresi oluşturmak için  **Ekle** butonuna tıklayınız.

- Form parametlerinin her biri önyüzde form nesnelerini oluşturmaktadır.

|Alan Adı|Açıklama|
|--|--|
|Parametre Adı|Parametrenin adının belirlendiği alandır.|
|Parametre Tipi|Parametrenin tipinin seçildiği alandır. ***SS*** butonuna tıklanarak parametre tipi belirlenir.|
|CssClass|Parametrenin oluşturacağı form nesnesinin alacağı CSS Class' ıdır.|
|Attribute|Form nesnesinin alacağı Attribute'ların girildiği alandır.|
|Text Format|Parametrenin uluşturacağı form nesnesinin formatının belirlendiği alandır. (Sadece sayısal değerler ve 10 karakterli olmalıdır.)|
|Ön Değer|Parametrenin oluşturacağı form nesnesinin ön değerinin belirlendiği alandır.|
|Parametre Seçenekleri|Parametre tipi olarak DropdownList veya Radio Button List seçildiğinde bu form nesnelerine ait olası değer ve textlerin girildiği alandır. Her bir değer-text grubu **buraya "pipe" gelicek** sembolü ile birbirinden ayrılır. Değer ve text bilgisi ise aralarına ";" sembolü koyularak girilmelidir.<br> Kullanım şekli: Value1;Text1,Value2;Text2|
|Sütun Adı|Önyüzde görünecek form nesnesinin sütun adının belirlendiği alandır. Bu bilgi XML Form Data sayfasında girilen formlar gösterilirken kolon başlıkları olarak kullanılacaktır. Bu başlıklardan hangilerinin gözükeceğini "Listede Gözüksün Mü?" checkbox ı belirler.|
|Mail Sıra|Önyüzden form girişi yapıldığında bilgilendirme maili atılacak kişilere formun hangi kolonlarının, hangi sıra ile mail gövdesinde görüntüleneceğini belirler."0" girdiğimiz takdirde girmiş olduğumuz parametre maille gönderilmeyecek; 1,2,... gibi girilen rakamlar parametre sıra numarasını belirleyecek ve ilgili parametrenin mail içerisinde de gönderilmesini sağlayacaktır.|
|Liste Gözüksün Mü?|XML Form Data Tanımı ekranındaki listeleme ya da excel raporlama yapıldığında kullanılacak olan kolonları belirler.|
|Onay|Önyüzde parametrenin görüntülenip görüntülenmeyeceği belirlenir.|

Yukarıdaki form doldurulduktan sonra **Kaydet** butonuna tıklanarak girilen bilgiler kaydedilir.