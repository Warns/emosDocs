---
id: fiyat-tipi-tanimi
title: Fiyat Tipi Tanımı
---

Fiyat tipi tanımı ile e-MOS üzerinde kullanıcı segmenti bazlı bir çok özelleştirme işlemi yapılabilmektedir. Aynı zamanda hediye kuponu ve kampanya tanımı da önceden belirlenen bir fiyat tipini göre çalışabilmektedir. Çeşitli kullanıcı gruplarına farklı farklı tipteki kampanyalardan yararlanma olanağını sunar.

Yeni bir fiyat tipi tanımı oluşturma için **Ekle** butonu kullanılır. Açılan sayfada bulunan alanlarla ilgili detaylar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Fiyat Tipi|Tanımlamak istediğiniz fiyat tipinin adının girildiği alandır.|
|Ref Fiyat Tipi|Yeni oluşturulacak olan fiyat tipinin referans olarak çalıştığı fiyat tipinin seçildiği alandır.<br>❗️ _Genel kullanım olarak sistem üzerinde default olarak bulunan Perakende fiyat tipi bu alanda kullanılır._|
|ESI KOD|Aynı sistem üzerinde çalışan 2 farklı site için kullanılan bir tanımlayıcıdır "Unique Identifier". |
|İndirim|Bu fiyat tipiyle yapılan alışverişlerde direkt olarak uygulanacak indirim oranı.|
|Üye Bonus kazandırma Oranı (Peşin Ödeme)|Bu fiyat tipiyle yapılan alışverişlerde peşin ödemelerde kazanılacak bonus oranı.|
|Tavsiye Bonus Kazanma Oranı|Arkadaş tavsiyesinde kazanılacak bonus oranı|
|Havale İndirim Oranı|Havale ödemelerde uygulanacak indirim oranı.|
|Kapıda Ödm. İndirim Oranı|Kapıda ödemelerde uygulanacak indirim oranı.|
|Ent. Kodu|Bu fiyat tipi bir entegrasyona bağlı olarak çalıştığı durumlarda kullanılacak olan entegrasyon ID'sinin girildiği alandır.|
|Min. Teklif Limiti|İlgili fiyat tipindeyken sepette teklif vermek mödülü için kullanılan alandır.<br><br>❗️ _Bu yapı genellikle B2B için kullanılmaktadır._  | 
|Artış|Referans fiyat tipi seçildiği durumda referansın üzerine artış veya azalışa karşılık gelmektedir.|
|Üye Bonus kazandırma Oranı (Taksitli Ödeme)|Bu fiyat tipiyle yapılan alışverişlerde taksitli ödemelerde kazanılacak bonus oranı.|
|Tavsiye Bonus Kazanma Süresi|Arkadaş tavsiyesinde bonus kazanma süresini belirleyen alandır.|
|Üye Bonus kazandırma Oranı (Banka Bonus)|Arkadaş tavsiyesinde banka bonus kazanma tutarını belirleyen alandır.|
|Kdv Gösterim Şekli|İlgili fiyat tipine bağlı ürünlerin KDV dahil veya KDV hariç olarak gösterilmesi için kullanılır.|
|Ürün PB Gösterimi|Para birimi olarak resmi para birimi veya diğer döviz para biriminin gösterilmesini belirleyen alandır.|
|Fiyatsız Ürün Gösterimi|Fiyatsız ürünlerin önyüzde gösterilip gösterilmemesi ve satınalmaya izin verilip verilmemesiyle ilgili kullanılan alandır.|
|Varsayılan Üye Fiyat Tipi?|Sistemde default olarak kullanılacak fiyat tipine karşılık gelir.<br>❗️ _Bu kutucuk seçili olduğunda seçili olduğu andan itibaren her yeni üyelik oluşturan kullanıcının fiyat tipi bu fiyat tipi olarak seçilir. Seçilmeden önce planlı bir şekilde dikkat edilmesi gereken bir alandır._|
|Sipariş Oluşturma Anında Kimlik Doğrulama Zorunludur|Bu fiyat tipine bağlı olan kullanıcılar sipariş oluşturacağı zaman kimlik doğrulama işlemine zorlanacaktır.|
|Yurt dışı satışında kullanılsın|İlgili fiyat tipinin yurt dışı satışında kullanılıp kullanılmamasını belirleyen alandır.|
|Not|e-MOS panel kullanıcısı tarafından kullanılabilir not alanıdır. Bu alana yazılan yazı önyüzde görünmeyecektir.|
|Onay|Fiyat tipinin durumunu belirleyen alandır. İlgili fiyat tipinin aktif olması için bu kutucuğun işaretli olması gerekir.|


> ❗️ _Fiyat tipi tanımı doğrudan sipariş sürecini etkilediği için dikkatli ve test sitesine test ederek kullanılmalı._

> ❗️ _Fiyat tipi tanımı [İndirim Kuponu](indirim-kuponu.md) ve [Kampanya Tanımı](kampanya-tanimi.md)nda da kullanılır. Özel bir fiyat tipini indirim kuponu ve kampanya tanımıyla ilişkilendirerek özel bir müşteri segmentine veya sayılı indirim kuponuna özel bir kampanya uygulanabilecektir._