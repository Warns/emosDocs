---
id: script-yoneticisi
title: Script Yöneticisi
---

Script manager, müşterilerin script entegrasyonları için yapılan bir çalışmadır. Müşteriler tarafından talep edilen, sistemde olmayan yada varolan şekliyle uyumsuz olan script entegrasyonları için yazılım ekibi tarafından geliştirme/güncelleştirme işlemleri yapılmaktaydı. Yapılan bu geliştirme/güncelleştirme işlemlerinin canlı ortama taşıma işlevi her zaman yapılamadığından dolayı müşterilerin zaman kaybetmesine neden oluyordu. Bu yapı sayesinde sistemde ön tanımlı ya da özel script entegrasyonları sisteme doğrudan dinamik şekilde eklenebilecek.

Ekran standartları için Tıklayınız.

Script Yöneticisi, Master ve Detay olarak 2 bölümden oluşmaktadır;

**Master Ekranı:**

####1. Sekme (Genel Bilgiler)

|Alan Adı|Açıklama|
|--|--|
|Script|Sistemde ön tanımlı olan script veya özel entegrasyon tipini seçmek için kullanılmaktadır.|
|Açıklama|Script'e açıklama girmek için kullanılan alandır. Bu alana eklenen açıklama önyüze yansımamaktadır.|
|Parametreler|Script içerisinde özel parametre(ler) kullanabilmek için kullanılan bölümdür. Parametreler aralarına ";" belirtilerek ve ekleme sırasına göre ilgili sayfalarda “$prm[parametreSırası]$” şeklinde kullanılmalıdır.|
|Parametre Açıklaması	||
|Çalışma Tipi|Script entegrasyonunun ajax yapısı yada doğrudan sayfa output yoluyla çalıştırılmasını belirlemek için kullanılan parametredir. Dinamik bir işlem olmadığı sürece Senkron yapısı kullanılmalıdır. Eğer entegrasyon "Üye Login" gibi anlık değişebilen bir yapı içeriyorsa "Asenkron" yapı seçeneği seçilmelidir. Asenkron yapı seçildiğinde sistem ajax altyapısı üzerinden işlemleri yapacaktır. Eğer senkron yapı seçilirse "Üye Login" işlemindeki parametreler hatalı getirilebilir.|
|Sıra||

####2. Sekme (Diğer Bilgiler)

|Alan Adı|Açıklama|
|--|--|
|Header Script|Header Script alanına eklenen parametre belli başlı js dosyalarının ajax yapısı ile çağırılmasının sorun oluşturduğu entegrasyonlar için kullanılan bölümdür. Bu bölüme girilen bilgiler doğrudan sayfada "head" içerisine eklenmektedir. Bu sayede js dosyaları sayfa yüklenirken hazır duruma gelmektedir.|
|Header Script (Sayfa Bazlı)|Bu bölüm belli başlı js dosyalarının ajax yapısı ile çağrılmasının sorun oluşturduğu entegrasyonlar için kullanılan bölümdür. Bu bölüme girilen bilgiler doğrudan sayfada “head” içerisine eklenmektedir. Bu sayede js dosyaları sayfa yüklenirken hazır duruma gelmektedir. Bu özelliği master’daki “Header Script” ten ayıran en büyük fark ise sayfa bazlı çalışmasıdır. Bu özellik kullanılarak o anki sayfaya özel kodlar eklenebilmektedir.|
|Header İçerik|Bu bölüm ilgili sayfa içeriği basılmadan önce basılan script içeriğidir. İlgili detay içerikte aksi belirtilmediği sürece script içeriğine dahil edilmektedir. Kullanım şekline örnek verecek olursak; her sayfada olması gereken temel script bilgileri ya da belli başlı parametreler bu bölüme eklenerek ilgili sayfalarda kullanılabilir.|
|Footer İçerik|Bu bölüm ilgili sayfa içeriği basıldıktan sonra içeriğe eklenen script içeriğidir. İlgili detay içerikte aksi belirtilmediği sürece script içeriğine dahil edilmektedir. Kullanım şekline örnek verecek olursak; Her sayfada, sayfa içeriği eklendikten sonra çalıştırılması gereken script kodları var ise bu parametre kullanılabilir..(Örnek Visilabs ent. Gibi her sayfada kullanılan VL.Collect() methodu footer içeriğine eklenerek her sayfada otomatik olarak çalıştırılması sağlanabilir.)|
|Onay	|İstenilen script entegrasyonu grubunun önyüze yansıtılıp yansıtılmayacağını belirlemek için kullanılan parametredir. Bu parametre sayesinde istenen entegrasyon silinmeden devre dışı bırakılabilir.|


