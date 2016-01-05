İletim Bozulmaları, Kanal kapasitesi, ağlarda gecikme ve İletim ortamları
-------
#### İletim Bozulmaları
Alınan sinyal gönderilen sinyallerden farklı olabilir. Analog iletimde sinyal kalitesinde bozulma verim kaybı, sayısal iletimdede bit hataları olabilmektedir.

İletim ortamındaki bozulmaların ana kaynağı;
* İletim ortamının çeşidi
* İletilen verinin bit hızı
* Haberleşen iki cihaz arası mesafe

İletim Bozulma çeşitleri
* Zayıflama (Attenuation)
* Sınırlı Bandgenişliği (Limited Bandwidth)
* Gecikme Bozulması (Distortion)
* Gürültü (Noise)



* Zayıflama (Attenuation)
![](iletim-bozulmalari.png)

Zayıflama sinyal gücünün mesafeye bağlı olarak azalmasından kaynaklanır. Güclendirici veya tekrarlayıcı kullanarak sorun çözülebilir. 

```
dB = 10log(sinyalin son durumdaki gücü (watt) / sinyalin üretilirken gücü (watt))
```

* Sınırlı Bandgenişliği (Limited Bandwidth)


Bir sinyal farklı frekans bileşenlerinin toplamından oluşuyordu, herhangi bir iletişim kanalı sınırlıdır. Bu yüzden bandgenişliğinin dışında kalan frekanslar kayıp edilecektir.

* Gecikme Bozulması (Distortion)

Sinyalin şekli değişir, bir sinyalin iletim ortamındaki kayma durumuna denir.

* Gürültü (Noise)

Verici ve alıcı arasındaki sinyale ek (istenmeyen) sinyaller eklenir. Bazı gürültüler;
* Termal gürültü
* Intermodulation gürültü
* Crosstalk (yanses, başka kabloların etkisi yüzünden oluşan gürültüdür)
* Impulse Gürültüsü

#### Sinyal gürültü oranı
Bir sinyalin içerdiği gücün gürültü gücüne oranı iletimde önemli bir konudur ve sinyal gürültü oranı SNR olarak tanımlanır.

```
SNR(db) = 10 log (Sinyal gücü / Gürültü gücü)
daha önce zayıflama miktarını anlamak için bu formülü kullandık.
```

![](snr.png)

#### Kanal kapasitesi
Daha büyük bir band genişliği daha yüksek bir bilgi taşıma kapasitesi sağlar. Bu mantığa göre herhangi bir sayısal dalga aslında sonsuz bir bandgenişliğine sahiptir. Fakat iletim ortamı bozulmalardan dolayı, bu bandgenişliği sınırlandıracaktır ve bununla birlikte herhangi verilen bir ortam için daha yüksek bandgenişliği iletim maaliyetinin artmasına neden olur, buna karşılık band genişliğini sınırlamak bozulmalara neden olmaktadır.

Bütün bunlara bağlı olarak Kanal kapasitesi, belirli şartlar altında verilen bir iletim ortamı yada kanalı üzerindne iletilebilecek maksimum bit hızını tanımlar, **Nyquist** tarafından gürültüsüz ve **Shannon** tarafından gürültülü kanal için bit hızları belirlenmiştir. Bandgenişliği, gürültü ve hata oranı gibi 3 faktörden etkilenmektedir.

#### Nyquist Bit Hızı
Gürültüsüz ve hatadan yoksun bir kanal için tanımlanır. Bandgenişliği B ise en yüksek haberleşme hızı 2B'dir. İki voltaj seviyeli binary sinyal için;

```
Nyquist bit hızı = 2B(bps)
```
Çoklu voltaj seviyesine veya sinyal seviye sayısına (L) sahip sinyal için Nyquest bit hızı
```
Nyquist bit hızı = 2Blog2L(bps)
```

**Örneğin** _L=8 ve 3000Hz bandgenişliği için Nyquest bit hızı = 18kbps olur._