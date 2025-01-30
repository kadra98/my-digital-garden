---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 5.13 – Regulacja prędkości obrotowej silników prądu stałego/","tags":["wiedza/zettel"]}
---

* ## Regulacja szeregowa
{ #36d915}

	* Polega na włączeniu rezystancji regulacyjnej $R_{R}$ w szereg z obwodem twornika, tj. wirnika
	* Stosuje się zarówno w [[10 Notatki/Silnik szeregowy DC (series motor)\|silnikach szeregowych]] jak i [[10 Notatki/Silnik bocznikowy DC (shunt motor)\|silnikach bocznikowych]]
	* Im większa rezystancja, tym mniejsza prędkość obrotowa
	* ![Pasted image 20250130195452.png](/img/user/80%20Zasoby/Pasted%20image%2020250130195452.png)
	* Jest podobna do regulacji prędkości obrotowej w [[10 Notatki/silnik pierścieniowy\|silniku pierścieniowym]]
	* Jest nieekonomiczna, bo zamieniamy energię elektryczną w ciepło wydzielane na rezystorze
		* Więc nie stosuje się jej w silnikach dużej mocy
	* ### Silnik bocznikowy
		* ![Pasted image 20250130221729.png](/img/user/80%20Zasoby/Pasted%20image%2020250130221729.png)
	* ### Silnik szeregowy
		* ![Pasted image 20250130221751.png](/img/user/80%20Zasoby/Pasted%20image%2020250130221751.png)
* ## Regulacja bocznikowa
{ #682474}

	* polega na osłabieniu pola magnetycznego
	* im mniejsze pole magnetyczne, tym – **paradoksalnie** – większa prędkość obrotowa
	* można ją przeprowadzić w zakresie $n_{n} \div 3n_{n}$ 
		* w regulacji bocznikowej im większa prędkość obrotowa, tym większe napięcie między wycinkami komutatora
			* zgodnie z równaniem $$n=c\frac{U-RI_{tw}}{\Phi}$$
				* gdzie $RI_{tw}=\text{const}$
		* Dlatego zakres regulacji jest ograniczony – by nie dochodziło do iskrzenia
		* Zjawisko to nie występowałoby jednak, gdyby maszyna miała uzwojenie kompensacyjne
		* Przy dalszym osłabianiu strumienia ujawnia się także niekorzystny wpływ oddziaływania twornika na przebieg charakterystyki mechanicznej, co wpływa na zmniejszenie stabilności pracy
	* Regulacja ta jest ekonomiczna
	* ### Silnik szeregowy
		* ![Pasted image 20250130213252.png](/img/user/80%20Zasoby/Pasted%20image%2020250130213252.png)
			* bocznikujemy obwód wzbudzenia (stojan)
			* zakazane jest zwieranie obwodu wzbudzenia
	* ### Silnik bocznikowy
		* ![Pasted image 20250130213201.png](/img/user/80%20Zasoby/Pasted%20image%2020250130213201.png)
		* włączamy w szereg z obwodem wzbudzenia, czyli stojanem
		* zakazane jest rozwieranie obwodu wzbudzenia, bo wówczas przy biegu jałowym strumień spadnie do 0, a prędkość silnika wielokrotnie wzrośnie (jeśli wcześniej był w ruchu i utrzyma prędkość)
* ## Regulacja przez zmianę napięcia zasilania
	* ### Układ trakcyjny
		* 2 silniki szeregowe podłączone
			* na początku szeregowo
				* ![Pasted image 20250130215829.png](/img/user/80%20Zasoby/Pasted%20image%2020250130215829.png)
				* na każdy silnik przypadka połowa napięcia sieciowego i odpowiednio do tego ustala się przy określonym momencie obciążenia wypadkowa prędkość obrotowa
			* później równolegle
				* ![Pasted image 20250130215932.png](/img/user/80%20Zasoby/Pasted%20image%2020250130215932.png)
				* na każdym silniku panuje pełne napięcie
				* przy obciążeniu takim samym momentem, prędkość obrotowa jest dwukrotnie większa
		* skokowa zmiana napięcia przy przełączeniu wywołałaby duże uderzenie prądowe, pojawienie się dużego momentu (zryw) i gwałtowny wzrost prędkości
			* w związku z tym wykorzystuje się rozrusznik, analogicznie jak przy rozruchu silnika
			* Rozrusznik ten może pełnić również rolę regulatora prędkości [[10 Notatki/EGZ INŻ 5.13 – Regulacja prędkości obrotowej silników prądu stałego#^36d915\|tak jak w regulacji szeregowej]], o ile został odpowiednio dobrany
				* Zasadniczo rozkruszków używa się jedynie podczas rozruchu; standardowo nie jest przystosowany do ciągłej pracy pod obciążeniem
	* ### Układ Leonarda
		* pozwala na regulację prędkości w szerokich zakresach i regulacji wielokrotnej podczas jednej rodziny
		* ![Pasted image 20250130220730.png](/img/user/80%20Zasoby/Pasted%20image%2020250130220730.png)
		* źródłem zasilania wirnika jest prądnica (tzw. prądnica sterująca) przeznaczona jedynie i specjalnie do tego
			* Prądnica ta pracuje przy stałej prędkości obrotowej
			* Zarówno prądnica jak i silnik (jeśli jest [[10 Notatki/Maszyna synchroniczna, generator, prądnica\|silnikiem synchronicznym]]) są wzbudzane przez dodatkową wzbudnicę osadzoną na wspólnym wale
		* Regulując prąd wzbudzenia prądnicy za pomocą regulatora możemy w sposób ciągły zmieniać napięcie tej prądnicy, a zarazem napięcie podawane na wirnik silnika DC w zakresie $0\div n_{n}$
			* Ciągłej zmianie napięcia odpowiada ciągła zmiana prędkości obrotowej
		* Regulacja jest ekonomiczna, bo wiąże się jedynie z regulacją prądu wzbudzenia prądnicy sterującej
		* Zmianę kierunku wirowania przeprowadza się poprzez zmianę kierunku prądu wzbudzenia prądnicy
		* Jeśli dodatkowo chcielibyśmy wykroczyć ponad prędkość znamionową $n_{n}$ możemy posłużyć się regulacją osłabiającą strumień (i przez to pole magnetyczne w obwodzie wzbudzenia) – [[10 Notatki/EGZ INŻ 5.13 – Regulacja prędkości obrotowej silników prądu stałego#^682474\|regulacja bocznikowa]]
		* Maksymalne wykorzystanie tej metody osiąga się, gdy
			* w obwodzie twornika (stojana) płynie prąd znamionowy (w zakresie $0\div n_{n}$) – wtedy mamy przez cały czas stały moment znamionowy
			* a powyżej momentu znamionowego przy malejącym wartości momentu i stałe mocy
		* Przy intensywny hamowaniu, jeśli zmniejszymy wzbudzenie prądnicy, że jej napięcie będzie mniejsze, niż wartość indukowanego napięcia w silniku DC, to wówczas silnik DC staje się prądnicą, prądnica sterująca zaczyna pracować jako silnik synchroniczny napędzając silnik M1, który zaczyna pracę jako prądnica oddając energię elektryczną do sieci
		* Każda maszyna w tym układzie powinna mieć moc znamionową silnika roboczego