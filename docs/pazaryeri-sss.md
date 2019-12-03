---
id: pazaryeri-sss
title: Sıkça Sorulan Sorular
---

<details style="margin: 1rem;"><summary style="cursor: pointer;">Ürünün stoğu güncel değil, sebebi nedir?</summary>
<br>Ürünün eMOSta stoğu yok iken, pazaryeri panelinde stoklu olması veya paneldeki stokların stok fiyat gönder görevi çalışmasına rağmen e-MOS'tan farklı olması ürünün pazaryerine bildirilmediği yani güncellenmediği anlamına gelmektedir.

Ürünün güncellenmemesinin sebebini tespit etmek için öncellikle log ekranı kontrol edilmelidir. İlgili ürün, log ekranında “İşleme alınan ürün”lerin arasında aratılmalıdır. Ürün pazaryerine bildiriliyor ancak bazı kurallara takılıp gönderilemiyorsa servisten uyarı mesajı döner ve log ekranına ürün ismi ile birlikte yansır.

Ürün “İşleme alınan ürün”lerin arasında değil ise ürün bildirilmiyor demektir. Bu durumda file log pasifse aktifleştirilmelidir. File log aktif edildikten sonra ürün üzerinde değişiklik yapılarak (Örneğin, açıklama alanında bir boşluk karakteri konulabilir) ürünün pazaryerine bildirilmesi için tetiklenmesi sağlanır. Sonrasında “Pazaryeri Ürün Stok Fiyat gönder” görevi çalıştırılır ve sunucuda pazaryeri loglarının bulunduğu klasöre gidilir. İlgili ürünün gönderilen ürünler arasında olup olmadığı kontrol edilir. Eğer ürün bu tetikleme sonrası bildirilmiş ve uyarı mesajı almış ise uyarı çözümlenmeye çalışılır. Alınan uyarı mesajı bilinmiyorsa ürünün request ve response dosyaları alınıp, müşterinin de CC’de yer aldığı bir mail ile ilgili pazaryerinin API Destek birimine iletilir veya müşterinin iletmesi için müşteriye gönderilir. API Destek biriminin yönlendirmeleri ile ürün gönderim sorununun çözümü için gerekli işlemler (tanımlama, seçim, onay vs) yapılır. Eğer uyarı dönmüyorsa veya ürün işleme alınmamışsa Backend ekibinde ilgili kişiye bilgi verilmelidir.

</details>

<details style="margin: 1rem;"><summary style="cursor: pointer;">Stoğu olmayan ürün satılabilmiş, sebebi nedir?</summary>
<br>Ürünün stoğu güncellenmediğinde satış gerçekleşebilir. Bu durumda öncelikle ürünün neden güncellenmediği tespit edilmelidir. Bunun için pazaryeri log ekranı kontrol edilmelidir. İlgili ürün, log ekranında “İşleme alınan ürün”lerin arasında ve “Karşılaştırma raporu”nda aratılmalıdır. İşleme alınan ürünlerin arasındaysa yanında bulunan uyarı mesajı incelenmelidir. Bu uyarı mesajı ürünün neden güncellenmediği bilgisini verir. Bu bilgi doğrultusunda ürün üzerinde gerekli düzeltmeler yapılıp bilgisi müşteriyle paylaşılmalıdır.

Bu tip durumların önüne geçmek için müşteri “Karşılaştırma raporu” loglarını incelemeli ve güncellenmeyen ürünleri takip etmelidir. Stoğunun güncellenmediğini tespit ettiği ürünleri “İşleme alınan ürün”lerin arasında aratıp uyarı mesajlarını okumalı ve bu uyarı mesajlarını dikkate almalı. Ürünün güncellenmesi için gerekli kriterlere sahip olmasını sağlamalı. </details>

<details style="margin: 1rem;"><summary style="cursor: pointer;">Ürünün pazaryeri kategorisi nasıl öğrenilir? </summary>
<br>Şu adımlar izlenmeli: Pazaryeri Tanımı > Pazar Yeri Ürünleri > Bu sayfada ilgili Pazaryeri: seçilir ve Ürün kodu kısmına ilgili ürünün kodu yazılır. Böylece ürünün pazaryeri kategori kodu <code>Paz.Kat.Kodu</code> ve pazaryeri kategori adı <code>Paz.Kat.Ad</code> alınır.</details>

<details style="margin: 1rem;"><summary style="cursor: pointer;">Ürün satış fiyatı maliyet fiyatından düşük olamaz” uyarısının sebebi nedir? </summary>
<br>Ürünün pazaryerine gönderilen satış fiyatı, maliyet fiyatının altında olduğu için ürün gönderilemiyor. Örneğin, Satış Fiyat: 237,12 - Maliyet: 237,15
<br>_Çözüm:_ Ürünün maliyet fiyatı ürün kartında bulunur ve manuel yönetilir. Müşteri ürünün fiyatı ile ilgili bu kurala uygun olarak ürün fiyatında veya maliyet fiyatında düzenleme yapmalıdır.</details>

<details style="margin: 1rem;"><summary style="cursor: pointer;">Log ekranında e-MOS'a aktarılmayan ve pazaryerinde olup e-MOS'ta olmayan sipariş uyarısı mevcut. Sebebi nedir?</summary>
<br>Pazaryerinden alınıp emosa işlenmeyen bir sipariş olduğunda bununla ilgili emosta tanımlanan ilgili kullanıcılara mail gönderilir. Mailde siparişin neden aktarılmadığı ve ürün kodu, barkodu belirtilir. Pazaryerinden sipariş alan görev her çalıştığında bu mail ilgili kişilere gönderilerek sorundan haberdar edilir. Aynı zamanda bu uyarı pazaryeri log ekranına da yazılır. Böyle bir sorunla karşılaşıldığında kontrol edilmesi gereken birkaç adım vardır:

