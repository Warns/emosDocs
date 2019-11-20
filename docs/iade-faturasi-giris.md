---
id: iade-faturasi-girisi
title: İade Faturası Girişi
---

Kullanıcıların herhangi bir nedenden dolayı iade ettikleri ürünlerin faturalarını belirli kriterlerde raporlayan sayfadır.

Yeni bir iade faturası girişi yapmak için **Ekle**  butonuna tıklanarak açılmış olan aşağıdaki form doldurulur.

|Sütun Adı |Açıklama|
|--|--|
|Fatura No|İade edilen ürünün faturasında belirtilen fatura numarasını girilen alandır.|
|Fatura Tarihi |İade edilen ürünün faturasında belirtilen tarihi girmeniz gereken alandır.|
|Ent. Kodu|İade girişi yapılan faturanın entegrasyon kodunun görüntülendiği alandır.|
|Depo|İade edilen ürünün hangi depodan geldiğini girmeniz gereken alandır.|
|Müşteri|İade işlemi gerçekleştiren müşterinin isim bilgisini girmeniz gereken alandır.|
|Ödeme Tipi |Ürünün ödeme şeklinin (Havale,Kredi Kartı) belirtildiği alandır.|
|Para Birimi |Ürünün para biriminin <code>USD</code> <code>YTL</code> <code>EUR</code> belirtildiği sütundur.|
|Kur|Kurun girildiği alandır.|
|Onay|İade işleminin onaylanması halinde kutucuğun işaretlenmesinin gerekli olduğu alandır.|
|Vade Tarihi|Ürünün satışının vadelendirilmesi halinde yapılıcak aylık ödemelerin ödeneceği tarihin belirtildiği alandır.|
|Açıklama|İade işlemiyle ilgili açıklama yapabileceğiniz alandır.|

>❗️ _İade Faturası Girişi ekranına **Entegrasyon Kodu** eklenerek, Entegrasyon Koduna göre filtreleme yapılması sağlanmıştır._

>❗️ _**"Otm. İade Oluştur"** alanı e-MOS da yer alan satış faturasının sistem numarası girilerek, o faturaya ait tüm ürünlerin iade faturası otomatik olarak oluşturulabilmektedir.
Bunun yanı sıra eklenen iade faturasının onayı verildikten sonra Ödeme Yapıldı olarak işaretlenen faturalar için, müşteriye iade konusunda gönderilecek mail şablonu otomatik olarak oluşturulmakta ve gönderime hazır şekilde site yöneticisine gösterilmektedir. Burada gönderilecek mail içerisinde ekleme çıkarma işlemleri yapılarak gönderilmesi mümkündür. 
Satış fatura listesinin yer aldığı ekranda fatura bazında dökülebilen İade Döküm raporundaki barkodlu kısım, iade bölümünde girilen bu alana karşılık gelmektedir._

<br>

Yukarıda doldurmuş olduğunuz formu kaydettikten sonra **Fatura Detayı** bölümü aktif olur.


|Sütun Adı |Açıklama|
|--|--|
|Ürün|İade edilen ürünün belirtilmesi gereken alandır.|
|Fatura No|İade edilen ürünün faturasında belirtilen numaranın ekrana otomatik olarak geldiği alandır.|
|Adet|İade edilen ürünün adetinin belirtilmesi gereken alandır.|
|Brm. Fiyat|İade edilen ürünün birim fiyatının belirtilmesi gereken alandır.|
|İndirim|İade edilen ürüne uygulanmış olan indirim varsa, ekranda otomatik olarak bu alanda gösterilir.|
|Vergi|İade edilen ürününden alınan verginin otomatik olarak geldiği alandır.|
|Toplam|İade edilen ürünün toplamının ekrana otomatik olarak geldiği alandır.|
|İade Sebebi|İade edilen ürürün iade gerekçesinin belirtilmesi gerekli olan alandır. (Yanlış seçim, hasarlı ürün vb.)|
|İndirim%|Ürüne uygulanmış olan indirimin yüzde değerinin girildiği alandır.|
|Vergi%|Ürüne uygulanan verginin yüzde değeri girildiği alandır.|
