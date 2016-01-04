Veri İletişimine Giriş
-------

#### Protokol
**Protokol:** İletişim için oluşturulan kuralların bütününü tanımlar, Hem gönderici hemde alıcı tarafında aynı yapıya ihtiyaç duyulmaktadır. 

Protokolün belirli bir formatı ve veri yapısı vardır. Frame adı altında (Çerçeve) çeşitli datalar saklanır. Örneğin Hedef adresi, Kaynak adresi veya verinin kendisi

Protokolde gelen datayı anlamlı kılan semantik bir kısım vardır. Gelen datanın doğru gelip gelmediği ile ilgilenir.

Son olarakta zamanlama protokolün ne kadar hızlı çalıştığı ve doğru sıralamada gelip gelmediği incelenir bu işe senkronizasyonda denebilir.

_Örneğin A, B'e veri gönderiyor, B saniyede 10 sayı okuyabiliyor ancak A saniyede 100 sayı gönderiyor. Gönderilen 90 sayı ne olacaktır?_


#### Standartlar
**Standartlar:** Farklı bir çok ürün vardır. Bu ürünlerin belirli standartlar altında birlikte çalışılabilmesi için geliştirilmiştir. Üreticiler ürünlerini bu standartlara göre yapar. 

Bazı Standart Organizasyonları
* ISO
* ANSI
* EIA
* IEEE
* ITU-T
* ATM Forum
* IAB
* RFC

2 standart kategori vardır
* **De facto standart** - benimsenen kabul edilen (Ethernet)
* **De jure standart** - kural - IEEE 802.3

Ticari uygulamalarının verdiği isimler daha yaygınsa **de facto standart**, Standart organizasyonlarının verdiği isimler daha yaygınsa **de jure** standarttır.

--------

Temel Kavramlar
------------

#### Hat Konfigurasyonu

**Hat:** Fiziksel iletişim yolu

**Hat Konfigürasyonu**: Bir cihazın bir hattaki ilişkisini tanımlar.

İki farklı hat konfürasyonu vardır
* Noktadan noktaya (point to point), İki cihaz arasında direk bağlantının olduğu durumdur. Sadece 2 bağlantı hattı paylaşır.

<img src='http://g.gravizo.com/g?
 digraph G {
    a [shape=box, label="İstasyon A"]
    b [shape=box, label="İstasyon B"]
    a -> b -> a
 }
'/>

* Çoklu nokta bğalantısı (multipoint), İkiden daha fazla cihaz hattı paylaşır, kanal kapasitesi cihazlar arasında paylaşılır.


<img src='http://g.gravizo.com/g?
 digraph G {
    a [shape=box, label="İstasyon A"]
    b [shape=box, label="İstasyon B"]
    c [shape=box, label="İstasyon C"]
    hat -> a -> hat
    hat -> b -> hat
    hat -> c -> hat
    hat -> Mainframe
    Mainframe -> hat
 }
'/>

#### Topolojiler

Bilgisayar ağını oluşturan elemanların yada birimlerin fiziksel veya mantıksal bağlantı ile oluşturulduğu yapı.

4 tip topoloji vardır.

* Yol (Doğrusal) topoloji
* Yıldız (Star) topoloji
* Halka (Ring) topoloji
* Mesh topoloji

<img src='http://g.gravizo.com/g?
 digraph G {
    Topoloji
    Topoloji -> Mesh
    Topoloji -> Yıldız
    Topoloji -> Yol
    Topoloji -> Halka
 }
'/>

#### İletim Modları

İletim modları bir sistemde iletimin nasıl gerçekleştiğini tanımlar

* Simplex (Tek yön) _Televizyon_
* Half duplex (Her iki yönde ancak aynı anda aktarım olma) _Polis radyosu_
* Full duplex (Aynı anda her iki yönde) _Telefon_




