---
id: sms-icerik-yonetimi
title: SMS İçerik Yönetimi
---

Sistem tarafından gönderilen otomatik SMS'lerin görüntülendiği ve içeriklerinin düzenlenebildiği sayfadır.

Herhangi bir SMS kaydını güncellemek için SMS listesinden güncellenmesi istenen kayda tıklanır. Açılan sayfada bulunan alanlar üzerinde değişiklik yapılır. Son olarak **Kaydet** butonuna tıklayarak değişikliklerin güncellenmesi sağlanır.

>❗ _SMS içerikleri güncellenirken $ karakteri arasında gösterilen sms parametrelerinin silinmemesine dikkat edilmektedir. Bu parametrelerin yerleri değiştirilebilir. Eğer silinirse o parametrenin karşılığı olan metin gönderilen maillerde görüntülenmeyecektir.
Her SMS'in sağ üst köşesinde o sms'de kullanılabilecek parametrelerin listelendiği **"SMS Parametreleri"** linki bulunmaktadır. Bu linke tıklayıp kulanılabilecek parametreler ve karşılık metin bilgileri öğrenilebilir._

<br>

**Örnek SMS parametreleri :**

<code>$strUyeCepTel$</code> Üyenin cep telefonu bilgisidir
<br>
<code>$strOnayKodu$</code> Üyeye gönderilecek onay kodudur

<br>

## Sistem Tarafından Otomatik Gönderilen SMS Örnekleri

|Sms Adı|Açıklama|
|--|--|
|Üyelik Aktivasyon Mesajı|Üye kayıt işlemleri sırasında Onay Kodu için gönderilen SMS'dir.|
|Sipariş Kargoya Verildi Mesajı |Sipariş Takip bölümünden üyeye ait sipariş için kargoya verildi seçeneği işaretlendiğinde gönderilen SMS'dir.|
|Sipariş Alındı Mesajı|Başarılı bir şekilde sipariş verdikten sonra kullanıcıya gönderilecek SMS içeriğinin girildiği SMS'dir.|