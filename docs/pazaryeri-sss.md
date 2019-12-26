---
id: pazaryeri-sss
title: Sıkça Sorulan Sorular
---

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Ürünün stoğu güncel değil, sebebi nedir?</summary>
<br>Ürünün e-MOS'ta stoğu yok iken, pazaryeri panelinde stoklu olması veya paneldeki stokların stok fiyat gönder görevi çalışmasına rağmen e-MOS'tan farklı olması ürünün pazaryerine bildirilmediği yani güncellenmediği anlamına gelmektedir.

Ürünün güncellenmemesinin sebebini tespit etmek için öncellikle log ekranı kontrol edilmelidir.İlgili ürün, log ekranında “İşleme alınan ürün”lerin arasında aratılmalıdır.Ürün pazaryerine bildiriliyor ancak bazı kurallara takılıp gönderilemiyorsa servisten uyarı mesajı döner ve log ekranına ürün ismi ile birlikte yansır.

Ürün “İşleme alınan ürün”lerin arasında değil ise ürün bildirilmiyor demektir. Bu durumda file log pasifse aktifleştirilmelidir. File log aktif edildikten sonra ürün üzerinde değişiklik yapılarak (Örneğin, açıklama alanında bir boşluk karakteri konulabilir) ürünün pazaryerine bildirilmesi için tetiklenmesi sağlanır. Sonrasında “Pazaryeri Ürün Stok Fiyat gönder” görevi çalıştırılır ve sunucuda pazaryeri loglarının bulunduğu klasöre gidilir.İlgili ürünün gönderilen ürünler arasında olup olmadığı kontrol edilir. Eğer ürün bu tetikleme sonrası bildirilmiş ve uyarı mesajı almış ise uyarı çözümlenmeye çalışılır. Alınan uyarı mesajı bilinmiyorsa ürünün request ve response dosyaları alınıp, Firmanin de CC’de yer aldığı bir mail ile ilgili pazaryerinin API Destek birimine iletilir veya Firmanin iletmesi için Firmaya gönderilir. API Destek biriminin yönlendirmeleri ile ürün gönderim sorununun çözümü için gerekli işlemler (tanımlama, seçim, onay vs) yapılır. Eğer uyarı dönmüyorsa veya ürün işleme alınmamışsa Backend ekibinde ilgili kişiye bilgi verilmelidir.

</details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Stoğu olmayan ürün satılabilmiş, sebebi nedir?</summary>
<br>Ürünün stoğu güncellenmediğinde satış gerçekleşebilir. Bu durumda öncelikle ürünün neden güncellenmediği tespit edilmelidir. Bunun için pazaryeri log ekranı kontrol edilmelidir.İlgili ürün, log ekranında “İşleme alınan ürün”lerin arasında ve “Karşılaştırma raporu”nda aratılmalıdır.İşleme alınan ürünlerin arasındaysa yanında bulunan uyarı mesajı incelenmelidir. Bu uyarı mesajı ürünün neden güncellenmediği bilgisini verir. Bu bilgi doğrultusunda ürün üzerinde gerekli düzeltmeler yapılıp bilgisi Firmayle paylaşılmalıdır.

