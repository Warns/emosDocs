---
id: satis-siparis-takibi
title: Satış Sipariş Takibi
---

Önyüzden gelen siparişlerin sevkiyat sürecine kadar yönetildiği ekranlardır. Ayrıca bu modül telefonla veya başka yollarla gelen siparişlerin (önyüzden verilmeyen siparişler) sisteme girilmesini sağlamak amacıyla da manuel olarak kullanılabilmektedir.

Sayfanın üst kısmında bulunan filtre seçenekleriyle aradığınız siparişe hızlıca ulaşabilirsiniz.

## 1. Genel Bilgiler

Panel üzerinden yeni bir sipariş oluşturmak için Satış Sipariş Takibi sayfasındayken **Ekle** butonuna tıklanır. Varolan bir siparişi yönetmek için istenen kaydın üzerine tıklayarak sipariş detay sayfasının açılması sağlanır. Açılan sayfadaki alanların açıklamaları aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Sipariş No|Müşterinin verdiği siparişin kodunun ekrana otomatik olarak geldiği alandır.|
|Müşteri |Siparişi veren üyenin isim bilgilerinin görüntülendiği alandır.|
|Fatura Adresi|Faturanın gönderileceği adres bilgisini gösterir. Gerektiği durumda teslimat adresini seçim butonuna tıklanarak adres değiştirilebilir.|
|Teslimat Adresi|Siparişin teslimatının yapılacağı adres bilgisinin gösterildiği alandır.|
|Para Birimi / Kur |Ödemenin alındığı para biriminin belirtildiği alandır. Kur tanımı ekranından girilen kur bilgisi burada otomatik oladak görüntülenmektedir.|
|Ödeme Tipi|Ödemenin nasıl yapıldığının belirlendiği alandır.|
|Nakliye|Müşteri siparişi verirken hangi Nakliye şirketini seçtiyse bu alanda o firma yer alır|
|Sipariş Tarihi|Siparişin verilmiş olduğu tarihin belirtildiği alandır.|
|Sipariş Tipi|Sipariş tipinin belirlendiği alandır.|
|Depo|Ürünün hangi depodan sevkedileceğinin belirlendiği alandır. Sevkiyat Yönetimi ekranlarında ilgili depo yöneticisi sadece kendi deposuna atanan siparişleri görebilecektir.|
|Durum|Siparişin hangi işlem sürecinden geçtiğini gösteren alandır. Önyüzden gelen bir siparişi yönetim paneli kullanıcısı Beklemede veya İptal durumuna getirebilir. Diğer durumlar Fatura kesimi, sevkiyat vb.. işlemler gerçekleştirildikçe otomatik olarak güncellenir.|
|Teklif No|B2B uygulamalarında müşteri sepeti için bir teklif isteyebilir. Eğer müşteri teklif istemişse bu alanda teklif numarası görüntülenir. Teklifin süreci "Satış Yönetimi > Teklif Takibi" menüsünden yönetilir.|
|Fiyat Tipi|Sipariş oluştururken hangi fiyat tipi üzerinden verildiğini gösteren alandır.<br>Fiyat Tipi hakkında ayrıntılı bilgi almak için [Tıklayın](fiyat-tipi-tanimi.md).|
|İstenilen Teslim Tarihi|Siparişin teslim edildiği tarihin belirlendiği alandır.|
|Farklı Alıcı|Müşteri siparişi teslim alacak ikinci bir kişi belirlediyse bu kişinin görüntülendiği alandır|
|E-Arşiv Fatura e-mail|E-Arşiv faturasının gönderileceği e-mail adresinin gösterildiği alandır.|
|Açıklama|Sipariş ile ilgili açıklama yazılan alandır.|
|Oluşturan Kul. Adı|Sipariş manuel olarak admin paneli üzerinden oluşturulmuş ise bu alanda kimin tarafından oluşturulduğunun bilgisi gösterilir.|
|Gün.Tarihi / Kul.Adı|Sipariş üzerinde değişiklik yapıldığı tarih ve değişikliği yapan admin panel kullanıcısının bilgisi.|
|Sip. Ver. Ip/Ülke/Şehir|Siparişin verildiği IP adres, ülke ve şehir bilgisi.|
|Kupon Kodu|Sipariş oluşturulurken kupon kodu kullanılmış ise bu alanda ilgili kupon kodunun bilgisi gösterilir.|
|Sipariş Desi (Net)|Siparişin net desi bilgisinin gösterildiği alandır.|
|Ent. Kodu|Kampanyanın ticari sistemdeki karşılığıdır. Sipariş ve fatura entegrasyonu sırasında ihtiyaca göre kampanyaya giren siparişlerde bu kodun entegrasyon ile gönderilmesini sağlar.|
|Kargo Takip No|Kargonun vermiş olduğu kargo takip numarasının girildiği alandır.|

