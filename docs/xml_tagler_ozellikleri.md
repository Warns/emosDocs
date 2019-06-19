####Sayfalara Göre Kullanılan Ön Ekler ve Tanımı:

|Ön Ekler|Açıklama|Örnek|
|--|--|--|
|S1|Tüm sayfalarda tekil kayıtları getiren kısım için kullanılmaktadır.|Örneğin; Ürün detay, Sepet sayfasında sepetin toplamı vs.|
|S2|Ürün liste XML tag'i içerisinde, ürün liste sayfalarında kullanılmaktadır.|Örneğin; Ürün Liste, Sipariş Sonuç Liste ve Sepetim Ürün Liste gibi.|
|S3|Ürün özellik XML tag'i içerisinde ürün özelliklerini getirmek için kullanılmaktadır.|Sadece Ürün Detay sayfasında kullanılabilir.|
|S4|Banner XML tag'i içerisinde banner bilgilerini getirmek için kullanılmaktadır|Tüm sayfalarda kullanılabilir.|
|S5|Sayfa hiyerarşi XML tag'i içerisinde hiyerarşi bilgisini getirmek için kullanılmaktadır.||

**Not:** “s1” ön ekiyle başlayan parametreleri kullanabilmek için herhangi bir XML tag’i bilgisine gerek yoktur. İlgili sayfada doğrudan kullanılabilir.

####Sayfalara Göre Kullanılabilecek XML Tagleri ve Özellikleri:

Sistem XML tagları “emos” öneki ile başlamaktadır. Ürün Detay, Anasayfa, Sepet(Toplam tutar v.s.), Sipariş Sonuç(Siparişin toplam tutarı, üye bilgileri vs.) gibi tekil kayıt kullanılan sayfalarda parametreler “s1” öneki ile başlamaktadır. Bu sayede diğer parametreler ile karışması engellenmektedir. Örnek: “$s1_UYEAD$”. Çoklu işlemlerde(ürün liste, banner liste v.s.) veri filtreleme, sıralama, ayırma işlemleri yapabilmek için kullanılan bazı parametreler bulunmaktadır.


####Bu parametreler ve kullanım şekilleri aşağıdaki gibidir; 

**sort:** Sıralama yapmak için kullanılan XML attribute’dir. Virgül ile birden fazla alan üzerinden sıralama yapılabilir. 
**Kullanım şekli:** “ < xmlTagAdi sort=”PARAMETRE_ADI ” >içerik< /xmlTagAdi > ” 
**Örnek 1:** < emosProds sort=” URNAD ” >İçerik< / emosProds >
**Çıktı:** Ürün adına göre artan şekilde sıralama yapan tag'dir.
**Örnek 2:** < emosProds sort=” URNAD, URNID DESC ” >İçerik< / emosProds>
**Çıktı:** Ürün adına göre artan, Ürün ID bilgisine göre azalan şekilde sıralama yapacaktır.
**filter:** Çoklu kayıtlar üzerinde filtreleme yapabilmek için kullanılan XML attribute’dir. SQL syntax yapısı üzerinden koşula göre data getirilmesi sağlanabilir. 
**Kullanım şekli:** “ < xmlTagAdi filter=” PARAMETRE_ADI = DEGER ” >içerik< / xmlTagAdi > ” 
**Örnek 1:** < mosProds filter= ” URNID < > 15 ” > $s2_URNAD$ < / emosProds >
**Çıktı:** Ürün ID bilgisi 15’e eşit olmayan ürünleri listeleyecektir.
**delimiter:** Çoklu kayıtlar üzerinde otomatik ayraç koymak için kullanılan parametredir. 
**Örnek 1:** < emosProds delimiter= ”,” >$s2_URNAD$< / emosProds >
**Çıktı:** Ürün adları aralarına “,” karakteri konularak listelenecektir
**rowIndex:** Aktif olan satırın numarasını döndürür. Kullanıldığı XML tag’ine göre ön ek alır. 
**Örnek(Ürünler için):** < emosProds delimiter= ”;” >$s2_rowIndex$, $s2_URNAD$< / emosProds >
**Çıktı:** 5 adet ürün var ise, “1, URUN1 2;URUN2;3, URUN3;4, URUN4;5, URUN5” şeklinde bir çıktı verecektir.
**Örnek(Ürünler için):** < emosBanners delimiter=”;” >$s4_rowIndex$, $s4_BNRAD$< / emosBanners >
**Çıktı:** 5 adet banner var ise, “1, BNR1; 2, BNR2; 3,BNR3; 4, BNR4; 5, BNR5” şeklinde bir çıktı verecektir.
**rowCount:** Döndürülerek toplam kayıt sayısı belirleyebilmek için kullanılan parametredir. 
**Örnek1:** Toplamda 10 adet ürün olduğunu varsayarak; < emosProds rowCount=”5” >$s2_URNAD$< / emosProds >
**Çıktı:** İlk 5 ürünün ürün adlarını ekrana yazdırır.
**Örnek2:** Toplamda 15 adet ürün olduğunu varsayarak; < emosProds rowCount=”7” sort= ”URNAD DESC” >$s2_URNAD$< / emosProds>
**Çıktı:** Ürün isimlerini azalan sırada filtreleyerek ilk 7 ürünün ürün adları ekrana yazdırır.
**Örnek3:** Toplamda 5 adet ürün olduğunu varsayarak; < emosProds rowCount=”2” sort= ”URNID DESC” filter= ”URNID <> 5” >$s2_URNAD$< / emosProds>
**Çıktı:** Ürün ID bilgisine göre azalan sırada ve ürün ID bilgisi “5” e eşit olmayan ürünler arasından filtreleyip ilk 2 ürünün ürün adları ekrana yazdırır.

