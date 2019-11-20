---
id: mail-icerik-yonetimi
title: Mail İçerik Yönetimi
---

Sistem tarafından gönderilen tüm otomatik maillerin görüntülendiği ve içeriklerinin düzenlebildiği sayfadır.

Herhangi bir mail kaydını güncellemek için mail listesinden güncellenmesi istenen kayda tıklanır. Açılan sayfada bulunan alanlar üzerinde değişiklik yapılır. Son olarak **Kaydet** butonuna tıklayarak değişikliklerin güncellenmesi sağlanır.

>❗ _Maillerin içerikleri güncellenirken **$** karakteri arasında gösterilen mail parametrelerinin silinmemesine dikkat edilmelidir. Bu parametrelerin yerleri değiştirilebilir. Eğer silinirse o parametrenin karşılığı olan metin gönderilen maillerde görüntülenmeyecektir.
Her mailin sağ üst köşesinde o mailde kullanılabilecek parametrelerin listelendiği **"Mail Parametreleri"** linki bulunmaktadır. Bu linke tıklayarak kullanılabilecek parametreler ve karşılık metin bilgileri öğrenilebilir._

<br>

**Örnek mail parametreleri:**

<code>$strKimeAdSoyad$</code>
Üye Adı ve soyadı bilgisidir.

<code>$strClientIpAdres$</code>
Mailin gönderildiği ip adresidir.

<code>$strUyeSifre$</code>
Üyeye ait şifre bilgisidir.

<code>$strKimeEMail$</code>
Üyenin mail adresidir.

<br>
## Sistem Tarafından Otomatik Gönderilen Mail Örnekleri