Bu tip durumların önüne geçmek için Firma “Karşılaştırma raporu” loglarını incelemeli ve güncellenmeyen ürünleri takip etmelidir. Stoğunun güncellenmediğini tespit ettiği ürünleri “İşleme alınan ürün”lerin arasında aratıp uyarı mesajlarını okumalı ve bu uyarı mesajlarını dikkate almalı.Ürünün güncellenmesi için gerekli kriterlere sahip olmasını sağlamalı.</details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Ürünün pazaryeri kategorisi nasıl öğrenilir? </summary>
<br>Şu adımlar izlenmeli: Pazaryeri Tanımı > Pazar Yeri Ürünleri > Bu sayfada ilgili Pazaryeri: seçilir ve Ürün kodu kısmına ilgili ürünün kodu yazılır. Böylece ürünün pazaryeri kategori kodu <code>Paz. Kat. Kodu</code> ve pazaryeri kategori adı <code>Paz. Kat. Ad</code> alınır.</details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Ürün satış fiyatı maliyet fiyatından düşük olamaz” uyarısının sebebi nedir? </summary>
<br>Ürünün pazaryerine gönderilen satış fiyatı, maliyet fiyatının altında olduğu için ürün gönderilemiyor.Örneğin, Satış Fiyat: 237, 12 - Maliyet: 237, 15
<br>**_Çözüm:_** Ürünün maliyet fiyatı ürün kartında bulunur ve manuel yönetilir. Firma ürünün fiyatı ile ilgili bu kurala uygun olarak ürün fiyatında veya maliyet fiyatında düzenleme yapmalıdır.</details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Log ekranında e-MOS'a aktarılmayan ve pazaryerinde olup e-MOS'ta olmayan sipariş uyarısı mevcut. Sebebi nedir?</summary>
<br>Pazaryerinden alınıp e-MOS'a işlenmeyen bir sipariş olduğunda bununla ilgili e-MOS'ta tanımlanan ilgili kullanıcılara mail gönderilir. Mailde siparişin neden aktarılmadığı ve ürün kodu, barkodu belirtilir. Pazaryerinden sipariş alan görev her çalıştığında bu mail ilgili kişilere gönderilerek sorundan haberdar edilir. Aynı zamanda bu uyarı pazaryeri log ekranına da yazılır. Böyle bir sorunla karşılaşıldığında kontrol edilmesi gereken birkaç adım vardır:

- Siparişte geçen ürün kodunun & barkodun formatı e-MOS'taki ile aynı mı? Eğer aynı değilse ürün bildirimi yanlış gerçekleşmiştir. Bu durumda siparişin aktarımı için BE müdahele edebeilir ve Firmaya bilgisi verilerek ürünlerin doğru formatta göndeirlmesi için kontrol etmesi istenebilir.

- Siparişte geçen ürün kodunun & barkodun e-MOS'ta stoğu var mı? Eğer stoğu yoksa sipariş e-MOS'a aktarılmaz, eğer varsa sorun stokla ilgili değildir.

- Siparişlte gelen il-ilçe datası ile e-MOS'taki il-ilçe tanımı uyuşuyor mu? Eğer uyuşmuyorsa buna uygun tanım yapılmalı.

- Gelen siparişin logu, başarılı gelen bir sipariş logu ile kıyaslanıp arada bir fark olup olmadığı incelenmeli.

- Yukardakı adımlara rağmen sorun tespit edilemiyorsa BE e bilgi verip debug edilmeli.</details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Pazaryerine gönderilirken hata alan ürünler nasıl listelenir?</summary>
<br>Pazaryeri ürünleri ekranında gönderim yapılırken servisten dönen uyarılar Ürün Uyarı kısmında belirtilir. Uyarı Metni arama alanında anahtar sözcük aratılarak ilgili kayıtlar ekrana getirilir ve excel’e aktarılabilir.</details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Pazaryeri kategori eşlemesi yapılmamış ürünler nasıl tespit edilir?</summary>
<br>Pazaryeri ürünleri ekranında filtreleme yapılarak eşlemesi yapılmayan ürünler bir excel'e aktarılabilir.<code>Paz. Kat. Kodu</code> alanının boş olması eşlemesinin yapılmadığı anlamına gelir.</details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Pazaryeri görevleri hata alıyor, sebebi nedir?</summary>
<br>X ürünün ürün kartında Gittigidiyor özellikleri kısmında, o ürünün bağlı olduğu pazaryeri kategorisi için GG servisinde geçerli olmayan bir spec girişi yapılmıştır.Ürün bu yüzden gönderilememektedir.
<br>**_Çözüm:_** Job hatası varsa önce hata detayı incelenmeli.İlgili servisten ne mesaj döndüğü kontrol edilmeli.Örneğin servisin yanıt vermediği görülüyorsa bu ilgili pazaryerinin servisiyle alakalı durum olabilir. Aynı saatte aynı pazaryerini kullanan diğer Firmalerde de hata oluşmuş mu kontrol edilmeli. Sonrasında pazaryeri destek birimine email ileterek kullanılan servisi (görev linkini değil, o link çalıştığında çağrılan servisi product, stock and price, order gibi), varsa request ve response logu ile birlikte alınan hata mesajını sormak gerekir. Dönen yanıt doğrultusunda nasıl aksiyon alınması gerektiği netleştirilir. Pazaryeri tarafında sorun yoksa sorun Backend ekibine iletilir.

