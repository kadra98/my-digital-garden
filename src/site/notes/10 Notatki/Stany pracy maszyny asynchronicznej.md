---
{"dg-publish":true,"permalink":"/10 Notatki/Stany pracy maszyny asynchronicznej/","tags":["wiedza/zettel"]}
---

* ![Pasted image 20250123205429.png](/img/user/80%20Zasoby/Pasted%20image%2020250123205429.png)
* ![Pasted image 20250123212616.png](/img/user/80%20Zasoby/Pasted%20image%2020250123212616.png)
* ## Transformator
{ #8d179e}

	* ### Sposób działania
		* Podłączamy stojan do sieci
		* Rozwieramy obwód wirnika
		* W wirniku indukuje się napięcie, ale nie płynie prąd, bo jest rozwarty
			* Transformator w stanie jałowym
		* Unieruchamiamy wirnik
		* Zamykamy obwód włączając odbiorniki
			* Transformator w stanie obciążenia
			* Moc elektryczna z sieci zmienia się w moc elektryczną o niższym napięciu
			* Ta sama częstotliwość, co w sieci
		* Jeśli pierścienie byśmy zwarli, lub próbowali to zrobić w [[10 Notatki/silnik klatkowy\|silniku klatkowym]], to będziemy mieli
			* Transformator w stanie zwarcia
	* ### Zastosowanie
		* przesuwnik fazowy
		* regulator napięcia
	* należy pamiętać, że unieruchomiony wirnik znacząco pogarsza chłodzenie i powoduje znaczny wzrost strat w uzwojeniu wirnika
* ## Praca silnikowa
{ #6d3697}

	* klasyka gatunku, temat ten omówiony już w [[10 Notatki/Maszyna asynchroniczna (indukcyjna)\|Maszyna asynchroniczna (indukcyjna)]]
* ## Idealny bieg jałowy
	* w naturze nie występuje, silnik musiałby osiągnąć prędkość synchroniczną, a ze względu na tarcie i opory powietrza, nie jest to możliwe – [[10 Notatki/Dlaczego silnik asynchroniczny nigdy nie uzyska prędkości  synchronicznej\|Dlaczego silnik asynchroniczny nigdy nie uzyska prędkości  synchronicznej]]
* ## Praca prądnicowa
{ #6f77e5}

	* ### Zasada działania
		* wał / wirnik obraca się szybciej, niż prędkość synchroniczna
		* zmienia się kierunek wirowania wirnika względem pola
			* w [[10 Notatki/EGZ INŻ 5.08 – Bilans mocy czynnej i strat przy pracy silnikowej, hamulcowej i prądnicowej maszyny indukcyjnej (schemat zastępczy, kierunki przepływu mocy)#^6d3697\|pracy silnikowej]] wirnik *gonił* wirujące pole, więc względem wirnika pole wirowało np. w prawo
			* gdy wirnik obraca się szybciej niż pole, to tak, jakby wirowało ono w drugą stronę
		* prowadzi to do
			* zmiany zwrotu napięcia w wirniku
			* zmiany zwrotu prądu w wirniku
			* zmiany zwrotu momentu elektromagnetycznego, czyli siły działającej na wał [[10 Notatki/Siła Lorentza\|Siła Lorentza]]
				* czyli wirnik jest hamowany – chce wrócić co najmniej do biegu jałowego, albo prędkości znamionowej
				* by się temu przeciwstawić – musimy dostarczać energię, by kręcić wałem
					* czyli przekształcamy energię mechaniczną, którą dostarczamy na wał, na elektryczną wydawaną do sieci
			* wtedy to stojan znajduje się w zmieniającym się polu magnetycznym, dzięki któremu w uzwojeniu stojana zostaje wyindukowane napięcie, które jest zwracane do sieci
	* ### Zastosowanie
		* wytwarzanie energii elektrycznej – np. farmy wiatrowe
			* tutaj istotne jednak, by tego typu prądnica była podłączona do źródła, z którego mogłaby pobierać moc bierną indukcyjną np. [[10 Notatki/Maszyna synchroniczna, generator, prądnica\|Maszyna synchroniczna, generator, prądnica]], niezbędną do wzbudzenia pola magnetycznego
		* hamowanie
* ## Praca hamulcowa
{ #8ab4b8}

	* ### Zasada działania
		* wirnik obraca się w przeciwną stronę, niż wiruje pole
		* kierunek wirowania pola taki sam, jak przy [[10 Notatki/EGZ INŻ 5.08 – Bilans mocy czynnej i strat przy pracy silnikowej, hamulcowej i prądnicowej maszyny indukcyjnej (schemat zastępczy, kierunki przepływu mocy)#^6d3697\|pracy silnikowej]] i [[10 Notatki/EGZ INŻ 5.08 – Bilans mocy czynnej i strat przy pracy silnikowej, hamulcowej i prądnicowej maszyny indukcyjnej (schemat zastępczy, kierunki przepływu mocy)#^8d179e\|pracy transformatorowej]]
			* zwroty napięcia i prądu w wirniku również bez zmian
		* w takim układzie [[10 Notatki/Siła Lorentza\|moment elektromagnetyczny]] ma przeciwny zwrot, niż kierunek obracania się wirnika
			* ten moment to moment hamujący
		* maszyna w tym stanie pobiera prąd z sieci elektrycznej w obwodzie stojana, która wraz z mocą mechaniczną jest przekazywana do urządzeń włączonych w obwód wirnika, lub w maszynie klatkowej zamienia się całkowicie w ciepło (straty)
		* Czyli na prosty rozum
			* Jedziemy, wał obraca się w prawo
			* Za bardzo się rozpędziliśmy, musimy wyhamować
			* Zamieniamy kolejność faz
			* Tak uzyskujemy to, że kierunek wirowania pola jest przeciwny do kierunku wirowania wirnika
			* I w ten sposób uzyskujemy przeciwny zwrot siły / momentu, który hamuje
	* ### Zastosowanie
		* ze względu na fakt, że wraz ze zmianą obciążenia, częstotliwość w obwodzie wirnika się zmienia, układ ten jest rzadko stosowany jako prądnica
		* inaczej tzw. hamowanie prądem, lub przeciwłączenie