|Mail Adı|Açıklama|
|--|--|
|Üyelik Sözleşmesi|Sitede gözükmesini istediğiniz üyelik sözleşmesi metni bu alandan girilebilir.|
|Üyelik Aktivasyon Maili|Üye kayıt  işlemlerinde üyelerin aktivasyonu için sistem tarafından otomatik gönderilen maildir.|
|Üyelik Hoşgeldin Maili|Üyelik tamamlandığında son olarak üye olan kullanıcıya gönderilen hoşgeldin maildir.|
|Üyelik Şifremi Unuttum|Üyelerin önyüzden şifremi unuttum butonuna tıkladıklarında yeni şifre alması için sistem tarafından üyeye gönderilen maildir.|
|Bayi Başvurusu Onaylandı Bilgi Maili|Sistemde eğer Üyelik yerine Bayillik kullanılıyorsa, Bayi başvurusu onaylandığında gönderilen, email ve şifre bilgisi içeren sistem mailidir.|
|Üyelikten Üyelere Mesaj Gönderilirse|Admin kullanıcıların üyelere gönderdikleri maildir.|
|Ürün Tavsiye Et|Üyelerin önyüzden tavsiye modülünü kullandıklarında gönderilen maildir.|
|Arkadaşını Davet Et Mail İçeriği|Üyeler önyüzden tavsiye modülünü kullandıklarında arkadaşlarına sistem tarafından otomatik gönderilen maildir.|
|Satış Sözleşmesi|Sipariş onay sayfasındaki satış sözleşmesinin dinamik gelmesi için kullanılır.|
|Müşteriye Yeni Sipariş Onay Maili - Havale|Ödeme havale ile yapıldıysa sipariş adımının en sonunda, eğer hiç bir hata oluşmamışsa gönderilen maildir.|
|Müşteriye Yeni Sipariş Onay Maili - Kredi Kartı|Ödeme kredi kartı ile yapıldıysa sipariş adımının en sonunda, eğer hiç bir hata oluşmamışsa gönderilen maildir.|
|Satış Ortaklığı Sözleşmesi|Satış ortaklığı onay sayfasındaki satış ortaklığı sözleşmesinin dinamik gelmesi için kullanılır.|
|Siparişin Havale Onayı|Sipariş takip esnasında da Ödendi checkbox'ı tıklandığında sistem tarafından otomatik olarak gönderilen maildir.|
|Arkadaşını Davet Et Açıklama İçeriği|Arkadaş tavsiyesi işlemi yapılması için belirlenen koşulların dinamik olarak gelmesi için kullanılan maildir.|
|Üyelere Giden Mesaj Formatı|Üyelere gönderilmek istenilen mesajların gönderildiği maildir.|
|Sipariş Kargoya Verildi|Siparişi durumu kargoya verildi seçeneği seçildiği anda sistem tarafından otomatik gönderilen maildir.|
|Sipariş İptali|Sipariş iptal işlemi yapıldığında üyeye sistem tarafından otomatik gönderilen maildir.|
|Firmaya Giden Sipariş maili |Aktif tedarik işlemleri veya olası tedarik işlemleri sayfasından tedarikçilere gönderilen maildir.|
|Admine Yeni İşlem Olduğunda gidecek olan mail |Üyelerin önyüzden yeni bir yorum eklediklerinde gönderilen maildir.|
|Bonus çekiminde hata oluştuysa gidecek|Üyelerin bonus kullanımlarında hata oluşursa gönderilen maildir.|
|Üyelere doğum günlerinde gidecek olan mail|Üyelere doğum günlerinde sistem tarafından otomatik olarak gönderilen maildir.|
|Satış Ortaklığı Başvurusu Uyarı Maili|Üyeler önyüzden satış ortaklığı başvurusu yaptıktan sonra admine otomatik olarak gönderilen mail şablonudur.|
|Admine yeni sipariş olduğunda gidecek mesaj|Üyelerin önyüzden verdikleri sipariş için admine sistem tarafından otomatik gönderilen uyarı mailidir.|
|Üye soru sorduğunda yetkililere gidecek mesaj|Üyelerin on yüzden sordukları soruların yetkililere gönderildikleri maildir.|
|Admine Ürün adetleri kritiğe düştüğünde haber verilmesi|Kritik seçeneği seçilmiş ürünler, stokta belirlenen miktara düştüğü anda admine gönderilecek maildir.|
|Stok giren ürünlerin habercisi |Üyelerin önyüzden **Stoğa Gelince Haber Ver** butonuna tıkladıkları ürünler için stok girişi yapıldığında sistem tarafından otomatik gönderilen maildir.|
|Fiyatı Düşünce Haber Ver|Üyelerin önyüzden **Fiyatı Düşünce Haber Ver** butonuna tıkladıkları ürünler için fiyatları düşünce gönderilen maildir.|
|Hediye Çeki|Üyenin hediye çekinin gönderildiği maildir.|
|İndirim Kuponu|Üyeye İndirim kuponu hak kazandığında gönderilecek maildir.|
|İade Bildirim Maili|İade işlemlerinin ardından ödemenin iade alındığı bilgisinin gönderildiği maildir.|
|Depoya Sevkiyat Bildirim Maili |Sevkiyat birimine ilgili sipariş için gönderilen bildirim maildir.|
|Admine İptal Talebi yapıldığında gidicek olan Mail|Kullanıcı Siparişini iptal ettiğinde sipariş yöneticisine ulaşan bildirim mailidir.|
|Sipariş Bilgi Maili|Kullanıcı Sipariş verdiğinde, siparişine ilişkin bilgileri aldığı maildir.|

<br>

**Publish Mail İçeriği**

Site üzerinde bulunan bir içerik sayfası değiştirildiği durumda yetkilendirmenin verildiği kişiye aşağıda bulunan bilgiler;

<code>$strKimeAdSoyad$</code>
Mailin gideceği kullanıcının “Ad Soyad” bilgisi.

<code>$strKimeEMail$</code>
Mailin hangi mail adresine gideceğinin bilgisi.

<code>$strPblDurum$</code>
İçerik üzerinde yapılan en son işlem.

<code>$strIcerikUrl$</code>
Düzenleme yapılan içeriğin URL bilgisi.

<code>$strIcerikAd$</code>
Düzenleme yapılan içeriğin adı.

<code>$strDuzenleyenKln$</code>
İçeriği düzenleyen kullanıcının “Ad Soyad” bilgisi.

<code>$strWebAdresi$</code>
İlgili müşterinin aktif domain bilgisi (web adresi).

>❗ _İçerik Sayfasında yapılan bu değişiklikler yetkilendirme yapılan kişi tarafından onaylandığı zaman, içeriği düzenleyen kişiye “İçeriğin düzenleme işlemi”ne onay verildiğine dair mail gidecektir._

