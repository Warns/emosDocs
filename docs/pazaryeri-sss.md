---
id: pazaryeri-sss
title: Sıkça Sorulan Sorular
---

<details><summary>Ürünün stoğu güncel değil, sebebi nedir?</summary>
<p>
Ürünün eMOSta stoğu yok iken, pazaryeri panelinde stoklu olması veya paneldeki stokların stok fiyat gönder job ı çalışmasına rağmen eMOStan farklı olması ürünün pazaryerine bildirilmediği yani güncellenmediği anlamına gelmektedir.  

Ürünün güncellenmemesinin sebebini tespit etmek için öncellikle log ekranı kontrol edilmelidir. İlgili ürün, log ekranında “İşleme alınan ürün”lerin arasında aratılmalıdır. Ürün pazaryerine bildiriliyor ancak bazı kurallara  takılıp gönderilemiyorsa servisten uyarı mesajı döner ve log ekranına ürün ismi ile birlikte yansır. Bkz. Şekil 2.2.2.4.1  

Ürün “İşleme alınan ürün”lerin arasında değil ise ürün bildirilmiyor demektir. Bu durumda file log pasifse aktifleştirilmelidir. Bkz.Şekil 2.2.2.4.2 File log aktif edildikten sonra ürün üzerinde değişiklik yapılarak (Örneğin, açıklama alanında bir boşluk karakteri konulabilir) ürünün pazaryerine bildirilmesi için tetiklenmesi sağlanır. Sonrasında “Pazaryeri Ürün Stok Fiyat gönder” job ı çalıştırılır ve sunucuda pazaryeri loglarının bulunduğu klasöre gidilir. İlgili ürünün gönderilen ürünler arasında olup olmadığı kontrol edilir. Eğer ürün bu tetikleme sonrası bildirilmiş ve uyarı mesajı almış ise uyarı çözümlenmeye çalışılır. Alınan uyarı mesajı bilinmiyorsa ürünün request ve response dosyaları alınıp, müşterinin de Cc’de yer aldığı bir mail ile ilgili pazaryerinin API Destek birimine iletilir veya müşterinin iletmesi için müşteriye gönderilir. API Destek biriminin yönlendirmeleri ile ürün gönderim sorununun çözümü için gerekli işlemler ( tanımlama, seçim, onay vs) yapılır. Eğer uyarı dönmüyorsa veya ürün işleme alınmamışsa Backend ekibinde ilgili kişiye bilgi verilmelidir. 

Önemli: Bazı müşteriler File log kaydının sürekli aktif durumda olmasını talep etmektedir, bu sebeple müşterinin onayı olmadan file log kaydı pasif edilmemelidir.  
</p>
</details>

