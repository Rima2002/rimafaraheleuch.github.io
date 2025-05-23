# AI Prompt'ları

## Prompt#1:
JavaScript'te klavye tuşlarını dinleyerek bir karakteri nasıl hareket ettiririm? Yön tuşları (ok tuşları) için basit bir event listener örneği verir misin?

## Cevap#1:
> ```keydown``` ve ```keyup``` event'larını kullanabilirsin. Tuş kodlarını (```keyCode```) bir diziye kaydederek hangi tuşun basılı olduğunu takip edebilirsin. Örneğin, sol ok tuşu (37) basılıysa karakterin X pozisyonunu azalt.

## Prompt#2:
Peki tüm görseller yükledikten sonra "assetLoaded" fonksiyonu ile oyunu nasıl başlatabilirim kısacası .

## Cevap#2:
> Harika bir soru! Oyunlarda tüm görseller (ve sesler) yüklendikten sonra oyunu başlatmak için genellikle bir yükleme sayacı (asset counter) kullanılır. Bu sayede tüm asset’ler (resimler, sesler, vs.) yüklendiğinde tek bir fonksiyon (startGame() gibi) çağrılır.
>  Kısaca:
1.	Kaç görselin yükleneceğini bil.
2.	Her yükleme tamamlandığında assetLoaded() fonksiyonu çalışsın.
3.	Tüm asset’ler yüklendiğinde startGame() fonksiyonu çağrılsın.
```
Özet:
*	assetLoaded() her görsel yüklendiğinde çağrılır.
*	İçinde assetsLoaded sayısını takip edersin.
*	Hepsi tamamlandığında startGame() ile oyun başlar.
```

## Prompt#3:
Bir oyunda Skoru (1 artırarak ) textContent kullanarak nasıl güncelleyebilirim kısacası

## Cevap#3:
> Bir oyunda skoru textContent kullanarak 1'er 1'er artırmak için yapman gerekenler çok basit:
```
Özet:
*	textContent DOM üzerindeki metni değiştirir.
*	score += 1 ile sayı artar.
  	element.textContent = "Skor: " + score ile ekrana yansıtılır.
```

## Prompt#4:
Klavye kontrol ayarları, yani ok tuşları,'keyup' 'keydown' ile 'keyCode' (hepsini bir Array içinde koyarak) değerleri kullanarak nasıl yapabilirim kısacası.

## Cevap#4:
> Kısaca: Klavye ok tuşlarını (ArrowUp, ArrowDown, ArrowLeft, ArrowRight) keydown ve keyup ile takip edip, hangi tuşların basılı olduğunu bir keys dizisi içinde tutarak kolayca kontrol sistemi kurabilirsin.
```
Kısacası:
*	keys[e.keyCode] = true/false ile hangi tuş basılı takip edilir.
*	Oyun döngüsünde if (keys[KEY]) kontrolüyle hareket yapılır.
*	Bu sistem hem basılı tutmayı hem birden fazla tuşu aynı anda kontrol etmeyi sağlar.
```

## Prompt#5:
Karakter hareketini nasıl kontrol edebilirim sağ, sol, yukarı, aşağı kısacası 

## Cevap#5:
> Karakteri sağ, sol, yukarı, aşağı yönlerde hareket ettirmek için:
1.	Klavye tuşlarını dinle (keydown / keyup)
2.	Tuşlara basıldığında bir keys dizisinde tut
3.	Oyun döngüsünde bu tuşlara göre x ve y pozisyonlarını değiştir
4.	Canvas’ta her frame'de karakteri yeni konumda çiz

```
Açıklama:
*	player.x ve player.y pozisyonudur.
*	keys[KEY] kontrolüyle yön belirlenir.
*	draw() ile canvas her seferinde temizlenir ve kare yeniden çizilir.
```

## Pormpt#6:
20 Saniyelik bir geri sayımı nasıl başlatabilirim kısacası

## Cevap#6:
> 20 saniyelik bir geri sayımı başlatmak için setInterval() kullanarak her saniye sayıyı 1 azaltabilir, DOM'da textContent ile gösterebilirsin.
```
Özet:
*	setInterval() ile her saniye sayıyı azalt.
*	textContent ile ekranda göster.
*	clearInterval() ile süre bitince sayacı durdur.
```