Örnek hata mesajı: Unable to connect to the remote server.(Pazaryeri kaynaklıdır, ilgili servislere erişilmediği anlamına gelir.)</details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Gittigidiyor soruları</summary><br>Gittigidiyor pazaryeriyle ilgili sıkça sorulan sorular.

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">A isimli spec girişi zorunludur. Lütfen geçerli bir değer girişi yapınız uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>X ürününün bağlı olduğu kategoride A spec seçimi zorunlu olduğu halde bu spec seçilmemiştir.<br>**_Çözüm:_** Spec tanımlı ise ürün kartında GG özelliklerinden A speci seçilir. Spec tanımlı değilse GG eşlemesi yapılmış kategorilerin özelliklerinin işlenmesi görevi çalıştırılır ve güncel speclerin servisten çekilmesi sağlanır.</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">"A spec girişinde () Text; Combo ve Checkbox tipleri için geçersizdir. Uygun bir değer giriniz.” uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>X ürünün GG özellikleri arasında seçimi zorunlu olan A speci seçilmiş ancak GG servisinde tanımlı olmayan bir parametre seçilmiştir.Örneğin, X ürünü için GG özellikleri kısmında Renk başlığı altında tanımlı olan Mavi rengi seçilmiş, ancak GG servisinde Renk başlığı altında Mavi tanımlı olmadığı için hata alınmıştır.<br>**_Çözüm:_** GG eşlemesi yapılmış kategorilerin özelliklerinin işlenmesi görevi çalıştırılır ve güncel parametrelerin servisten çekilmesi sağlanır. Güncel parametreler arasında uygun olan seçim yapılır, eğer uyarı dönmeye devam ediyorsa Firma GG kategori yöneticisi ile iletişime geçip o spec için eksik olan parametrenin tanımlanmasını sağlar. Bu tanımlama yapıldıktan sonra parametre seçildiğinde hata alınmayacaktır.</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">A geçersiz bir spec ismidir. Lütfen bu kategoriye uygun spec girişi gerçekleştiriniz. Uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>X ürünün ürün kartında Gittigidiyor özellikleri kısmında, o ürünün bağlı olduğu pazaryeri kategorisi için GG servisinde geçerli olmayan bir spec girişi yapılmıştır. Ürün bu yüzden gönderilememektedir.<br>**_Çözüm:_** Geçersiz olduğu uyarısı verilen spec seçimi kaldırılmalıdır. </p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Geçersiz model değeri uyarısının sebebi nedir? </summary><p style="padding-left: 30px; "><br>Model kavramı ürüne karşılık gelmektedir. X ürünü için hiç spec girişi yapılmadığı anlamına gelmektedir.<br>**_Çözüm:_** GG eşlemesi yapılmış kategorilerin özelliklerinin işlenmesi görevi çalıştırılır ve ürün kartına gelen özellikler seçilir. Uygun özellik seçimi yapıldığında uyarı dönmeyecektir.</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Model bilgilerini sıralı bir şekilde eksiksiz gönderiniz uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>Model kavramı ürüne karşılık gelmektedir. X ürünü için ürün kartında Gittigidiyor özellikleri arasında seçimi yapılmayan specler ve eksik bilgiler vardır.<br>**_Çözüm:_** Ürün kartında bulunan özellikler seçilir. Uygun özellik seçim yapıldığında uyarı dönmeyecektir.</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Tekrarlanan varyant bilgileri tespit edildi. Lütfen ürüne ait benzer varyant bilgisi girmediğinizen emin olunuz” uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>İlgili ürünün bulunduğu kategoride GG tarafında beden/numara/yaş spec'i olmadığı için veya e-MOS'ta tanımlı spec parametresi ile GG tarafındaki parametre uyuşmadığından uyarı döner. Örneğin; e-MOS'ta XXL olarak tanımlı beden var iken ürünün bağlı olduğu kategoride 2XL beden tanımlanmış olabilir. Bu durum file log incelenerek gönderilen ürün datasından anlaşılabilir.<br>**_Çözüm:_** Firma ürünün bulunduğu pazaryeri kategori kodunu, kategori yöneticisi ile paylaşıp Beden/Numara/Yaş isimli bir spec yoksa açılması gerektiğini iletmeli, eğer varsa uygun parametre için tanım yapılması gerektiği iletmeli. (Ör; ABC kategorisindeki beden spec'i için XXL parametresinin tanımlanması).</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Girdiğiniz model özellikleri içerisinde ürün özelliği olarak atadığınız specler mevcut” uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>Ürünün hem spec kısmında hem de variant kısmında aynı spec'in gönderilmesi sebebi ile ilgili uyarı mesajı alınmaktadır.<br>**_Çözüm:_** Varyantlı/Seçenekli olan ürünlerde Beden/Numara/Yaş spec seçimi kaldırılmalıdır. Örneğin, seçeneği (numaraları) olan bir ayakkabı ürünü için ürün kartındaki GG spec kısmında Numara seçilmemelidir. Çünkü seçenekleri/numaraları zaten gönderilmektedir.</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Spec ve başlık tanımlamaları konusunda firmaya ve tarafımıza düşen görevler nelerdir?</summary><p style="padding-left: 30px; "><br>1- Firma loglarda eksik veya tanımsız spec uyarısı gördüğü tüm ürünleri kontrol edip yukarıdaki bilgiler doğrultusunda gerekli seçimleri yapmalı. Eğer uygun bilgilerini göremiyorsa, ilgili görev çalıştırılmalı.<br>2- Görev çalıştığında e-MOS'a çekilen güncel spec ve parametreleriyle birlikte Firmanin ilgili bilgileri görüyor olması beklenmektedir. Eğer ürün için gerekli bilgiyi hala görmüyorsa (Örn; Durum başlığı altında “Sıfır” görülmüyor) Firma bu eksik bilgileri toplayıp GG Kategori yöneticisi ile paylaşmalı. Böylece GG gerekli bilgileri açacak veya tanımlayacaktır. </p></details>

