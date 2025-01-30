---
{"dg-publish":true,"permalink":"/10 Notatki/Silniki prądu stałego DC/","tags":["wiedza/zettel"]}
---

* ## Prosty silnik
	* Wirnik ma dwa końce, które są podłączone osadzonych a sztywno na wale dwóch pierścieni komutacyjnych, które obracając się stykają się za pomocą szczotek komutacyjnych z komutatorem, który jest nieruchomy 
		* Jeden pierścień jest podłączony do +, drugi do minusa
		* W miarę obrotu, prąd płynie raz z jednego końca uzwojenia wirnika do drugiego, a następnie polaryzacja się zmienia
		* Względnie, z punktu widzenia pola magnetycznego wytwarzanego przez stojan, prąd zawsze płynie w tym samym kierunku
			* Polaryzacja musi się zmieniać, bo wirnik się obraca
		* Za pomocą siły [[10 Notatki/SEM (Prawo Faradaya)\|SEM (Prawo Faradaya)]] pole wytwarzane przez stojan wprawia w ruch uzwojenie wirnika, w którym płynie prąd
* ## Utyk wirnika
	* W pozycji, gdy ramka jest w płaszczyźnie prostopadłej do linii pola magnetycznego, moment wytwarzany na wale równy jest 0 i wirnik obraca się jedynie siłą rozpędu
		* Stąd na wirniku stosuje się dwa uzwojenia
			* Gdy jedno uzwojenie wytwarza moment równy 0, wówczas drugie wytwarza maksymalny moment, co wpływa na płynną pracę
* ## Realna budowa wirnika
	* Z powyższego wynika wniosek, że im więcej uzwojeń wirnika, tym praca może być bardziej płynna, więc w rzeczywistości stosuje się wiele uzwojeń
	* Dodatkowo, by zwiększyć moment generowany przez silnik, uzwojenia są poprzekładane żelazem
* ## Stojan
	* W silnikach małej mocy, można stosować stojan w postaci permanentnych magnesów
	* Zazwyczaj jednak stosuje się elektromagnes, który jest zasilany z tego samego źródła DC
		* Elektromagnes składa się z uzwojenia i nałożonego na niego pierścieni z żelaza, które nie musza być zalaminowane od siebie, bo w uzwojeniu płynie prąd DC, więc nie powstają prądy wirowe
* ## Rodzaje silników
	* ### [[10 Notatki/Silnik szeregowy DC (series motor)\|Silnik szeregowy DC (series motor)]]
		* 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/10-notatki/silnik-szeregowy-dc-series-motor/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




* ![Pasted image 20250130184849.png](/img/user/80%20Zasoby/Pasted%20image%2020250130184849.png)
* prąd przepływa przez:
		1. jedną część stojana
		2. uzwojenia wirnika
		3. drugą część stojana
* dobry moment rozruchowy
* prędkość spada drastycznie podczas obciążenia
* Nietypowe silnik szeregowy – [[10 Notatki/Silnik uniwersalny (AC-DC)\|Silnik uniwersalny (AC-DC)]]

</div></div>

	* ### [[10 Notatki/Silnik bocznikowy DC (shunt motor)\|Silnik bocznikowy DC (shunt motor)]]
		* 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/10-notatki/silnik-bocznikowy-dc-shunt-motor/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




* ![Pasted image 20250130185311.png](/img/user/80%20Zasoby/Pasted%20image%2020250130185311.png)
	* wirnik podłączony równolegle do stojana
* niski moment rozruchowy
* jest w stanie obracać się bezmała z tą samą prędkością, bez względu na obciążenie

</div></div>

* ## Zwrotna siła [[10 Notatki/SEM (Prawo Faradaya)\|SEM (Prawo Faradaya)]]
	* Ponieważ wirnik jest to uzwojenie (ramka w uproszczeniu), które znajduje się w zmiennym polu magnetycznym, to na jej końcach indukuje się napięcie o przeciwnej polaryzacji do zasilania z pierścieni komutatorowych
	* W związku z tym, w tym uzwojeniu zaczyna płynąć prąd w przeciwną stronę, niż ten, który płynie ze względu na podłączenie do dwóch komutatorów
		* W efekcie, w uzwojeniach wirnika płynie prąd wypadkowy równy różnicy tych dwóch prądów
	* Prąd zwrotny jest proporcjonalny do prędkości obrotowej silnika
		* Ponieważ przy większej prędkości występuje większa zmiana strumienia magnetycznego
	* Siła ta jednak jest w pewnym sensie korzystna, bo pozwala redukować prąd w uzwojeniu wirnika, dla którego uzwojenie jest zwarciem (cewka w układzie DC)
		* Przy rozruchu prąd zwrotny jest jednak zbyt mały i bez odpowiedniego układu rozruchowego, mogłoby dojść do spalenia się uzwojeń wirnika