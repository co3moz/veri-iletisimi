Veri İletişimine Giriş
-------

#### Protokol
İletişim için oluşturulan kuralların bütününü tanımlar, Hem gönderici hemde alıcı tarafında aynı yapıya ihtiyaç duyulmaktadır. 

Protokolün belirli bir formatı ve veri yapısı vardır. Frame adı altında (Çerçeve) çeşitli datalar saklanır. Örneğin Hedef adresi, Kaynak adresi veya verinin kendisi

Protokolde gelen datayı anlamlı kılan semantik bir kısım vardır. Gelen datanın doğru gelip gelmediği ile ilgilenir.

Son olarakta zamanlama protokolün ne kadar hızlı çalıştığı ve doğru sıralamada gelip gelmediği incelenir bu işe senkronizasyonda denebilir.

_Örneğin A, B'e veri gönderiyor, B saniyede 10 sayı okuyabiliyor ancak A saniyede 100 sayı gönderiyor. Gönderilen 90 sayı ne olacaktır?_


#### Standartlar
Farklı bir çok ürün vardır. Bu ürünlerin belirli standartlar altında birlikte çalışılabilmesi için geliştirilmiştir. Üreticiler ürünlerini bu standartlara göre yapar. 

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

Ticari uygulamalarının verdiği isimler daha yaygınsa **de facto** standart, Standart organizasyonlarının verdiği isimler daha yaygınsa **de jure** standarttır.


#### Hat Konfigurasyonu

**Hat:** Fiziksel iletişim yolu

**Hat Konfigürasyonu**: Bir cihazın bir hattaki ilişkisini tanımlar.

İki farklı hat konfürasyonu vardır
* Noktadan noktaya (point to point), İki cihaz arasında direk bağlantının olduğu durumdur. Sadece 2 bağlantı hattı paylaşır.

![](http://g.gravizo.com/g?digraph%20G%20{%20a%20[shape=box,%20label=%22%C4%B0stasyon%20A%22];%20b%20[shape=box,%20label=%22%C4%B0stasyon%20B%22];%20a%20-%3E%20b%20-%3E%20a;%20})

* Çoklu nokta bğalantısı (multipoint), İkiden daha fazla cihaz hattı paylaşır, kanal kapasitesi cihazlar arasında paylaşılır.


![](http://g.gravizo.com/g?%20digraph%20G%20{%20a%20[shape=box,%20label=%22%C4%B0stasyon%20A%22]%20b%20[shape=box,%20label=%22%C4%B0stasyon%20B%22]%20c%20[shape=box,%20label=%22%C4%B0stasyon%20C%22]%20hat%20-%3E%20a%20-%3E%20hat%20hat%20-%3E%20b%20-%3E%20hat%20hat%20-%3E%20c%20-%3E%20hat%20hat%20-%3E%20Mainframe%20Mainframe%20-%3E%20hat%20})

#### Topolojiler

Bilgisayar ağını oluşturan elemanların yada birimlerin fiziksel veya mantıksal bağlantı ile oluşturulduğu yapı.

4 tip topoloji vardır.

* Yol (Doğrusal) topoloji
* Yıldız (Star) topoloji
* Halka (Ring) topoloji
* Mesh topoloji

![](http://g.gravizo.com/g?%20digraph%20G%20{%20Topoloji%20Topoloji%20-%3E%20Mesh%20Topoloji%20-%3E%20Y%C4%B1ld%C4%B1z%20Topoloji%20-%3E%20Yol%20Topoloji%20-%3E%20Halka%20})

#### İletim Modları

İletim modları bir sistemde iletimin nasıl gerçekleştiğini tanımlar

* Simplex (Tek yön) _Televizyon_

![](http://g.gravizo.com/g?%20digraph%20G%20{%20A-%3EB%20})

* Half duplex (Her iki yönde ancak aynı anda aktarım olma) _Polis radyosu_

![](http://g.gravizo.com/g?%20digraph%20G%20{%20M[shape=box,label=%22M%C3%BCsaitse%20kontrolu%20al%22]%20A-%3EM-%3E%20A%20B-%3EM-%3E%20B%20})

* Full duplex (Aynı anda her iki yönde) _Telefon_

![](http://g.gravizo.com/g?%20digraph%20G%20{%20A-%3EB%20B-%3EA%20})

#### Coğrafi yapılara göre ağ kategorileri

* BAN (Body Area Network)  **~1m**
* PAN (Personal A.N.) **~10m**
* LAN (Local A.N.) **~500m**
* MAN (Metropolitan A.N.) **~3-25km**
* WAN (Wide A.N.) **~>10km**

_Sayılar temsilidir. İlk tasarlanırken bu şekilde düşünülmüştür. Zaman içinde değişmiş güncellenmiştir._

Örneğin bluetooth pan kategorisinde bulunmaktadır. 


#### Ağ Modeli
OSI referans modeli haberleşme sistemi problemini çözmek üzere ISO tarafından 1984'te Açık Sistem Bağlantıları (Open Systems Interconnection) adıyla oluşturulmuştur.

7 Katmandan oluşmaktadır 
* (7) Application: Uygulamalara ağ servisleri sunar
* (6) Presentation: Veri formatı
* (5) Session: Uç birimler arası iletişim
* (4) Transport: Uçtan uca bağlantı
* (3) Network: Adres ve en uygun patika
* (2) Data link: İletim ortamına erişim
* (1) Physical: İkili sayıların transferi

![](http://g.gravizo.com/g?%20digraph%20G%20{%207[shape=box,%20label=%227%20uygulama%20katman%C4%B1%22]%206[shape=box,%20label=%226%20sunum%20katman%C4%B1%22]%205[shape=box,%20label=%225%20oturum%20katman%C4%B1%22]%204[shape=box,%20label=%224%20ta%C5%9F%C4%B1ma%20katman%C4%B1%22]%203[shape=box,%20label=%223%20a%C4%9F%20katman%C4%B1%22]%202[shape=box,%20label=%222%20veri%20ba%C4%9F%C4%B1%20katman%C4%B1%22]%201[shape=box,%20label=%221%20fiziksel%20katman%22]%207-%3E6-%3E5-%3E4-%3E3-%3E2-%3E1%201-%3E2-%3E3-%3E4-%3E5-%3E6-%3E7%20})

#### Kapsülleme
Katmanlar arasında header ekleme ve silme işlemidir.

![](kk.png)

#### OSI ve TCP/IP

TCP/IP mimarisinde uygulama katmanı, OSI'de Uygulama Sunum ve Oturum katmanlarına karşılık gelir. Taşıma aynı şekilde taşımada, İnternet ağda, Ağ erişimde veri bağı ve fiziksel katmanlar olarak düşünülmüştür.

TCP/IP Protokol ailesinde;
* HTTP, FTP, SMTP, DNS, Telnet.. gibi protokoller uygulama
* TCP veya UDP taşıma
* IP (ARP, IGMP, ICMP) internet katmanı
* Eternet, Token Ring, Frame Relay, ATM Ağ erişim katmanını tanımlar.

![](osi-tcp.png)
