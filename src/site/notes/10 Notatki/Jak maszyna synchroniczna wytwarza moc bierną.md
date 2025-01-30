---
{"dg-publish":true,"permalink":"/10 Notatki/Jak maszyna synchroniczna wytwarza moc bierną/","tags":["wiedza/zettel"]}
---

* O tym, jak jest postrzegana maszyna indukcyjna z punktu widzenia [[SEE\|SEE]], decyduje
		* $Q ∝ (E_{f}-U_{s})$
			* $Q$ – moc bierna prądnicy
{ #624130}

			* $E_{f}$ – [[10 Notatki/SEM (Prawo Faradaya)\|SEM (Prawo Faradaya)]] generowana przez wirnik (prąd wzbudzenia) w stojanie
			* $U_{s}$ – napięcie sieci [[SEE\|SEE]]
	* ### Stan niedowzbudzenia
		* W stanie niedowzbudzenia, czyli głębokim [[10 Notatki/EGZ INŻ 5.10 – Schemat zastępczy 3-fazowej prądnicy synchronicznej cylindrycznej, wykres wskazowy prądnicy przy pracy na odbiory o różnych współczynnikach mocy, charakterystyki zewnętrzne#^f80828\|nienasyceniu]], maszyna ta pobiera moc bierną z sieci moc bierną indukcyjną
		* W stanie tym, zgodnie z [[10 Notatki/Dlaczego prądnica synchroniczna może być źródłem mocy biernej, a prądnica asynchroniczna – nie#^624130\|powyższym równaniem]], napięcie generowane przez prądnicę jest mniejsze, niż napięcie sieci
			* A zatem, zgodnie z definicją pradu, przepływa od z miejsca (w tym przypadku [[SEE\|SEE]]) o wyższym potencjale do miejsca o niższym
				* Czyli w tym wypadku – z sieci do stojana
				* A stojan, jako że jest kupą zwojów, to jest odbiornikiem mocy biernej indukcyjnej
				* Coś go po prostu musi namagnesować, jeśli nie będzie to wirnik, to będzie to sieć
		* Prądnica zachowuje się więc jak wielka cewka w systemie
			* **bo pobiera moc bierna, tak jak właśnie [[10 Notatki/Moc bierna – co ją pobiera, a co ją oddaje#^87ae1a\|cewka]]**
			* Więc moglibyśmy to w uproszeniu zastosować w takiej sieci, w której jest dużo kondensatorów
	* ### Stan przewzbudzenia
		* W przewzbudzenia, czyli maksymalnego [[10 Notatki/EGZ INŻ 5.10 – Schemat zastępczy 3-fazowej prądnicy synchronicznej cylindrycznej, wykres wskazowy prądnicy przy pracy na odbiory o różnych współczynnikach mocy, charakterystyki zewnętrzne#^6bde79\|nasycenia]]i jeszcze dalej, maszyna oddaje do sieci moc bierną pojemnościową
		* Ta reaktancja, którą wytwarza tak wielki strumień, jest tak wielka, że jest wypychana z uzwojenia stojana
		* W efekcie, prądnica oddaje do sieci moc bierną, coś niezbędnego, dla cewek
			* A **skoro oddaje moc bierną, to zachowuje się jak wielki [[10 Notatki/Moc bierna – co ją pobiera, a co ją oddaje#^efa6a9\|kondensator]]**
	* Mozliwe jest takie dostosowanie prądu wzbudzenia, by $\cos\phi$ był równy 1, czyli generował tylko i wyłącznie moc czynną