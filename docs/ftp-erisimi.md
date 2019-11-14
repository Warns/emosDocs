---
id: ftp-erisimi
title: FTP Erişimi
---

e-MOS kullanılmaya başlanmadan önce verilen FTP bilgileri ile siteye özel **images, languages, printerFiles, styles, upload** FTP klasörlerine ulaşılabilmektedir.

FTP ile erişilebilecek klasörler aşağıda açıklanmıştır;

|Klasör Adı|Açıklama|
|--|--|
|images|Sitenin önyüz grafik tasarımı için kullanılan resimlerin bulunduğu klasördür|
|languages|Sitede bulunan sabit metinlerin <code>.txt</code> dosyaları halinde bulunduğu klasördür. Bütün sabit metinler bu .txt</code> dosyaları içerisinden güncellenebilir. Eğer site çoklu dil destekli olarak açıldıysa başka dillere çevirilebilir. Örneğin <code>tr-TR</code> alt klasörü türkçe sabit metinleri, <code>en-EN</code> alt klasörü ingilizce metinleri belirler. Eğer bir sabit metin bilgisinin <code>ID</code> si, bu dosyalarda yer almıyor ise, yazılım tarafındaki öndeğer karşılığı gösterilir. Sabit metinlerin <code>ID</code> si  <code>lbf_</code> öneki ile başlamaktadır. Herhangibir sabit metnin ID sini bulmak için ilgili sayfa internet tarayıcısında açıldıktan sonra kaynak koduna bakarak bulunabilir|
|printerFiles|Sistemden kesilen matbu evraklardan nokta vuruşlu olanların <code>.txt</code> dosyaları şeklinde biriktirildiği klasördür|
|styles|Sitenin ön yüz görüntüsünün düzenlenebildiği .css dosyalarını içeren klasördür|
|upload|Sistemde sıkça kullanılacak olan **Resim / Dosya Yükleme** modülü sadece bu klasöre ve alt klasörlerine erişebilir.

<br>
Styles klasöründe <code>genel.css</code> <code>icerik.css</code> <code>kutu.css</code> <code>popup.css</code> <code>sayfa.css</code> <code>urun.css</code> <code>ajaxtabs.css</code> <code>dhtmlwindow.css</code> ve <code>rating.css</code>  dosyları bulunmaktadır. Bu dosyalar yardımı ile sitenin görsel öğeleri tasarlanabilmektedir.

styles klasörünün kullanımı;

|Dosya Adı|Açıklama|
|--|--|
|genel.css|Sitedeki genel nesnelerin tasarlandığı kısımdır. Genel sayfa yerleşimi, Butonlar, linkler, inputlar, label ve radio lar bu bölümden tasarlanır.|
|icerik.css|Admin panelinden sıkça kullanılan HTML editörünün içerisinde yer alan ve genel font - renk stillerinin seçilebildiği style listbox ının içine dolacak css bilgilerinin belirlendiği dosyadır.|
|kutu.css|En çok satanlar, sepet, yeni ürünler, üye login, anket, duyuru, kampanya, paket ürünler, arkadaş tavsiyesi, arama, chat, e-bülten, hızlı yardım kutularının tasararlandığı css dosyasıdır.|
|popup.css|Favori ürünlerime ekle, stoğa gelince haber ver, indirime girince haber, vb. durumlarda açılan ve ekranın ortasına yerleşen yeni pencerenin tasarımının yapıldığı dosyadır.|
|sayfa.css|Önyüzde açılan tüm sayfaların (sepet, üye sayfaları, favori ürünlerim, satınalma adımları, anket sonuçları, vb) tasarımlarının yapıldığı css dosyasıdır.|
|urun.css|Ürün liste (vitrin ürünler, yeni ürünler, ençok satan ürünler, kategori ürünleri), ürün detay, promosyon ürünler, paket ürünler sayfalarındaki ürün dizilişlerinin tasarlandığı css dosyasıdır.|
|ajaxtabs.css|Ürün detay sayfasında "Sayfa Yerleşim Düzenleme" ekranından (Ürün Detay) sürükle bırak modülünde Tab1, Tab2, ....., Tab7 seçeneklerinden en az biri seçildiğinde ortaya çıkan Tab gösterim modülünün tasarlandığı css dosyasıdır.|
|dhtmlwindow.css|Popup olarak açılan sayfaların genel tasarımının yapıldığı css dosyasıdır.|
|rating.css|Ürün rating modülünün tasarlandığı dosyadır.|

<br>
languages klasörünün kullanımı;

Bu klasörün altındaki .txt dosyaları kullanılarak sitenin ön yüzü farklı dillere çevirilebilmektedir.

>❗️ _Ayrıca **siteBilgileri.txt** dosyası kullanılarak sitenin <code>TITLE</code> <code>META TAG</code> <code>ICON</code>** vb.. bilgiler her sayfaya eklenecek şekilde düzenlenebilmektedir._


**SiteMap Oluşturma**
SiteMap dosyaları **Google, Yahoo ve BING** gibi arama motorlarının, sitenin içeriğini daha doğru ve kolay indeksleyebilmesi için hazırlanır. Oluşturulan sitemap dosyaları "UPLOAD/sitemap" klasörü altına yerleştirilir.

>❗️ _Arama motorlarının bu dosyaları görebilmeleri için dosyaların ilgili arama motorlarına tanımlanmış olması gerekmektedir. 
**Örnek:** https://www.google.com/webmasters/tools/home?hl=en 
Örnekteki linkin çalışması için "Google Search Console"'a login olmanız gerekir._

