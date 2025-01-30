---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 5.01 – Straty mocy czynnej w ferromagnetyku przy polu sinusoidalnie zmiennym – geneza, zależności, skutki (przykłady)/","tags":["wiedza/zettel"]}
---

* ## Geneza
	* gdy przemagnesowujemy jakiś materiał, to domeny magnetyczne pod wpływem pola magnetycznego, *chcą* się dostosować do nowego pola, ułożyć inaczej
* Straty dzielimy na:
* ## [[10 Notatki/Straty jałowe\|Straty jałowe]]
	* głównie o te się rozchodzi
	* **przyjmuje się, że nie są one zależne od temperatury rdzenia i są uznawane jako straty stałe, niezależne od obciążenia**
	* ### [[10 Notatki/Straty histerezowe\|Straty histerezowe]]
{ #0995d3}

		* wynikają z cyklicznego magnesowania i rozmagnesowywania materiału ferromagnetycznego w zmiennym polu magnetycznym
			* podczas zmiany pola magnetyczne, wewnętrzne domeny magnetyczne w ferromagnetyku zmieniają swój układ, co wymaga energii
			* Ta energia jest pożytkowana na przezwyciężenie tarcia magnetycznego
		* #### zależą od
			* **częstotliwości**
			* **powierzchni pętli**
				* w [[10 Notatki/Blacha anizotropowa transformatorowa\|Blacha anizotropowa transformatorowa]] zależy od wartości i kierunku indukcji względem kierunku walcowania
					* Przy walcowaniu blachy ziarna układane są w pewien, określony sposób
					* Magnesowanie zgodne z kierunkiem walcowania powoduje zmniejszone pole powierzchni pętli histerezy (mniejsze straty)
					* W taki sposób projektuje się właśnie rdzenie transformatorów
					* Np. w narożnikach może dochodzić do lokalnych przegrzań ze względu na zmianę kierunku walcowania względem 
				* od stanu odprężenia (wyżarzenia)
					* Walcowanie powoduje duże naprężenia mechaniczne, co powoduje trudności i straty w przemieszczaniu się domen
					* Wyżarzenie blachy (podniesienie jej temperatury) powoduje dysfazję atomową – cząstki układają się lepiej; zmniejsza to napięcia mechaniczne i straty, a więc zawęża pętlę histerezy.
	* ### [[10 Notatki/Straty od prądów wirowych\|Straty od prądów wirowych]]
		* zgodnie z [[10 Notatki/SEM (Prawo Faradaya)\|SEM (Prawo Faradaya)]], zmienne pole magnetyczne powoduje powstanie siły elektromotorycznej, która to powoduje przepływ prądu
			* Skoro strumień w rdzeniu się zmienia, to powoduje to wystąpienie siły elektromotorycznej i przepływ prądu
			* Prąd ten przepływając przez rdzeń powoduje straty (przemianę w ciepło) – zgodnie z [[10 Notatki/Prawo Joula\|Prawo Joula]]
		* #### zależne od
			* jakości zaplatania blach
				* każda blacha w rdzeniu jest pokryta lakierem, który pełni rolę izolacji elektrycznej, by zmniejszyć obwody prądów wirowych
				* złe zaplatanie blach może prowadzić do
					* zarysowania, uszkodzenia lakieru na blachach
					* nierównego ułożenia
					*  prze powyższe do zwarć i zwiększenia obwodów prądów wirowych i większych stray
			* grubości blach
				* im cieńsze blachy, tym lepiej
				* obecnie standard to blachy o grubości ok. 0,3-0,4 mm
				* cieńsza blacha => mniejszy (krótszy) obwód elektryczny prądu wirowego => mniejsze straty
			* obecności zadziorów
				* mogą powodować uszkodzenia lakieru i izolacji, a więc zwiększenie obwodów prądów wirowych
				* zakłócają jednorodność pola
				* powodują lokalne koncentracje strumienia magnetycznego, co prowadzi do większych strat w tych miejscach
				* ostrza mogą indukować dodatkowe lokalne prądy wirowe
	* ### Straty dodatkowe (obu rodzajów)
		* powodowane m. in przez
			* nierównomierną indukcję
			* zjawisko wirowania strumienia w węźle środkowym
			* zmiany kierunku linii sił w narożnikach i w miejscach zaplatania
			* jarzma i kolumny w transformatorach pięciokolumnowych
				* ponieważ strumień w tych częściach jest odkształcony
	* ### Podsumowanie [[10 Notatki/Straty jałowe\|Straty jałowe]]
		* W blasze anizotropowej, wartości strat histerezowych i wirowopradowych przy częstotliwości 50 Hz są mniej więcej takie same.
		* Przy stałej częstotliwości i sinusoidalnym strumieniu straty jałowe $\Delta P_{o}$ obliczyć można ze wzoru:
			* $\Delta P_{0}=\Delta p_{1,5}*(\frac{B_{max}}{1,5})^3*m_{Fe}*k_{d_{0}}$
				* $\Delta p_{1,5}$ – stratność blachy przy $B_{max}=1,5 \space \text{T}$ mierzona małym aparatem Epsteina
				* $m_{Fe}$ – masa rdzenia (lub równoważnego fragmentu rdzenia)
				* $k_{d_{0}}$ – współczynnik strat dodatkowych ($k_{d_{0}}=1,2\div{1},4$)
* ## [[10 Notatki/Straty obciążenia\|Straty obciążenia]]
	* podstawowe (w miedzi)
	* ### dodatkowe
		* prądy wirowe wzbudzone strumieniem rozproszenia we wszystkich metalowych elementach
{ #c37240}

			* uzwojenia – przewodzące prąd i wyłączone
			* elementy konstrukcyjne
			* kadź
			* ekrany
		* straty te są proporcjonalne do kwadratu prądu
		* ich zależność od temperatury nie jest jednoznaczna
			* część wraz ze wzrostem temperatury maleje
			* część rośnie
			* część się nie zmienia
		* W temperaturze t0 75 st C nawet kilkadziesiąt procent strat podstawowych
		* W celu ich zmniejszenia
			* buduje się ekrany elektromagnetyczne
				* osłony miedziane lub aluminiowe, które nie dopuszczają strumienia rozproszonego do elementów konstrukcyjnych lub kadzi
			* Ekrany magnetyczne
				* boczniki z blach z blach transformatorowych, tworząc drogę do zamykania strumienia rozproszonego