<br>
## 2. Aksiyon Butonları
Görüntülemekte olduğunuz siparişle ilgili manuel olarak kullanılabilen butonlardır.

Butonlarla ilgili detaylar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Sevk Başlat|Siparişin tamamı için veya sipariş içerisinden istenilen ürünleri seçerek sevk işleminin manuel olarak başlatılabildiği butondur.|
|Mail Gönder|Siparişle ilgili kullanıcıya gönderilebilecek mail çıktısı. Bu butona tıkladığınızda gönderilecek mail içeriği açılır ve güncellenebilir.|
|Mesaj Gönder|Siparişle ilgili kullanıcıya gönderilebilecek SMS çıktısı. Bu butona tıkladığınızda gönderilecek SMS içeriği açılır ve güncellenebilir.|
|Sipariş İptal|Henüz faturası kesilmemiş Beklemede durumunda olan siparişler için kullanılabilecek manuel sipariş iptal butonudur.|
|Sıfırla|Faturası kesilmiş ve entegrasyonla ERP sistemine gönderilmiş bir siparişin entegrasyon kodunu sıfırlayan butondur.|

<br>
## 3. Sipariş Edilen Ürünler Bölümü
Bu bölümde sipariş içerisinde bulunan ürünler listelenir. Alt kısmında ise siparişle ilgili diğer ödeme detayları yer alır. 

Bu bölümde bulunan alanlarla ilgili detaylar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--
|Müşteri Notu|kullanıcı tarafından ilgili siparişle ilgili bir not bırakılmış ise bu alanda görünür.<br>❗️ _Bu süreç önyüz tasarımına ve yapısına bağlı olarak sipariş notu olarak bir not kısmı var ise çalışır._|
|Ödeme Notu|kullanıcı tarafından ilgili siparişle ilgili bir ödeme notu bırakılmış ise bu alanda görünür.<br>❗️ _Bu süreç önyüz tasarımına ve yapısına bağlı olarak ödeme notu olarak bir not kısmı var ise çalışır._|
|Hediye Paketi|Sipariş oluştururken hediye paketi yapılsın seçeneği seçilmiş ise bu kutucuk işaretli olur ve hediye paketleme sürecine tabi tutulur.<br>❗️ _Bu süreç önyüz tasarımına ve hediye paketi entegrasyon sürecine bağlı olarak çalışır._||
|Hediye Notu|Hediye paketiyle birlikte kullanıcı tarafından bırakılan hediye notunun kaydedildiği alandır.|
|Banka|Ödemenin yapıldığı bankanın görüntülendiği alandır.|
|Kart Üzerindeki İsim|Kredi kartının Ad-Soyad bilgilerinin görüntülendiği alandır.|
|Kart Numarası|Kredi kartı numarasının kısmi olarak göründüğü alandır.|
|Taksit Sayısı/Aylık|Taksit ve taksit tutarının göründüğü alandadır.|
|Banka Puan Kullanımı|Banka puanı kullanımı olduğunda tutarın görüntülendiği alandır.|
|Ödenecek Tutar|Siparişin toplam tutarının görüntülendiği alandır.|
|Sepetteki Ürün Toplamı|Sepetteki ürünlerin toplam tutarının görüntülendiği alandır.|
|Nakit İndirimi|Nakit ödemede kazanılacak indirim. Nakit ödeme süreçlerinin bulunduğu projelerde kullanılır.|
|Puan Kullanımı|İlgili siparişte kullanılan puan miktarının gösterildiği alandır.|
|Kampanya İndirimi|Sipariş oluşturma anında bir kampanyadan yararlanmış ise kampanyanın sağladığı indirimin gösterildiği alandır.|
|Vade Farkı|Vadeli alışverişlerdeki vade farkının görüntülendiği alandır.|
|Nakliye Bedeli|Siparişin nakliyesi sonucunda oluşan nakliye bedelinin görüntülendiği alandır.|
|Vergi Toplamı|Toplam vergi tutarının görüntülendiği alandır.|
|Toplam Tutar|Vergiler dahil Toplam tutarın görüntülendiği alandır. |
|Kazanılan Bonus|Alışveriş sonucunda müşterinin kazandığı site paunının görüntülendiği alandır.|
|GiftCard Tutarı|Sipariş oluşturuken bir gift card kullanılmış ise bu alanda kullanılan gift card tutarı gösterilir.|

<br>
Sipariş vermiş olduğunuz ürünün iptalini gerçekleştirmek için, sipariş güncelleme sayfasında seçmiş olduğunuz ürünün üzerine tıklayarak açılan sayfadaki alanları doldurmanız yeterli.

