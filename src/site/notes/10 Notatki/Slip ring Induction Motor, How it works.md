---
{"dg-publish":true,"permalink":"/10 Notatki/Slip ring Induction Motor, How it works/","tags":["input/video"]}
---

* ponieważ wirnik silnika to układ RL (a więc o charakterze z natury impedancyjnym), napięcie wyprzedza prąd.
	* zgodnie z zasadą działania [[10 Notatki/Maszyna asynchroniczna (indukcyjna)\|Maszyna asynchroniczna (indukcyjna)]] i [[10 Notatki/SEM (Prawo Faradaya)\|SEM (Prawo Faradaya)]]:
		* zmienne pole magnetyczne wytwarza siłę elektromotoryczną
		* siła ta powoduje przepływ prądu
	* ze względu na fakt, że wirnik to obwód RL, napięcie (siła elektromotoryczna) wyprzedza prąd
		* to to nie jest tak, że na tym pręcie / uzwojeniu, na którym aktualnie występuje największa siła elektromotoryczna, występuje też największy prąd
* silnik ma największy moment, gdy prąd w danym pręcie / uzwojeniu wirnika jest w najsilniejszym punkcie pola magnetycznego
	* zgodnie z [[10 Notatki/Siła Lorentza\|Siła Lorentza]], gdzie siła to iloczyn prądu i natężenia pola
	* a ze względu na charakterystykę układu (RL), pręt / uzwojenie z maksymalnym prądem jest przesunięte od tego miejsca
	* ta różnica jest największa przy starcie silnika
	* im bliżej prędkości synchronicznej, tym ta różnica jest mniejsza
* Jeśli w układzie RL zwiększymy znacząco R, tak, że R będzie znacząco większe od L, to układ ten będzie układem w zasadzie czysto rezystancyjnym, a nie RL, co spowoduje, że przesunięcie prądu względem napięcia, będzie w zasadzie równe 0, a więc uzyskamy maksymalny prąd w miejscu maksymalnego natężenia pola magnetycznego
	* i właśnie po to stosuje się **rezystory rozruchowe**
		* **by mieć większy moment już w trakcie rozruchu**
	* chociaż oczywiście i tak (ze względu na początkową niską wartość wyindukowanego napięcia, a przez to prądu) przy samym rozruchu nie uzyskamy maksymalnej siły, czyli momentu