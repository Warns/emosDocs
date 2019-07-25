---
id: profil-tanimi
title: Profil Tanımı
---

Kullanıcı Profil Tanımının yapıldığı ve yetkilendirme haklarının verildiği sayfadır.

Yeni bir profil kaydı oluşturmak için **Ekle** butonu kullanılır. Var olan bir kayıt üzerinde değişiklik yapmak için ilgili kaydın üzerine tıklamak yeterlidir.

Açılan sayfada bulunan alanlarla ilgili detaylar aşağıdaki gibidir;

## 1. Genel Bilgiler

|Alan Adı|Açıklama|
|--|--|
|Profil Adı|Tanımlacak olan profil adının girildiği alandır.|
|Profil Açıklama|Profil açıklamasının girildiği alandır.|
|Ent. Kodu|Profil tanımı entegrasyona bağlı olarak çalıştığı durumlarda kullanılır.|
|Onay|Profilin aktif olabilmesi için bu kutucuğun işaretli olması gerekmektedir.|

### 1.1. Alan Hakları

Oluşturulan profilde bu bölümünden "Okuma" hakkı verilmiş bir içeriğin içerisindeki belli alanların değiştirilmesine izin verilebilir.

|Alan Adı|Açıklama|
|--|--|
|Modül Adı|Yetkilendirme verilecek olan modül adının seçildiği alandır.|
|Alan Adı|Yetkilendirme verilecek olan alan adının girildiği alandır.|
|Alan pasif olsun mu?|Alan hakları bölümünde ilgili kaydın pasif/aktif etmek için kullanılır.|

<br>
## 2. Sayfa Hakları

Tanımlı kullanıcılara belli sayfalar veya tüm sayfalar için  **Okuma, Yazma** yetkilerinin tanımlanabildiği bölümdür.

### 2.1. Okuma Hakkı
Yönetim panelinde belirlenen sayfalarda sadece sayfayı görüntüleme olanağı sağlar.

### 2.2. Yazma Hakkı
Admin panelinde belirlenen sayfalarda işlem yapma imkanı sağlar. 

>❗ _Her hangi bir yetki verilmediğinde kullanıcı ilgili modülü görüntüleyemeyecektir._

Eğer bir sayfa için flag (tik işareti) yeşil ise ilgili sayfaya yetki verilmiştir, kırmızı ise yetki verilmemiştir.

Kullanıcıya belirlenen bir sayfada yetki verebilmek için;

- Yetki verilmek istenen sayfalar listeden işaretledikten sonra **Okuma Hakkı** veya **Yazma Hakkı** butonlarına tıklayarak yetki veilir.
- Eğer sayfalar işaretlendikten sonra **Hakları Kaldır** butonuna tıklanırsa o kullanıcı ilgili sayfayı görüntüleyemez.
- Eğer görüntülenen ana kategorilerden biri işaretledikten sonra yazma veya okuma hakkı verilirse ana kategoriye bağlı olan alt kategoriler de aynı hakkı alacaktır .

>❗ _Sayfa hakkı verilecek kullanıcıya Admin yazma hakkı verilirse diğer sayfalarda izni olmasa bile site üzerindeki bütün sayfalara ulaşabilir._


- #### Mesaj Hakları :
Yetki verilen kullanıcının hangi tür mesajları görüp yanıtlayabileceğinin belirlendiği bölümdür. Eğer yetki verilen kullanıcının belli gruplardaki mesajları görüntülemesi ve cevap vermesi isteniyorsa **kutucuğun** işaretli olması gerekmektedir.

>❗ _Eğer bir kullanıcı admin olarak tanımlandı ise bütün mesajları görür ve yanıtlayabilir._

<br>
## 3. İçerik Sayfa Hakları
[Sayfa Hiyerarşi](sayfa-hiyerarsi.md) sayfasında bulunan içerik ve statik sayfalara yetki tanımlamak için kullanılan sayfadır.

Sayfaların sol tarfında bulunan kutucukları işaretleyerek topluca Okuma, Yazma veya Yayınlama hakkı tanımlanabilecektir. En üst seviyedeki bir sayfa klasörüne yetki tanımlandığında ilgili yetki klasördeki diğer tüm alt sayfalar için de geçerli olacaktır.

### 3.1. Okuma Hakkı
Sayfa hiyerarşideki ilgili sayfaya sadece görüntüleme yetkisi tanımlanır.

### 3.2. Yazma Hakkı
Sayfa hiyerarşideki ilgili sayfaya yazma ve görüntüleme yetkisi tanımlanır.

### 3.3. Yayınlama Hakkı
Canlı siteye publish etme yetkisi. Bu yetkiye sahip olan kullanıcı ilgili içerik sayfasını veya değişikliği doğrudan canlı sitede yayınlama yetkisine sahiptir.

>❗ _Yayınlama Hakkına sahip olmayan bir kullanıcı yaptığı değişikliği veya eklentiyi yetkili birinden onay isteme mekanizmasıyla sürdürebilecektir._

>❗ _Her hangi bir yetki verilmediğinde kullanıcı ilgili modülü görüntüleyemeyecektir._

<br>
## 4. Mesaj Hakları
Website kullanıcıları tarafından gönderilen mesajlara cevap verme yetkilerinin verildiği sayfadır. 

Soru gruplarında bulunan soru mesajlarının yanlarındaki kutucukları işaretlediğinizde ilgili profile bağlı kullanıcılara cevap verme yetkisi tanımlamış olursunuz. 

<br>
## 5. Sistem ve Grup Hakları
Kullanıcıya sistem ve grup hakları konusunda gönderilen mesajları okuyabilme ve cevaplayabilme izni verilebilen sayfadır. Kullanıcının görüntülemesi ve cevaplaması istenilen mesajlar buradan belirlenir.

<br>
## 6. Özel İşlem Hakları
İlgili kullanıcı profiline sistem zerinde bulunan bazı özel modül ve işlemlerin yetkisinin verildiği sayfadır. 

<br>
## 7. API Hakları
İlgili kullanıcı profiline API V3 servisinin üzerinde bulunan metodlara yetkilerin verildiği sayfadır. 