Alanlarla ilgili detaylar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Ürün Adı|Ürün isminin seçileceği alandır.	|
|Adet|Ürünün adetinin girildiği alandır.	|
|Brm. Fiyat|Ürünün birim fiyatının girildiği alandır.|
|İndirim|Üründe daha önceden yapılmış bir indirim varsa, otomatik olarak indirimin yazdığı ekrandır.|
|İndirim %|Üründe daha önceden yapılmış bir indirim varsa, otomatik olarak indirimin yüzdesinin yazdığı ekrandır.|
|Vergi|Ürüne uygulanacak verginin yazdığı alandır.|
|Vergi %|Ürüne uygulanacak vergi yüzdesinin yazdığı alandır.|
|Tutar|Ürünün toplam fiyatının görüntülendiği alandır.|
|Gerçek Vergi %||
|İptal|Eğer üründe iptal varsa, iptal miktarının girileceği alandır.|
|İptal Sebebi |Ürünün iptali durumunda iptal sebebinin yazıldığı alandır.|
|Ent. Kodu|Entegrasyon sürecine bağlı olarak çalışan bir yapıdır.|

<br>
## 4. Bilgi Sayfaları

Sayfanın sağ üst tarafında bulunan bilgi ekranlarla ilgili detaylar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Cari Hareketler|Sipariş ile ilgili yapılan tüm transaction işlemleri bu ekranda yer alacaktır. **Örnek:** Sipariş iptali, POS iadesinin tutarı, sipariş iadesi, kısmi iade vs.|
|Fatura Bilgileri|Sipariş ile ilgili faturaların bulunduğu ekrandır. Herhangi bir fatura kaydına tıklayarak faturanın detayına gidebilirsiniz.|
|Üye Mesajları|Siparişle ilgili kullanıcıyla yapılan mesajlaşmaların yer aldığı ekrandır.|
|Sipariş Logları|Sipariş ile ilgili servis üzerinden yapılan sorgu ve cevap şeklindeki XML log dosyalarının bulunduğu ekrandır.<br>❗️ _Ödemede oluşan sorunlardan dolayı geçersiz durumuna düşen ve banka tarafından hata dönen siparişlerde bu dosyaları bankaya ileterek detaylı inceleme yapılır._|

<br>
## 5. Sipariş Durumları ve Manuel Güncelleme

Kapanan durumundaki bir siparişin durumunu değiştirmek için [Satış Faturaları](satis-faturalari.md) sayfasından ilgili sipariş için oluşturulan Faturanın **İptal Et** butonu ile İptal edilmesi gerekir.

Bu işlem sonrasında sipariş "Kapanan" durumundan bir adım geri giderek "İşlemde" durumuna geçecek ve içerisinde biri "Yeni" diğeri "İptal" olmak üzere 2 adet Fatura oluşacaktır.

"İşlemde" durumundaki siparişi "Beklemede" durumuna almak için [Satış Sipariş Takibi](satis-siparis-takibi.md) sayfasından "Fatura Bilgileri" bölümünden Yeni durumundaki Faturanın seçilip silinmesi gerekecektir.

Bu işlemden sonra sipariş Beklemede durumuna gelecektir. Dilerseniz düzenleme yapıp siparişi yeniden kapatabilir yada İptal durumuna çekebilirsiniz.

## 6. Siparis Aktarım Yenileme

[Satış Sipariş Takibi](satis-siparis-takibi.md) sayfasından aktarımı yapılmış bir siparişin detayına girip, Ent. Kodu alanında bulunan Sıfırla butonuna tıklanması yeterlidir.

Bu işlem sonuncunda Ent. Kodunun silindiğini göreceksiniz. Sipariş aktarım entegrasyonu tekrar çalıştığında ilgili sipariş aktarılacak ve Ent. Kod alanı yeniden dolacaktır. 

Sitede bulunan siparişleri daha kolay süzebilmek için filtreleme kısmına “Hepsi”, “Sevk Tam”, “Sevk Eksik” seçenekleri bulunuyor. Bu seçenekler sipariş içerisinde bulunan ürünlerin sevk edilip/edilmedikleri durumlara bakarak süzme işlemi yapılabilecektir.

Sevk durumuyla ilgili alanların detayları aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Sevk Tam|Bir siparişin içerisindeki tüm ürünlerin sevk edildiği anlamına gelmektedir. Örn; Siparişin içerisinde 3 adet ürün var ve bu ürünlerin hepsi sevk edilmiş ise Sevk Tam olarak filtreleme yapıldığında bu sipariş filtrelenecektir.|
|Sevk Eksik|Bir siparişin içersindeki tüm ürünlerin sevk edilmediği anlamına gelmektedir. Örn; Siparişin içerisinde 3 adet ürün var ve bu ürünlerden 1 tanesi sevk edilmemiş ise Sevk Eksik olarak filtreleme yapıldığında bu sipariş görünecektir.|