####Kullanılabilecek xml tagları aşağıdaki gibidir;

**“< emosProds >”:** Ürünleri listelemek için kullanılan XML tag’idir. Parametre ön eki “s2” dir. Ürün liste bilgisinin yer aldığı sayfalarda kullanılabilir.(Ürün Liste, Sipariş Sonuç Ürün Listesi, Sepet). Yukarıda belirtilen filtreleme, sıralama, ayırma özellikleri bu tag üzerinde kullanılabilir. 
**Örnek:** “ < emosProds sort=”URNID” delimiter=”;”>$s2_URNAD$< emosProds > ”
**Çıktı:** Artan şekilde URNID kolonuna göre sıralama yaparak, ürünleri “;” karakteri ile ayırarak ürün adlarını listeleyecektir.
“< emosSpecs >” Ürün özelliklerini listelemek için kullanılan XML tag’idir. Parametre ön eki “s3“ dir. Sadece Ürün Detay sayfasında kullanılabilir. Yukarıda belirtilen filtreleme ve sıralama, ayırma özellikleri kullanılabilir.
**Örnek 1:** < emosSpecs filter=”OPRAD <> ‘A’ ”>$s3_OPRAD$< /emosSpecs >
**Çıktı:** OPRAD bilgisi “A” karakterine eşit olamayan özelliklerin adlarını listeleyecektir.
**“< emosBanners >”:** Bannerları listelemek için kullanılan XML tag’idir. Parametre öneki “s4” dir. Tüm sayfalara ek olarak “Header İçerik” ve “Footer İçerik” bölümlerinde kullanılabilir. Yukarıda belirtilen filtreleme ve sıralama, ayırma attributeleri bu tag üzerinde kullanılmaktadır.
**Örnek:** “< emosBanners sort=”BNRAD”>$s4_BNRAD$< /emosBanners >”
**Çıktı:** BNRAD kolonuna göre artan şekilde sıralama yaparak bannerlar listelenecektir.
**“< emosPageHierarchy >”:** Sayfa hiyerarşi bilgisinin listelemek için kullanılan XML tag’idir. Parametre ön eki “s5” tir. Yukarıda belirtilen filtreleme ve sıralama, ayırma özellikleri kullanılabilir.
**Örnek:** “< emosPageHierarchy sort=”BNRAD”>$s4_BNRAD$< /emosPageHierarchy >”
**Çıktı:** BNRAD kolonuna göre artan şekilde sıralama yaparak bannerlar listelenecektir.
**“< emosFormat >”:** 
String değiştirme, html encode v.s. gibi işlemler için kullanılan XML tag’idir. Varsayılan ayıraç “|” dir. Bulunulan XML tag’i içerisindeki parametre ön eki kullanılır. Farklı bir ayıraç kullanılmak isteniyorsa attribute olarak “seperator” özelliği kullanılabilir. Bu XML tag’i üzerinde kullanılabilecek özellikler aşağıdaki gibidir;

r**eplace:** Belirli bir string’i başka bir string e değiştirmek için kullanılır. Birden fazla değiştirme işlemi yapılacaksa aralarına “|” işareti eklenir.

**Örnek 1:** “< emosFormat replace=”abc=bca”>abc123< /emosFormat >”
**Çıktı:** “bca123”
**Örnek 2:**“< emosFormat replace=”123=55|abc=a”>abc123< /emosFormat >”
**Çıktı:** “abc55”
**Örnek 3:**“< emosFormat > seperator=”;”
**Çıktı:** “a55”
**Örnek 4:**“< emosProds>< emosFormat replace=”;=$” >$s2_URNAD$< /emosFormat >< /emosProds >”
**Çıktı:** Ürün adlarındaki “;” değerini “$” değerine değiştirerek ürün adlarını listeleyecektir.
**onlyEng:** Belirli bir string’i türkçe karakterlerden arındırmak için kullanılır.Değer olarak “true” ya da “1” set edilmelidir.

**Örnek 1:** “< emosFormat onlyEng=”true” >Ürün 1< /emosFormat >”
**Çıktı:** “Urun 1”
**Örnek 2:**“< emosFormat onlyEng=”1” >Türkçe içerik< /emosFormat >”
**Çıktı:** “Turkce icerik”

**encodeDecode:** Belirli bit string’i “Html Encode/Decode”, “Url Encode/Decode”, “Javascript Encode”, “Html Attribute Encode” etmek için kullanılır.

**Örnek1(html encode):** “< emosFormat encodeDecode=”html=encode” >&< /emosFormat >”
**Çıktı:** & ;
**Örnek2(html decode):**“< emosFormat encodeDecode=”html=decode” >&< /emosFormat >”
**Çıktı:** &
**Örnek3(urn encode):**“< emosFormat encodeDecode=”urn=encode” >&< /emosFormat >”
**Çıktı:** %26
**Örnek4(javascript encode):** “< emosFormat encodeDecode=”javascript=encode” > text $$a< /emosFormat >”
**Çıktı:** text%20%24%24a
**Örnek5*html attribute encode):** “< emosFormat encodeDecode=”htmlattribute=encode”>İçerik< /emosFormat >”

**format:** Belirli bir string’i formatlamak için kullanılır.(Örn. Para formatı). Kullanım şekli “ format=”(d(double)/i(int)/s(string)/b(bool))={0:format}” “ dir.

**Örnek:** “< emosFormat format=”d={0:0,00}”>85< /emosFormat >”
**Çıktı:** 85,00
seperator: replace, encode decode v.s. gibi attributeler için birden fazla yapılması gereken işlemlerde ayıracın ne olması gerektiğini belirlemek için kullanılır.

**Örnek:** “< emosFormat seperator=”;” replace=”a=b;b=c” >a< /emosFormat >”
**Çıktı:** c