- Siparişte geçen ürün kodunun & barkodun formatı emostaki ile aynı mı? Eğer aynı değilse ürün bildirimi yanlış gerçekleşmiştir. Bu durumda siparişin aktarımı için BE müdahele edebeilir ve müşteriye bilgisi verilerek ürünlerin doğru formatta göndeirlmesi için kontrol etmesi istenebilir.

- Siparişte geçen ürün kodunun & barkodun emosta stoğu var mı?Eğer stoğu yoksa sipariş emosa aktarılmaz, eğer varsa sorun stokla ilgili değildir.

- Siparişlte gelen il-ilçe datası ile emostaki il-ilçe tanımı uyuşuyor mu? Eğer uyuşmuyorsa buna uygun tanım yapılmalı.

- Gelen siparişin logu, başarılı gelen bir sipariş logu ile kıyaslanıp arada bir fark olup olmadığı incelenmeli.

- Yukardakı adımlara rağmen sorun tespit edilemiyorsa BE e bilgi verip debug edilmeli.</details>

<details style="margin: 1rem;"><summary style="cursor: pointer;">Pazaryerine gönderilirken hata alan ürünler nasıl listelenir?</summary>
<br>Pazaryeri ürünleri ekranında gönderim yapılırken servisten dönen uyarılar Ürün Uyarı kısmında belirtilir. Uyarı Metni arama alanında anahtar sözcük aratılarak ilgili kayıtlar ekrana getirilir ve excel’e aktarılabilir.</details>

<details style="margin: 1rem;"><summary style="cursor: pointer;">Pazaryeri kategori eşlemesi yapılmamış ürünler nasıl tespit edilir?</summary>
<br>Pazaryeri ürünleri ekranında filtreleme yapılarak eşlemesi yapılmayan ürünler bir excel'e aktarılabilir. <code>Paz.Kat.Kodu</code> alanının boş olması eşlemesinin yapılmadığı anlamına gelir.</details>

<details style="margin: 1rem;"><summary style="cursor: pointer;">Pazaryeri görevleri hata alıyor, sebebi nedir?</summary>
<br>X ürünün ürün kartında Gittigidiyor özellikleri kısmında, o ürünün bağlı olduğu pazaryeri kategorisi için GG servisinde geçerli olmayan bir spec girişi yapılmıştır. Ürün bu yüzden gönderilememektedir.
<br>_Çözüm:_ Job hatası varsa önce hata detayı incelenmeli. İlgili servisten ne mesaj döndüğü kontrol edilmeli. Örneğin servisin yanıt vermediği görülüyorsa bu ilgili pazaryerinin servisiyle alakalı durum olabilir. Aynı saatte aynı pazaryerini kullanan diğer müşterilerde de hata oluşmuş mu kontrol edilmeli. Sonrasında pazaryeri destek birimine email ileterek kullanılan servisi (görev linkini değil, o link çalıştığında çağrılan servisi product, stock and price, order gibi), varsa request ve response logu ile birlikte alınan hata mesajını sormak gerekir. Dönen yanıt doğrultusunda nasıl aksiyon alınması gerektiği netleştirilir. Pazaryeri tarafında sorun yoksa sorun Backend ekibine iletilir.

Örnek hata mesajı: Unable to connect to the remote server. (Pazaryeri kaynaklıdır, ilgili servislere erişilmediği anlamına gelir.)</details>

<details style="margin: 1rem;"><summary style="cursor: pointer;">Gittigidiyor</summary><br>Gittigidiyor pazaryeriyle ilgili sıkça sorulan sorular.<details style="margin: 1rem;"><summary style="cursor: pointer;">A isimli spec girişi zorunludur. Lütfen geçerli bir değer girişi yapınız uyarısının sebebi nedir?</summary><p style="padding-left: 30px;"><br>X ürününün bağlı olduğu kategoride A spec seçimi zorunlu olduğu halde bu spec seçilmemiştir.<br>_Çözüm:_ Spec tanımlı ise ürün kartında GG özelliklerinden A speci seçilir. Spec tanımlı değilse GG eşlemesi yapılmış kategorilerin özelliklerinin işlenmesi görevi çalıştırılır ve güncel speclerin servisten çekilmesi sağlanır. Bkz. 2.2.2.Pazaryeri için ürünün özelliklerin girilmesi</p></details><details style="margin: 1rem;"><summary style="cursor: pointer;">"A spec girişinde () Text; Combo ve Checkbox tipleri için geçersizdir. Uygun bir değer giriniz.” uyarısının sebebi nedir?</summary><p style="padding-left: 30px;"><br>X ürünün GG özellikleri arasında seçimi zorunlu olan A speci seçilmiş ancak GG servisinde tanımlı olmayan bir parametre seçilmiştir. Örneğin, X ürünü için GG özellikleri kısmında Renk başlığı altında tanımlı olan Mavi rengi seçilmiş, ancak GG servisinde Renk başlığı altında Mavi tanımlı olmadığı için hata alınmıştır.<br>_Çözüm:_ GG eşlemesi yapılmış kategorilerin özelliklerinin işlenmesi görevi çalıştırılır ve güncel parametrelerin servisten çekilmesi sağlanır. Güncel parametreler arasında uygun olan seçim yapılır, eğer uyarı dönmeye devam ediyorsa müşteri GG kategori yöneticisi ile iletişime geçip o spec için eksik olan parametrenin tanımlanmasını sağlar. Bu tanımlama yapıldıktan sonra parametre seçildiğinde hata alınmayacaktır.</p></details></details>
