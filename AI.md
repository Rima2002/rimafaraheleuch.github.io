# AI Prompt'ları: DeepSeek

## Prompt#1:
JavaScript'te klavye tuşlarını dinleyerek bir karakteri nasıl hareket ettirebilirim? Ok tuşlarıyla kontrol edilen basit bir sistem lazım.

## Cevap#1:
>```keydown``` ve ```keyup``` event listener'ları kullan. Tuş kodlarını (37=sol, 38=yukarı, 39=sağ, 40=aşağı) bir dizide sakla. Her frame'de bu tuşların durumuna göre karakterin hızını ayarla ve pozisyonunu güncelle.

## Prompt#2:
Oyunumda UFO ile karakter çarpışmasını nasıl kontrol ederim? Sadece UFO kırmızı ışın yayarken öldürsün istiyorum.

## Cevap#2:
> UFO'nun ```isPulling``` özelliği true olduğunda, karakter ve UFO'nun sınır kutularını (bounding box) karşılaştır. Çarpışma için her iki nesnenin koordinatlarını ve boyutlarını kullan, ama hitbox'u biraz küçülterek daha adil bir sistem yap.

## Prompt#3:
UFO'ların ekranda sekerek hareket etmesini nasıl yaparım? Kenarlara çarpınca yön değiştirsinler.

## Cevap#3:
> UFO'ların ```speedX``` ve ```speedY``` değerlerini kullanarak pozisyonlarını güncelle. Canvas sınırlarına geldiklerinde ilgili hız değerini -1 ile çarparak ters yöne hareket etmelerini sağla.

## Prompt#4:
UFO'nun periyodik olarak kırmızı ışın yayıp karakteri çekme efekti nasıl yapılır? Çekme gücü mesafeyle azalsın.

## Cevap#4:
> Bir sayaç (```pullTimer```) kullanarak belirli aralıklarla ```isPulling``` durumunu değiştir. Aktifken, karakter ile UFO arasındaki mesafeyi hesapla. Mesafeye bölerek normalize et ve bir çekme kuvveti çarpanı uygula. Yakın mesafede ölüm kontrolü yap.


