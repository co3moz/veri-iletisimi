ADSL (Asymmetric Digital Subscriber Line)
--------

POTS (Plain old telephone service) standart telefon hizmetine karşılık gelir. POTS ağı aynı zamanda public switched telephone network (PSTN) olarak isimlendirilir. Sonrasında telefon hatlarından veri iletişim yapmak için çevrimeli ağ (dila-up) modemler geliştirilmiştir. Bu modemlerle erişilebilecek veri hızları 64kbps ile sınırlıdır. Bu hızlar internet bağlantısı için yeterli değildir.

Ev kullanıcılarına daha hızlı internet erişimini sağlayabilmek için DSL teknolojisi geliştirilmiştir. Ayrıca TV programlarının ev kullanıcılarına iletimi için geliştirilen Kablo TV ağlar da hızlı internet erişimi için DSL teknolojilerine alternatif olarak sunulmaktadır.


#### PSTN
Manuel PSTN, Analog Anahtarlamalı PSTN ve Sayısal PSTN şeklinde bir gelişim göstermiştir.

Abone hattından gelen sinyal, CO switch'e girdiğinde A/D dönüşümden önce 4kHz'lik Alçak geçiren filtreden geçer. Bir çok kanal switch vasıtasıyla karışıklı bağlantı kurarak anlaşabilir.

#### Çevirmeli Ağ (Dial-Up) Bağlantısı
Dial-Up modem veri aktarımı için ses hatları üzerinden 600 hz ile 3000 hz arasındaki frekans bandını kullanarak modülasyon ve demodülasyon işlemlerini yapar.

PC'deki sayısal veri modem vasıtasıyla analog sinyal haline dönüştürülür. Bu analog sinyal TELCO anahtar cihazı içerisindeki PCM (darbe kod modülasyonu) vasıtasıyla PSTN ağı için tekrar sayısal hale getirilir. Diğer tarafta tersi işlemler yapılarak iki uç düğüm arasında bir veri aktarımı yapılır.


![](dialup.png)

#### ADSL (Asymmetric Digital Subscriber Line)
Çok uzun yıllar telefon ağlarında 4kHz'den yukarısı kullanılmadı. Bu durum mevcut yerel çevrim kabloların 4kHz üstü frekans spektrumunu daha etkin kullanmak ADSL teknolojilerini ortaya çıkardı. ADSL günümüzde bakır telefon kabloları üzerinden 4kHz'den 1.1mHz arası band genişliğini yüksek hızlı veri servisleri için etkin bir şekilde kullanılır.

Bu frekans bandı POTS için kullanılan band ile örtüşmez böylece hem telefon hemde internet hizmeti alınabilir.

Asymmetric bir yöndeki veri akışının diğer  yöndekinden daha hızlı olmasıdır. upstream'den daha hızlı bir downstream hızını tanımlar. Örneğin 1024/256 kbps

Digital Veri tamamen sayısaldır ve sadece uçta yerel çevrim hattı üzerinden taşınabilmek için modüle edilir.

Subscriber Line veri aboneye tek bir burulmuş çift bakır kablo çevrimi üzerinden taşınır.

#### ADSL'de Mesafe
Genelde DSL için tekrarlayıcı kullanmadan maksimum mesafe 5.5km'dir. Telefon şirketlerinin ofisine olan mesafe azaldığında veri hızı artar. Daha uzun mesafeler için fiber optik kablo ile genişletişmiş bir dsl hattına sahip olmanız gerekir. 

Adaptif bir teknolojidir. Sistem abone hattının durumuna bağlı olarak uygun bir veri hızı kullanır. Şu faktörler hızı etkiler
* Yerel merkezden uzaklık
* Kablo tipi ve kalınlığı
* kablodaki ek sayısı ve çeşidi
* ADSL, ISDN ve ses harici sinyalleri taşıyan diğer kablolarla olan yakınlığı
* Radyo vericiye yakınlığı

