---
{"dg-publish":true,"permalink":"/10 Notatki/Dobór nastaw regulatora/","tags":["wiedza/definicja"]}
---

>w celu przygotowani się przestudiować instrukcję i sprawozdanie z ćwiczenia PID

* ## Zmienne (nastawy), które podlegają regulacji
	* Jaki widać z równania transmitancji 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/10-notatki/regulator-pid/#c15612" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



	* Transmitancja 

</div></div>

	* zmienne to:
		* $k_{reg}(s)$ – współczynnik proporcjonalności
			* w regulatorach przemysłowych mowa jest raczej o zakresie proporcjonalności $X_{P}$
				* $X_{p}=\frac{1}{k_{reg}}*100\%$
				* Procentowa część pełnego zakresu zmian wielkości wejściowej
					* czyli uchybu $\varepsilon$
				* potrzebną do wywołania pożądanej wielkości wyjściowej $u$ przy założeniu, że operacje całkowania i różniczkowania są wyłączone
		* $T_{i}$ – czas zdwojenia 
			* intensywaność działa całkującego
			* Na wykresie działania regulatora PI, bez różniczkowania, w chiwli $t=T_i$ wartość sygnału na wyjściu jest równa podwójnej amplitudzie skoku na wejściu
			* Dzięki działaniu całkującemu możliwe jest sprowaddzenie uchybu regulacji w stanie ustalonym do 0
		* $T_d$ – czas wyprzedzania
			* Dzięki odpowiedniemu odborowi, regulator może bardzo silnei reagować nawet na niewielkie, lecz szybkie zmiany uchybu $\varepsilon$
			* Przez odpowiednio silne oddziaływanie na wejście obiektu przeciwdziała dalszemu wzrostowi tego uchybu
	* Czyli w skrócie
		* całkowanie – pozwala sprowadzić uchyb do 0
		* różniczkowanie – antycypuje, przewiduje i zmniejsza wartość uchybu (bo wie, co się zaraz będzie działo)
* ## Algorytm wyznaczania nastaw w zależności od typu układu
	* Jeżeli:
			* Mamy układ  [[10 Notatki/Układy sterujące a regulacji#^cc6781\|regulacji stałowartościowej / stabilizacji]]
			* Jest to [[10 Notatki/Układy sterujące a regulacji#^243423\|układ otwarty]] (bez pętli sprzężenia zwrotnego)
		* to należy wybrać jedno z założeń
			1. Przebieg aperiodyczny (tzw. ładowanie kondensatora)
				* i jednocześnie jak najkrótszy czas regulacji
			2. Przebieg oscylacyjny
				+ + dopuszczalne przeregulowanie $\Delta y=20\%$ 
				+ + minimalny czas regulacji
			3. Przebieg zapewniający minimum z całki z kwadratu uchybu
				* inaczej – wymóg zużycia minimalnej ilości energii w procesie dochodzenia do wartości zadanej
		* W przypadku [[10 Notatki/Regulacja nadążna\|Regulacja nadążna]] optymalne nastawy regulatora wyznacza się z innych zależności
	* W przypadku [[10 Notatki/Układy sterujące a regulacji#^c15323\|układu zamkniętego]] należy skorzystać z [[10 Notatki/Metoda Zieglera i Nicholsa\|Metoda Zieglera i Nicholsa]]
	* Po zastosowaniu tej metody w efekcie pobocznym uzyskujemy oscylacje o amplitudzie trudnej do przewidzenia, więc np. w niektórych procesach technologicznych może to być niedopuszczalne