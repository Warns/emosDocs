---
id: template-tanimi
title: Template Tanımı
---

Website üzerinde kullanılacak olan banner içeriklerine ait template'lerin hazırlandığı sayfadır.

Yeni bir template tanımı eklemek için **Ekle** butonu kullanılır. Var olan bir template üzerinde değişiklik yapmak için herhangi bir kaydın üzerinde tıklayarak yeni bir sayfa açılır.

Sayfada bulunan alanlarla ilgili detaylar aşağıdaki gibidir;

## 1. Genel Bilgiler

|Ala Adı|Açıklama|
|--|--|
|Template Seçim|Template adının girildiği alandır.|
|Ters Sıra|Template içerisindeki parametrelerin azalan sayı veya artan sayı olarak sıralamasını sağlar. Bu ayara göre en büyük sayılı veya en düşük sayılı parametre (banner) ilk sırada veya en son sırada görünür.|
|Dil|Bu alan sitenin default diline göre otomatik olarak seçilmektedir. Çoklu Dil tanımı yapısıyla ilgili ayrıntılı bilgi almak için [Tıklayın](coklu-dil.md)|
|Onay|Template tanımının durumunu belirleyen alandır. Aktif hale getirmek için bu kutucuğun seçili olması gerekir.|

Gerekli alanları doldurduktan sonra **Kaydet** butonuna tıklayarak template tanım işlemi tamamlanır. Kaydetme işlemi tamamlanınca sayfanın bir alt kısmında bulunan **Template Parametreleri** bölümü aktif hale gelir.

<br>
## 2. Template Yapısı
Oluşturulacak olan template içeriğine göre aşağıdaki yapılardan biri kullanılacaktır; 

### 2.1. Liste Template 
Örnek olarak kampanyaların bulunduğu bir sayfa oluşturmak istendiğinde. Bu sayfada birçok kampanya, aynı biçimde ve belli bir düzenle sıralanacaktır.

Her bir kampanyanın üzerine tıklandığında, o kampanya ile ilgili detay bilgisi verilen bir sayfaya gidecektir. 

Kampanyalarımızın listelenme biçiminin (listedeki herbir kampanyanın) nasıl bir HTML yapısına sahip olacağının belirlendiği kısımdır. 

### 2.2. Detay Template
Listedeki herhangi bir kampanya üzerine tıklandığında gidilecek olan, kampanya detay sayfasındaki HTML yapısının belirlendiği kısımdır.

Oluşturduğumuz bu html yapısında, parametreleri çağırırken, "Parametre" kısmına girdiğimiz değişkeni, `$` işaretleri arasına koyarak çağırmamız gerekmektedir.<br>**Örnek:** `<span>$prmBaslik$</span>` veya `<img src="$prmResim$" />` vb.

<br>
## 3. Template Parametreler
İlgili template içerisinde kullanılacak olan parametrelerin (alanların) belirlendiği kısımdır.

> ❗ _Kullanılabilecek parametreler **Template Parametreleri**'nin üst kısmında belirtilmiştir._

Yeni bir parametre eklemek için **Ekle** butonu kullanılır. Var olan bir parametre üzerinde değişiklik yapmak için de herhangi bir kaydın üzerine tıklayarak yeni bir sayfa açılır.

Açılan sayfada bulunan alanlarla ilgili detaylar aşağıdaki gibidir;

|Alan Adı|Açıklama|
|--|--|
|Parametre Adı|Parametre'nin adının belirlendiği alandır.|
|Parametre|Kullanılabilecek olan parametrelerin arasında seçilen parametre bilgisinin girildiği alandır. HTML yapısında, parametrenin çağırılacağı değişken bilgisinin girileceği alandır. Bu alana girilen değer Template yapısında kullanılırken '$' işaretleri arasında kullanılmalıdır.|
|Parametre Tipi|Parametre tipinin seçildiği alandır.<br>**Örnek:** RichText, Seçenek, Kategori, Çoklu Seçim vs.|
|Parametre Seçenek|Parametre tipi olarak "Seçenek" seçildiyse bu kısıma seçenek değerleri aşağıdaki şekilde girilmelidir.<br>**Örnek:** SeçenekValue;SeçenekText, SeçenekValue2;SeçenekText2 vb.|
|Data Rule|Template içerisinde belli bir seçim yapıldığında bir kuralın tetiklenmesi için kullanılan alandır.<br>**Örnek:** İçerik tipi olarak Image seçildiğinde Image ekleme alanı göster. Video seçildiğinde Image ekleme alanını gizle ve video ekleme alanını göster gibi. |
|Parametre Sıra|Template içerisindeki parametre sırasını belirleyen alandır.|
|Zorunlu Alan|İlgili alanın zorunlu olup olmadığını belirleyen alandır. Zorunlu olarak işaretlendiğinde ilgili alan kırmızı renkte görünecektir..|
|Edit Edilebilir|İlgili parametrenin Inline Editing yapısında edit edilebilir veya edit edilemez durumunu ayarlayan alandır.|
|Onay|Parametrenin durumunu belirleyen alandır. Aktif hale getirmek için bu kutucuğun işaretli olması gerekir.|

>❗  _Parametre tipi Seçenek olarak seçilip Seçenek kısmına değer girildiğinde bu parametreyi Template tarafında kullanabilmek için parametre adından sonra _text, _value eklenmelidir. <br>**Örnek:** Seçenek parametre adımız `$prmSecenek1$` ise bu parametrenin text alanı için `prmSecenek1_text`, value alanı için `prmSecenek1_value` şeklinde kullanılır._

<br>
## 4. Diğer Diller
Birden fazla dil kullanılan sitelerde template ve parametrelerin diğer dillerini eklemek için kullanılan alandır. Çoklu Dil yapısıyla ilgili ayrıntılı bilgi almak için [Tıklayın](coklu-dil.md).

