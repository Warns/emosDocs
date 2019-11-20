---
id: pazaryeri-sss
title: Sıkça Sorulan Sorular
---

<details style="margin: 1rem;"><summary style="cursor: pointer;">Ürünün stoğu güncel değil, sebebi nedir?</summary>
<br>Ürünün eMOSta stoğu yok iken, pazaryeri panelinde stoklu olması veya paneldeki stokların stok fiyat gönder görevi çalışmasına rağmen e-MOS'tan farklı olması ürünün pazaryerine bildirilmediği yani güncellenmediği anlamına gelmektedir.  

Ürünün güncellenmemesinin sebebini tespit etmek için öncellikle log ekranı kontrol edilmelidir. İlgili ürün, log ekranında “İşleme alınan ürün”lerin arasında aratılmalıdır. Ürün pazaryerine bildiriliyor ancak bazı kurallara takılıp gönderilemiyorsa servisten uyarı mesajı döner ve log ekranına ürün ismi ile birlikte yansır.

Ürün “İşleme alınan ürün”lerin arasında değil ise ürün bildirilmiyor demektir. Bu durumda file log pasifse aktifleştirilmelidir. File log aktif edildikten sonra ürün üzerinde değişiklik yapılarak (Örneğin, açıklama alanında bir boşluk karakteri konulabilir) ürünün pazaryerine bildirilmesi için tetiklenmesi sağlanır. Sonrasında “Pazaryeri Ürün Stok Fiyat gönder” görevi çalıştırılır ve sunucuda pazaryeri loglarının bulunduğu klasöre gidilir. İlgili ürünün gönderilen ürünler arasında olup olmadığı kontrol edilir. Eğer ürün bu tetikleme sonrası bildirilmiş ve uyarı mesajı almış ise uyarı çözümlenmeye çalışılır. Alınan uyarı mesajı bilinmiyorsa ürünün request ve response dosyaları alınıp, müşterinin de CC’de yer aldığı bir mail ile ilgili pazaryerinin API Destek birimine iletilir veya müşterinin iletmesi için müşteriye gönderilir. API Destek biriminin yönlendirmeleri ile ürün gönderim sorununun çözümü için gerekli işlemler (tanımlama, seçim, onay vs) yapılır. Eğer uyarı dönmüyorsa veya ürün işleme alınmamışsa Backend ekibinde ilgili kişiye bilgi verilmelidir.  
</details>
<details style="margin: 1rem;"><summary style="cursor: pointer;">Stoğu olmayan ürün satılabilmiş, sebebi nedir? </summary>
<br>Ürünün stoğu güncellenmediğinde satış gerçekleşebilir. Bu durumda öncelikle ürünün neden güncellenmediği tespit edilmelidir. Bunun için pazaryeri log ekranı kontrol edilmelidir. İlgili ürün, log ekranında “İşleme alınan ürün”lerin arasında ve “Karşılaştırma raporu”nda aratılmalıdır. İşleme alınan ürünlerin arasındaysa yanında bulunan uyarı mesajı incelenmelidir. Bu uyarı mesajı ürünün neden güncellenmediği bilgisini verir. Bu bilgi doğrultusunda ürün üzerinde gerekli düzeltmeler yapılıp bilgisi müşteriyle paylaşılmalıdır. 

Bu tip durumların önüne geçmek için müşteri “Karşılaştırma raporu” loglarını incelemeli ve güncellenmeyen ürünleri takip etmelidir. Stoğunun güncellenmediğini tespit ettiği ürünleri “İşleme alınan ürün”lerin arasında aratıp uyarı mesajlarını okumalı ve bu uyarı mesajlarını dikkate almalı. Ürünün güncellenmesi için gerekli kriterlere sahip olmasını sağlamalı.   
</details>

