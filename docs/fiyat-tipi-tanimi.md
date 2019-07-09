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
|Min. 
|Artış||
|Üye Bonus kazandırma Oranı (Taksitli Ödeme)||
|Tavsiye Bonus Kazanma Süresi||
|Üye Bonus kazandırma Oranı (Banka Bonus)||
|Kdv Gösterim Şekli||
|Ürün PB Gösterimi||
|Fiyatsız Ürün Gösterimi||
|Varsayılan Üye Fiyat Tipi?||
|Sipariş Oluşturma Anında Kimlik Doğrulama Zorunludur||
|Onay||
|Yurt dışı satışında kullanılsın||
|Not||

> ❗️ _Fiyat tipi tanımı doğrudan sipariş sürecini etkilediği için dikkatli ve test sitesine test ederek kullanılmalı._

> ❗️ _Fiyat tipi tanımı [İndirim Kuponu](indirim-kuponu.md) ve [Kampanya Tanımı](kampanya-tanimi.md)nda da kullanılır. Özel bir fiyat tipini indirim kuponu ve kampanya tanımıyla ilişkilendirerek özel bir müşteri segmentine veya sayılı indirim kuponuna özel bir kampanya uygulanabilecektir._