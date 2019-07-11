---
id: satis-sevk-yonetimi
title: Satış Sevk Yönetimi
---

Sevkedilmeye hazır olan satış faturalarının izlendiği ve yönetildiği ekrandır.

Bu ekranı depodan sevkiyat yapacak birimler kullanır. Sadece kendi depolarındaki sevk edilecek ürünleri görürler ve sevkiyat işlemini tamamlarlar. 

>❗️ _Fatura kesim tarihi eğer günün tarihinden eski ise "Eski tarihli faturayı kesmek üzeresiniz. Devam etmek istiyor musunuz?" şeklinde Pop-Up çıkarak kullanıcıyı bilgilendirir. Satış Sevk Yönetimi sayfasında XXX numaralı fatura içerisine girdiğinizde günün tarihinden farklı bir tarih olduğunda "Fatura Kes" butonuna basıldığında aynı şekilde Pop-Up çıkarır._

![](https://snag.gy/85Z3Js.jpg)
                                      
**Faturayı Kesildi Duruma Getirmek için;**
- İlgili sipariş kaydına tıklanır.
- Açılan sayfada **Fatura Bilgileri** sekmesine tıklanır.
- Siparişe ait bir veya birden fazla faturanın bulunduğu **Faturalar** listesi görüntülenir. Bu listeden ilgili fatura kaydına tıklanır. 
- Ödemesi yapılmış ve Beklemede durumunda olan birden fazla siparişin kapatılması için ise **Toplu Fatura Kes** butonu kullanılır. Toplu Fatura Kes butonu kullanılmadan önce, faturası kesilmek istenen siparişlerin yanında bulunan kutucukların işaretlenmesi gerekmektedir.
- Açılan sayfada **Fatura Numarası** alanı doldurulup sayfa kaydedilir ve **Fatura Kes** butonuna tıklanarak işlem sonlandırılır. Eğer fatura çıktısı e-MOS tan yapılmıyorsa bilgileri yazıcıya gönderilen pencere çıkmaz. Yazıcıya fatura çıktısı alınacaksa aşağıdaki işlemlerin yapılması gerekmektedir.

**Nokta vuruşlu yazıcıdan çıktı almak için;**
- **Fatura Kes** butonlarına tıklanır.
- Açılan pencerede **Yazdır** butonun tıklanır.

>❗️ _Eğer bu buton görüntülenmiyorsa Java Yazılımı yüklenmemiş demektir. Yazılımın yüklenmesi aşağıda anlatılmıştır._

- Son olarak **Generic / Text Only** yazıcısı seçilip işlem onaylanır ve fatura / irsaliye basımı tamamlanır.  (Nokta vuruşlu yazıcıdan çıktı alabilmek için yapılması gereken teknik ayarlar aşağıda anlatılmıştır.)

**Nokta Vuruşlu Yazıcıdan çıktı almak  için gerekli teknik ayarlar**

Nokta buruşlu yazıcıdan sağlıklı çıktı alabilmek için **Ücretsiz Java Yazılımın ve Generic / Text Only** yazıcısının işlemi gerçekleştirecek bilgisayarlara yüklenmesi  gerekmektedir.

**Java Yazılımını yüklemek için;**

- İnternet tarayıcısından [http://www.java.com/tr] sitesi açılır.
- Açılan siteden Ücretsiz Java Yazılımı bilgisayara indirilir.
- İndirilen dosya bilgisayara kurulur.

**Generic / Text Only yazıcısının bilgisayara tanıtılması için;**

- **Denetim Masasına** gidilip **Yazıcılar ve Fakslar** tıklanır.
- Yazıcı Ekle butonuna tıklanır.
- İlk 3 adım Next e basılır (yazıcı seçilen ekrana kadar)
- Manufacturer (Generic ya da Sosyal) seçildikten sonra sağda görüntülenen yazıcılardan Generic / **Text Only** yazıcısı seçilir.
- Yazıcı ekleme işlemi sonlanana kadar **Next** denir. Son stepte **Finish** seçilir ve yazıcı ekleme işlemi sonlanır.
- Eklenen yazıcının üstüne gelip **Properties** e basılıp açılan sayfada **Font Selection** tabına gelinir.
- **Code Page** alanından MS-DOS Turkish seçilip **OK** butonuna tıklanır. 

**Fatura kesim ekranında aşağıdaki alanlar bulunmaktadır;**

- Fatura güncelleme ekranı (Faturanın kesim işlemi tamamlanmadan önceki ekrandır.)

|Alan Adı|Açıklama|
|--|--|
|Müşteri|Siparişi veren üyenin isim bilgileri görüntülenir.|
|Fatura Adresi|Faturanın gönderileceği adres bilgisini gösterir. Gerektiği durumda teslimat adresini seçim butonuna tıklanarak adres değiştirilebilir.|
|Sevk Adresi |Siparişin teslimatının yapılacağı adres bilgisi gösterilir. |
|Fatura No |Faturanın numarasının girildiği alandır.	|
|Fatura Tarihi|Faturanın kesim tarihinin girildiği alandır.|
|İrsaliye No|İrsaliye numarasının girildiği alandır.|
|İrsaliye Tarihi|İrsaliyenin kesim tarihinin girildiği alandır.|
|Nak. Firma|Nakliye işleminin hangi kargo tarafından yapıldığı seçeceğiniz alandır.|
|Waybill No|Kargonun vermiş olduğu kargo takip numarasını girildiği alandır.|
|Kargo Ölçümü|Sipariş edilen ürünün m3 cinsinden ölçümünün girileceği alandır.|
|Kargoya Ödenen|Kargoya ödenen ücretin yazıldığı alandır.|


- Fatura izleme ekranı (Fatura kesim işlemi tamamlandıktan sonra olabilicek değişiklikler açısından faturanın izlendiği ekrandır.)

|Alan Adı|Açıklama|
|--|--|
|Müşteri|Siparişi veren üyenin isim bilgileri görüntülenir.	|
|Fatura Adresi|Faturanın gönderileceği adres bilgisini gösterir. Gerektiği durumda teslimat adresini seçim butonuna tıklanarak adres değiştirilebilir.|
|Sevk Adresi |Siparişin teslimatının yapılacağı adres bilgisi gösterilir. |
|Ödeme Tipi |Ödemenin nasıl yapılıcağının belirtildği alandır.|
|Para Birimi |Ödemeyi yapacağınız para birimini belirteceğiniz alandır.	|
|Depo|Siparişin sağlanacağı deponun seçileceği alandır.|
|Durum|Siparişin hangi durumda olduğunun belirlendiği alandır.	|
|Fatura No |Faturanın numarasının girildiği alandır.|
|Fatura Tarihi |Faturanın kesim tarihinin girildiği alandır.|
|İrsaliye No |İrsaliye numarasının girildiği alandır.|
|İrsaliye Tarihi |İrsaliyenin kesim tarihinin girildiği alandır.|
|Sevk No|Sevkiyat numarasının girildiği alandır.|
|Nak. Firma|Nakliye işleminin hangi kargo şirketi tarafından yapıldığını gösteren alandır.|
|Waybill No|Kargonun vermiş olduğu kargo takip numarasının gösterildiği alandır.|
|Kargo Ölçümü|Sipariş edilen ürünün m3 cinsinden ölçümünün yazdığı alandır.	|
|Kargoya Ödenen|Kargoya ödenen miktarın yazdığı alandır.|
|Taşıyıcı Tipi |Kargoda kullanılan taşıyıcının tipinin belirtildiği alandır.|
|Taşıyıcı No |Taşıyıcı Numarasının Görüntülendiği alandır.	|
|Teslim Edildi|Bu kutucuk işaretlenirse siparişin fatura kesim işlemi tamamlandı kabul edilir.	|