**Detay Ekranı:**

####1. Sekme (Genel Bilgiler)

|Alan Adı|Açıklama|
|--|--|
|Script|Sistemde ön tanımlı olan script veya özel entegrasyon tipini seçmek için kullanılmaktadır.|
|Sayfa|Script’in hangi sayfada çalıştırılması isteniyorsa ilgili sayfa tipinin seçildiği bölümdür. Sistem, otomatik olarak hangi tip seçilmişse duruma göre ilgili script içeriğini o sayfada ve belirli kurallar çerçevesinde çalıştıracaktır.|
|Not|Sayfa tiplerine opsiyonel olarak açıklama girmek için bu bölüm kullanılabilir.|
|Header/Footer Aktif mi?|Bu parametre, Master üzerinde girilen “Header İçerik” ve “Footer İçerik” parametrelerinin sayfaya yansıtılıp yansıtılmayacağını belirlemek için kullanılır. Bu parametre aktif olduğunda ilgili sayfa için girilen içeriğe Header ve Footer içeriği dahil edilmez. Bu sayede özel durumu olan sayfalarda header/footer içeriklerinin çalıştırılması engellenebilir.|
|Sıra|Scriptlerin hangi sırada çalıştırılacağını belirlemek için kullanılan bölümdür. Burada belirlenen sıra üzerinden script içerikleri çalıştırılacaktır.|
|Onay|İçeriğin önyüze yansıtılıp yansıtılmayacağını belirlemek için kullanılan parametredir. Bu parametre sayesinde istenen içerik silinmeden devre dışı bırakılabilir.|
|Script İçerik|İlgili script entegrasyonu için içeriğin girildiği bölümdür. Bu bölüme girilen içerik istenilen sayfada ve koşulda önyüze yansıtılacaktır.|

####Sayfalara Göre Kullanılabilecek Sayfa Tipleri ve Açıklamaları:

|Sayfa Tipi|Açıklama|
|--|--|
|Ana Sayfa|Anasayfada çalıştırılması gereken script kodları için kullanılan sayfa tipidir.|
|Ürün Detay|Ürün detay sayfasında çalıştırılması gereken script kodları için kullanılan sayfa tipidir|
|Sepet|Sepete eklenen ürünlerin listelendiği sayfada çalıştırılması gereken script kodları için kullanılan sayfa tipidir.|
|Sepet’e Ürün Ekleme|İlgili ürün için sepet’e ekleme işlemi yapıldığında, sayfada çalıştırılması gereken script kodları için kullanılan sayfa tipidir.|
|Sipariş Sonuç(Başarılı Sipariş Oluşturma)|Ürün liste sayfasında çalıştırılması gereken script kodları için kullanılan sayfa tipidir.|
|Üye Login|İlgili ürün için sepet’e ekleme işlemi yapıldığında, sayfada çalıştırılması gereken script kodları için kullanılan sayfa tipidir.|
|Üye Kayıt(Başarılı)|Ziyaretçi sisteme başarı ile üye olduğunda çalışan sayfa tipidir.|
|Üye Profil Güncelleme|Üye profil güncelleme işlemi yapıldığında çalışan sayfa tipidir.|
|Üye Adres Ekleme & Güncelleme|Üyenin sipariş için eklediği ya da güncellediği durumda çalışan sayfa tipidir.|
|İçerik|İçerik sayfalarında çalışan sayfa tipidir.|
|Arama|Arama yapıldığında, arama sonuçlarının döküldüğü ekranda çalışan sayfa tipidir.|
|Tüm Diğer Sayfalar|Tanımı yapılmamış sayfa tipleri dışındaki sayfalarda çalışan sayfa tipidir. Eğer “Tüm Diğer Sayfalar” tipi dışında başka herhangi bir sayfaya tanım yapılmamışsa, belirtilen içerik tüm sayfalarda çalışacaktır.|
|Script içeriğini Güncelleme|Bu parametre üzerinden tüm script içeriğinin bir numaralı müşterideki son hali çekilebilir. Bu sayede ön tanımlı entegrasyonlar üzerinden hızlıca kod yazılabilir.|
