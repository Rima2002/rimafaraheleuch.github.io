# Sincap – Elma Toplama Oyunu
## 1. Proje Amacı
Bu proje, HTML5 Canvas ve JavaScript kullanılarak oluşturulmuş basit bir 2D macera oyunudur. Oyuncu, yön tuşları ile bir sincabı kontrol eder. Amaç, 30 saniye içerisinde 10 elmayı toplamak ve engellere çarpmadan oyunu kazanmaktır.

  ![image alt](https://github.com/Rima2002/rimafaraheleuch.github.io/blob/main/oyun_talimatlari.PNG)


  **Seçtiğim oyun:** ![ORB Inc.] (https://angry-armadillo-games.itch.io/bricker-breaks-free)

> Orbinc'in çekirdek mekaniği olan "yerçekimi alanlarından kaçarak enerji toplama" oyunu minimalist tasarımı ve basit ama bağımlılık yapan şekilde kendi kültürel öğelerimi katabileceğim bir versiyon oluşturmak istedim. Orbinc'teki uzay teması yerine Türk ormanlarında geçen bir sincap hikayesi kurguladım.
**Entegre Ettiğim Mekanikler:**
-Çekim Alanları (Orbinc'teki Kara Delikler):
Orbinc'teki kara deliklerin çekim gücünü, UFO'ların "kırmızı ışın" efektiyle uyarladım.


## 2. Kullanılan Teknolojiler
-	**HTML5:** Sayfa yapısı ve oyun alanı (canvas) oluşturmak için kullandım.
-	**CSS3:** Oyun tasarımı, butonlar ve kullanıcı arayüzü düzenlemeleri için kullandım.
-	**JavaScript:** Oyun mekaniği, hareket, skor sistemi, çarpışma tespiti ve zamanlayıcı işlemleri için kullandım.
-	**HTML5 <canvas>:** Oyun grafikleri çizimi için ana platform olarak kullandım.
-	**Görseller:** Sincap karakteri, elma, sarı robotlar, UFO ve arka plan (ChatGpt ile kendim oluşturdum)
- **Sesler:** Arka plan müziği, elma toplama sesi, oyun bitiş sesi.

## 3. Oyun Kuralları ve Mekanikleri
-	**Amaç:** Oyuncu, 30 saniye içinde 10 elma toplamalıdır.
-	**Kontroller:** Yön tuşları ile hareket sağlanır (↑ ↓ ← →).
-	**Kazanç:** Oyuncu 10 elmayı süresi dolmadan toplarsa oyunu kazanır.

  ![image alt](https://github.com/Rima2002/rimafaraheleuch.github.io/blob/main/kazanc.PNG)

-	**Kaybetme:** Oyuncu bir engelle çarpışırsa ya da süresi dolarsa oyun biter.
  
  ![image alt](https://github.com/Rima2002/rimafaraheleuch.github.io/blob/main/kaybetme.PNG) 
 	
  ![image alt](https://github.com/Rima2002/rimafaraheleuch.github.io/blob/main/zaman_doldu.PNG)

-	**Engeller:** Kırmızı ışın yayan UFO'lar (seni kendine çeker) ve sarı robotların attığı mermiler.
-	**Elma:** Haritada rastgele konumlanan, sabit boyutlu hedef.

## 4. Oyunun İşleyişi
1.	Oyuncu **“Oyunu Başlat”** butonuna tıkladığında oyun başlar.
2.	Süre geri saymaya başlar **(30 saniye)**.
3.	Sincap, yön tuşlarıyla hareket eder ve engellerden kaçar.
4.	Elma toplanınca skor artar ve yeni elma haritada rastgele bir yere yerleştirilir.
5.	**Skor 10**’a ulaştığında **“🎉 Kazandın!”** mesajı gösterilir.
6.	Oyun bittiğinde **“Oyunu Yeniden Başlat”** butonu aktif olur.

Oyun Linki: [GitHub Pages](https://rima2002.github.io/rimafaraheleuch.github.io/)

Youtube Linki: [Youtube Video](https://www.youtube.com/watch?v=h3-dopV331w)

## 5. Kullanıcı Arayüzü Özellikleri
*	Skor ve geri sayım sayacı.
*	Başlatma ve yeniden başlatma butonları.
*	Kazanma mesajı ve oyun talimatları .
*	Görsel olarak sade ve kullanıcı dostu tasarım.
  
> [!NOTE]
> - Seviye sistemi: Elma sayısını ve engel hızını artırarak zorluk seviyesi ayarlanabilir.
> - Can sistemi: Engellere birden fazla çarpma hakkı tanınabilir.
> - Daha fazla ses efekti: Etkileşimli sesler oyun deneyimini zenginleştirir.
> - Tema değişikliği: Farklı arka planlar ve karakter seçenekleri sunulabilir.

## 6. Sonuç
“Sincap: Elma Toplama” oyunu, temel düzeyde oyun geliştirme ve JavaScript ile interaktif uygulama yapma konusunda güçlü bir örnektir. Oyun hem eğlenceli hem de geliştirilmeye açık bir yapıya sahiptir.
