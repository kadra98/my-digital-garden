---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 5.07 – Schemat zastępczy 3-fazowej maszyny indukcyjnej i interpretacja jego parametrów/","tags":["wiedza/zettel"]}
---

* ## Schemat
	* ![Pasted image 20250123185914.png](/img/user/80%20Zasoby/Pasted%20image%2020250123185914.png)
* ## Parametry
	* $U_{s}$ – napięcie na stojanie
	* $R_{s}$ – rezystancja stojana
	* $X_{s}$ – reaktancja rozproszenia stojana
		* podobniej jak w przypadku [[10 Notatki/EGZ INŻ 5.02 – Schemat zastępczy transformatora 3-fazowego i interpretacja jego parametrów#^0e3f25\|reaktancji strumienia rozproszonego w transformatorze]], reaktancja ta jest reaktancją pasożytniczą – strumieniem rozproszonym
		* niestety ze względu na fakt stosowania np. żłobków stojana półdomkniętych lub całkowicie zamkniętych, reaktancje te są dużo wyższe, niż w przypadku transformatorów
		* różne kształty żłobków stosujemy w celu zmniejszenia wpływu wyższych harmonicznych rzędów i ograniczenia przepływy prądów wirowych w wirniku, które przyczyniają się [[10 Notatki/EGZ INŻ 5.01 – Straty mocy czynnej w ferromagnetyku przy polu sinusoidalnie zmiennym – geneza, zależności, skutki (przykłady)\|strat czynnych]] $R_{Fe}$ 
	* $R'_{r}$ – rezystancja wirnika
	* $X'_{lr}$ – reaktancja rozproszenia uzwojenia wirnika
		* ta reaktancja – tutaj podobnie jak w przypadku [[10 Notatki/EGZ INŻ 5.02 – Schemat zastępczy transformatora 3-fazowego i interpretacja jego parametrów#^0e3f25\|reaktancji strumienia rozproszonego w transformatorze]], chcemy, by ta reaktancja była jak najmniejsza, ponieważ przez jej obecność w obwodzie wirnika prąd jest przesunięty względem napięcia, a co istotniejsze – względem miejsca pola, w którym jest ono najsilniejsze – dlatego właśnie stosujemy dodatkową rezystancję w [[10 Notatki/silnik pierścieniowy\|silniku pierścieniowym]], by zmniejszyć jej udział
	* $X_{m}$ – reaktancja główna
		* Dokładnie tak jak w [[10 Notatki/EGZ INŻ 5.02 – Schemat zastępczy transformatora 3-fazowego i interpretacja jego parametrów\|transformatorze]] jest to ta reaktancja, która powoduje przepływ prądu magnesującego i powstanie strumienia głównego, za sprawą którego, w wirniku indukuje się siła elektromotoryczna
			* Niestety, ze względu na konieczność obecności szczeliny powietrznej, reaktancja ta jest słabsza, niż w transformatorze
			* M. in. z tego powodu, ale również ze względu na
				* zwiększenie prądu biegu jałowego
				* pogorszenie się współczynnika mocy
			* szczelina powietrzna powinna być jak najmniejsza
				* jak tylko pozwala nam na to
					* dokładność obróbki i montażu
					* strzałka ugięcia wału
					* rozszerzalność termiczna
	* $R_{Fe}$ – straty czynne
		* związane z przemagnesowywaniem stalowej obudowy stojana
		* nieco mniejsze, ponieważ na drodze strumienia jest jeszcze szczelina powietrzna, której przemagnesowanie nie powoduje strat czynnych
		* podobnie jednak jak w przypadku transformatora, stojan wykonany jest z odizolowanych pierścieni – pakietu blach – celem ograniczenia prądów wirowych.
		* Także podobnie jak w przypadku rdzenia transformatora, jako materiał wykorzystuje się materiał o wąskiej histerezie, by ograniczyć [[10 Notatki/EGZ INŻ 5.01 – Straty mocy czynnej w ferromagnetyku przy polu sinusoidalnie zmiennym – geneza, zależności, skutki (przykłady)#^0995d3\|straty histerezowe]].
	* $R'_{r}(\frac{1-s}{s})$ – rezystancja obciążenia
		* fikcyjna wartość, odpowiadająca obciążeniu wału silnika
		* reprezentuje moc przekazywaną z pola magnetycznego na wirnik
			* $s=\frac{n-n_{w}}{n}$
				* $s$ – poślizg
				* $n$ – prędkość synchroniczna (zależna od par biegunów)
				* $n_{w}$ – prędkość wirnika
		* konieczne jest jest zawarcie w schemacie zastępczym, ponieważ bez niej w obu oczkach panowałyby inne częstotliwości
			* w *oczku* stojana – 50 Hz
			* w *oczku* wirnika – w stanie spoczynku 0 Hz, w trakcie ruchu: $0<f_{w}<50 \space \text{Hz}$
	* Przedstawiony schemat nie uwzględnia wszystkich zjawisk występujących w maszynie. Pominięto m. in.
		* straty w rdzeniu wirnika
		* straty w izolacji
		* prądy pojemnościowe
	* Dla schematu zastępczego [[10 Notatki/silnik pierścieniowy\|silnika pierścieniowego]] szeregowo w gałęzi wirnika wpina się (przynajmniej na czas rozruchu) rezystancję dodatkową