</details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Trendyol soruları</summary><br>Trendyol pazaryeriyle ilgili sıkça sorulan sorular.

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Barkod alanı hatalı uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>İlgili ürünün barkod alanı boş olduğu için ürün gönderiminde hata alınmaktadır.<br>**_Çözüm:_** Firmaya barkod alanını doldurması gerektiği bilgisi verilmelidir.</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Zorunlu kategori özellik bilgisi eksiktir. Eksik alan: X uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>İlgili ürünün bağlı olduğu kategoriye ait zorunlu özellik bilgisi boş olduğu için ürün gönderiminde hata alınmaktadır. Örneğin; Cinsiyet.<br>**_Çözüm:_** Firmaya X alanını doldurması gerektiği bilgisi verilmelidir. Özellik seçimi yapıldıktan sonra ürün stok fiyat gönder görevi tetiklenmelidir.</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Beden için kategori özellik değeri geçerli değildir uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>İlgili ürünün bağlı olduğu kategoriye ait Beden özelliğinin altında uyarı alan ürünün beden/seçenek formatı Trendyol tarafında tanımlı olmadığı için veya e-MOS'ta Ürün seçenek tanım ekranında ilgili beden parametresinde geçersiz karakter bulunduğu için ürün gönderiminde hata alınmaktadır.<br>**_Çözüm:_** Sorunun Trendyol’da tanımlı olup olmadığını anlamak için Postman üzerinden ürünün bağlı olduğu kategori için o beden parametresi kontrol edilir. Eğer tanımlı değilse Firmaya bilgisi verilerek, Trendyol kategori yöneticisi ile iletişime geçmesi ve parametrenin tanımlanmasını sağlamalıdır.<br><br>İstek yapılacak servis ve detaylarına Trendyol API Döküman linkinden ulaşılabilir.<br>https://developers.trendyol.com/tr/urun-entegrasyonu/v2/trendyol-kategori-ozellik-bilgileri<br><br>Eğer tanımlı olduğu halde bu hata dönüyorsa e-MOS'taki tanımında sorun olabilir. Ürün seçenek tanım ekranında ilgili parametrede geçersiz karakter (sonunda boşluk olması gibi) olmadığından emin olmak gerekir. Buna rağmen hata alınıyorsa backend ekibine iletilip, debug edilerek sorun gözlemlenmelidir.</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Açıklama alanı boş olmamalıdır.</summary><p style="padding-left: 30px; "><br>Trendyol’a gönderilen ürünün açıklama alanı boş olmamalıdır. Aksi durumda hata alır, ürün gönderilemez. </p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Barkodlu ürün bulunamadı uyarısının sebbei nedir? </summary><p style="padding-left: 30px; "><br>Stok fiyat güncellerken iki metot kullanılmaktadır check metodu pazaryeri ve e-MOS'taki stokları alıp karşılaştırıp farklı olanları update etmektedir.  Stock and price görevi çalıştırıldığı zaman ürünün stok ve fiyatı güncellenmeye çalışılır. Eğer ürün pazaryerinde yoksa bu uyarı dönmektedir. Yani bu uyarı ürünün pazaryerinde olmadığı anlamına gelir. Bu durumda ürünün neden pazaryerine gönderilmediği kontrol edilmelidir.</p></details></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">N11 soruları</summary><br>N11 pazaryeriyle ilgili sıkça sorulan sorular.

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Bu ürün üzerinde işlem yapamazsınız uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>N11 ilgili ürün için bir işlem yapılmasına izin vermiyor.<br>**_Çözüm:_** Firma bu uyarıyı aldığı ürünler için N11 kategori yöneticisi ile iletişime geçmeli.</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Zorunlu olan özellikleri ürün özellikleri kısmında ve/veya sku özellikleri kısmında girmeniz gerekmektedir. Özellik Adı: A, Özellik ID:  uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>N11 için ürünün zorunlu özellikleri eksik girilmiştir.<br>**_Çözüm:_** N11 eşlemesi yapılmış kategorilerin özelliklerinin işlenmesi görevi çalıştırılır ve ürün kartına gelen özellikler seçilir. Uygun özellik seçimi yapıldığında uyarı dönmeyecektir.</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Satıcı stok kodu başka bir ürününüzde kullanılmaktadır uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>Firma X ürününde başka bir üründe kullanılan barkodu girmişse, N11 barkodun başka bir üründe kullanıldığına dair uyarı mesajı verir ve güncellemeye izin vermez.</p></details></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Hepsiburada soruları</summary><br>Hepsiburada pazaryeriyle ilgili sıkça sorulan sorular.

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Product not found uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>Hepsiburada paneline henüz yüklenmemiş/açılmamış bir ürüne e-MOS'ta pazaryeri onayı verilmişse, HB stok fiyat gönder görevi çalıştığında o ürünü Hepsiburada tarafında bulamadığı için bu uyarı döner. <br>**_Çözüm:_** Firma ilgili ürünü HB paneline yüklemeli/açmalı, eğer açılması istenmiyorsa e-MOS'ta ürünün Hepsiburada onayı kaldırılmalı.</p></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Stok-fiyat güncelleme görevi çalıştığında bazı ürünlerde “DiscountedListingPriceIncrease” uyarısı dönüyor. Sebebi nedir?</summary><p style="padding-left: 30px; "><br>Ürünlerde HB tarafında kampanya olduğu için gönderilen fiyat, indirim süresince geçerli değerden daha yüksek olduğundan fiyatı güncellenmiyor.<br>**_Çözüm:_** Firmaya bu bilgi verilmeli ve HB entegrasyon tarafına mail atılarak teyit edilmeli. Kampanya Firma ve HB tarafında yönetilir.</p></details></details>

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">ePttAVM soruları</summary><br>ePttAVM pazaryeriyle ilgili sıkça sorulan sorular.

<details style="margin: 1rem; "><summary style="cursor: pointer; font-size: 16px; ">Input string was not in a correct format uyarısının sebebi nedir?</summary><p style="padding-left: 30px; "><br>ePttAVM'ye ürün göndermek için ürünün ePttAVM tarafında uygun bir kategori ile eşleşmesi zorunludur. ePttAVM kategorisi ile eşleşme yapılmadığında bu hata alınır.<br>**_Çözüm:_** Firma gerekli kategori eşlemesini yapması gerektiği konusunda bilgilendirilir.</p></details>


</details>
