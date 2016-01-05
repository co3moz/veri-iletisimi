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