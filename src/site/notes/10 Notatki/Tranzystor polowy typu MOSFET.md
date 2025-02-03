---
{"dg-publish":true,"permalink":"/10 Notatki/Tranzystor polowy typu MOSFET/","tags":["wiedza/zettel"]}
---

* ## Budowa
	* ![Pasted image 20250203215515.png](/img/user/80%20Zasoby/Pasted%20image%2020250203215515.png)
	* nawet w zubożony polu P znajduje się wolne elektrony
	* bramkę od źródła oddziela bardzo wąska warstwa dielektryka (patrz poniżej zasada działania), który może zostać przebity w przypadku zbyt wysokiego napięcia
* ## Zasada działania
	* na podstawie kanału wzbogaconego typu P
	* zasada podobna do działania jak w przypadku kondensatora
		* po podłączeniu kondensatora do źródła DC, w stanie nieustalony elektrony z jednej okładki przepłyną w kierunku + źródła zasilania, a z – źródła przepłyną do drugiej okładki, tworząc tym samym stan ustalony
		* prąd przez kondensator nie płynie, jednak w stanie nieustalony elektrony się w pewnym sensie repozycjonują
	* analogicznie działa to w przypadku podłączenia dwóch końców zasilania do dwóch stron warstwy zubożonej
		* ![Pasted image 20250203220612.png](/img/user/80%20Zasoby/Pasted%20image%2020250203220612.png)
		* elektrony z jednej *okładki* podłączonej między 2 pola N odpłyną do źródła, tworząc na tej okładce pole +, zaś z drugiej strony wpłyną
	* pole elektryczne wytworzone przez okładkę ze znakiem + przyciąga wolne elektrony z warstwy P (po to są te wolne elektrony w warstwie zubożonej)
		* elektrony te wypełniają wolne dziury w tym miejscu warstwy zubożonej, a pozostałe pozostają wolnymi
			* zatem to miejsce tak naprawdę w momencie zrepozycjowania się elektronów staje się tak jakby polem N (posiadającym nadmiar elektronów)
				* to miejsce (kanał) pozwala na swobodny przepływ elektronów, jeśli do dwóch pól N podłączymy źródło zasilania
					* ![Pasted image 20250203221119.png](/img/user/80%20Zasoby/Pasted%20image%2020250203221119.png)
	* w przypadku zbyt słabego zasilenia bramki napięciem, wytworzone pole przez bramkę będzie zbyt słabe, by wytworzyć kanał do swobodnego przepływu elektronów
* ## Przewagi tranzystora typu MOSFET nad [[10 Notatki/Tranzystor bipolarny (BJT– ang. Bipolar junction transistor)\|tranzystorem typu BJT]]
	* Tranzystory typu MOSFET nie marnują energii w stanie *włączenia*, tak jak robią to [[10 Notatki/Tranzystor bipolarny (BJT– ang. Bipolar junction transistor)\|tranzystory bipolarne]]
	* Nośnikiem ładunku są tylko elektrony lub dziury, więc są one cichsze, niż BJT
* ## Symbole i typy
	* ![Pasted image 20250203223607.png](/img/user/80%20Zasoby/Pasted%20image%2020250203223607.png)
	* literka B oznacza *body* (podłoże) i zasadniczo jest połączona ze źródłem
* ## Właściwości
	* Krótkie czasy przełączania
	* Zastosowanie w przekształtnikach wysokoczęstotliwościowych
	* Łatwość łączenia równoległego, umożliwiająca uzyskanie dużej obciążalności prądowej zaworu
	* Dość wysoka wartość rezystancji w stanie przewodzenia
* ## Parametry
	* maksymalny prąd drenu
		* maksymalny prąd, jakim można sterować za pomocą tranzystora
		* maksymalne napięcie dren-źródło
		* maksymalna moc strat
			* wynika z nagrzewania się tranzystora
* ## Charakterystyka
	* ![Pasted image 20250203224059.png](/img/user/80%20Zasoby/Pasted%20image%2020250203224059.png)
	* 3 obszary pracy – takie same jak w przypadku BJT:
		* odcięcia
		* aktywny
		* rezystancyjny (liniowy) – stan pracy normalnej. Wówczas można zastąpić tranzystor w teorii obwodów rezystancją w stanie przewodzenia $R_{DS}$ (dana z karty katalogowej producenta)