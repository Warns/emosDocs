---
id: cache-recycle
title: Cache Recycle
---

Websitenin daha hızlı çalışması için, e-MOS cache tutma özelliği ile çalışır. Websitede bulunan çoğu bilgiler (içerik, fiyat, görsel vb.) cache sistemine dahil edilir. Cache sistemine dahil edilen herhangi bir bilgi üzerinde değişiklik yapıldığında (Örnek: Banner görselinin değişimi) önyüze anında yansımayacaktır. Ön yüze yansıması için sunucu üzerinde tutulan cache kayıtlarının silinmesi gerekir.

e-MOS giriş sayfasının header kısmında bulunan **Cache Recycle** butonuna tıkladığınız zaman sunucu üzerinde bulunan eski cache kayıtları silinir yerine güncel olan yeni kaytılar gelir, böylece yapılan değişiklikler önyüzde görünür hale gelir.

Aynı zamanda cache recycle butonuna tıkladıktan sonra yanında bulunan ![](https://snipboard.io/qvMaeu.jpg) butonu ile cache'in temizlenip temizlenmediğini (eğer varsa Varnish cache dahil) görüntüleyebilirsiniz.
<br>
> ❗️ _Yoğun ziyaretçi trafiği olduğu zamanlarda cache recycle yapıldığında websitede bir kaç dakikalığına yavaşlık hissedilebilir. Güncel olan yeni cache kayıtları oluştukça tekrar eski haline gelir._

Cache Recycle butonunun yanında bulunan sarı noktaya tıklayarak cache temizleme işlemini yapan kullanıcıları görüntüleyebilirsiniz.
