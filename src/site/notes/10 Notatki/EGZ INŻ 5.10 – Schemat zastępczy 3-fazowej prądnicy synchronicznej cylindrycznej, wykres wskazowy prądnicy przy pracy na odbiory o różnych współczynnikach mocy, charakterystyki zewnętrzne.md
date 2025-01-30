---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 5.10 – Schemat zastępczy 3-fazowej prądnicy synchronicznej cylindrycznej, wykres wskazowy prądnicy przy pracy na odbiory o różnych współczynnikach mocy, charakterystyki zewnętrzne/","tags":["wiedza/zettel"]}
---

* ## Maszyna nienasycona vs. nasycona
	* O stanie nasycenia obwodu magnetycznego maszyny decyduje przede wszystkim strumień główny
	* Za miarę tego strumienia głównego możemy uważać napięcie E indukowane przez ten strumień
	* O stanie nasycenia obwodu magnetycznego maszyny decyduje przede wszystkim strumień główny
	* ### Maszyna nienasycona
{ #f80828}

		* Rdzeń magnetyczny prądnicy (czyli i stojana i wirnika) jest zdolny do efektywnego przewodzenia strumienia magnetycznego
		* $\Phi ∝ I_{w}$
			* $I_{w}$ – prąd wzbudzenia (płynący w uzwojeniu wirnika)
		* W tej części charakterystyki magnesowani (liniowej), zwiększanie prądu wzbudzenia zwiększa strumień, a strumień zwiększa napięcie
	* ### Maszyna nasycona
{ #6bde79}

		* Taka maszyna, której obwód magnetyczny pracuje w obszarze wykraczającym poza prostoliniową w część charakterystyki magnesowania.
		* Materiał osiąga maksymalną zdolność do przewodzenia strumienia
		* Przy dalszym zwiększaniu prądu wzbudzenia wzrost strumienia jest nieliniowy, aż w pewnym momencie jego dalszy wzrost przestaje powodować wzrost strumienia
		* W stanie tym, lub jego bliskim, wszystkie, albo zdecydowana większość domen magnetycznych, są już uporządkowane
	* ### Skutki przejścia maszyny w stan nasycenia
		* Dalsze zwiększanie prądu wzbudzeni przestaje proporcjonalnie zwiększać napięcie generowane w prądnicy
		* W związku z tym, że strumień nie zmienia się już tak dynamicznie, to maleje reaktancja magnesująca $X_{m}$
			* Wpływa to na stabilność napięcia generowanego przez prądnicę
		* Straty mocy spowodowane zwiększonymi stratami histerezowymi i większymi prądami wirowymi, ponieważ pole magnetyczne w rdzeniu przestaje zmieniać się liniowo
		* Efekt nasycenia ogranicza maksymalną wartość napięcia, które można uzyskać z prądnicy przy danym prądzie wzbudzenia
* ## Schemat
	* ### Maszyna nienasycona
	* ![Pasted image 20250126094112.png](/img/user/80%20Zasoby/Pasted%20image%2020250126094112.png)
		* $E_{w}$ – napięcie indukowane w uzwojeniu twornika przez strumień $\Phi_{W}$
			* ![Pasted image 20250126094532.png](/img/user/80%20Zasoby/Pasted%20image%2020250126094532.png) 
			* **strumień wzbudzenia – główny strumień, który generuje napięcie w tworniku**
		* $X_{ad}$ – reaktancja oddziaływania twornika odpowiadająca strumieniowi $\Phi_{a}$, który indukuje się w uzwojeniu twornika napięcie $E_{a}$
			* ![Pasted image 20250126094656.png](/img/user/80%20Zasoby/Pasted%20image%2020250126094656.png)
			* **strumień oddziaływania twornika**
				* $\Phi_{a}$, który indukuje napięcie $E_{a}$, które sprzęga stojan i wirnik
		* $X_{s}$  reaktancja rozproszenia twornika, odpowiadająca strumieniowi $\Phi_{s}$, który indukuje w uzwojeniu twornika napięcie $E_{s}$
			* ![Pasted image 20250126094817.png](/img/user/80%20Zasoby/Pasted%20image%2020250126094817.png)
			* $\Phi_{s}$ – strumień rozproszenia twornika
		* $E$ – *realne* napięcie, które indukuje prądnica
			* Jego wartość, albo stosunek do napięcia sieciowego $U$, zależy od tego , czy [[10 Notatki/Jak maszyna synchroniczna wytwarza moc bierną\|maszyna synchroniczna wytwarza, czy pobiera moc bierną]]
		* $R$  rezystancja uzwojenia twornika
	* ### Maszyna nasycona
		* ![Pasted image 20250129214401.png](/img/user/80%20Zasoby/Pasted%20image%2020250129214401.png)
		* nie ma $X_{ad}$ (reaktancji twornika), ponieważ jest już w pełni *zmagnetyzowany*, nie jest on już odbiornikiem reaktancyjnym i moc bierną oddaje do sieci
		* pozostaje jedynie niewielka wartość reaktancji $X_{s}$ 
* ## Wykresy wskazowe
	* ### Praca na odbiór indukcyjny
		* ![Pasted image 20250129221945.png](/img/user/80%20Zasoby/Pasted%20image%2020250129221945.png)
			* Przez charakter indukcyjny odbioru, strumień twornika $\Theta_{E}$ jest nieco mniejszy, co przekłada się na mniejsze napięcie na zaciskach zewnętrznych $E$ (bo mniejsze [[10 Notatki/SEM (Prawo Faradaya)\|SEM (Prawo Faradaya)]], a więc i mniejsze napięcie na zaciskach $U$
				* Do celów kreślenia wykresów, warto zacząć od wyrysowania wektora napięcia $U$, a następnie za pomocą spadku napięcia na rezystancji twornika $RI$ oraz spadku napięcia na indukcji rozproszenia $jX_{s}I$ wykreślić wektor $E$
			* Napięcie $U$ wyprzedza prąd $I$ $(\text{CIUL})$
	* ### Praca na odbiór pojemnościowy
		* ![Pasted image 20250129222014.png](/img/user/80%20Zasoby/Pasted%20image%2020250129222014.png)
		* ze względu na wzrost namagnesowania twornika, strumień $\Theta_{w}$ jest większy, więc większe jest i napięcie indukowane przez twornik $E$
		* prąd $I$ wyprzedza napięcie $U$ $(\text{CIUL})$
		* $\Theta_{W}$ – strumień wirnika – stały
		* spadki napięcia $RI$ oraz $jX_{s}I$ – stałe
* ## Charakterystyki zewnętrzne
	* ![Pasted image 20250129220359.png](/img/user/80%20Zasoby/Pasted%20image%2020250129220359.png)
		* $E_{w}=\text{const}$
		* $I_{w}=\text{const}$
	* Im więcej mocy biernej maszyna oddaje do sieci (obciążenie o charakterze indukcyjnym), tym mniejsze jest napięcie na zaciskach prądnicy
		* No bo moc bierna, która jest wymagana do wyindukowania w tworniku napięcia, jest częściowo zabierana i rozmagnesowuje twornik
	* Jeśli jednak przyłączymy odbiór o charakterze pojemnościowym, to cała moc bierna wytwarzana przez prądnice jest zachowywana w tworniku (albo i jest jej dostarczane więcej przez sieć), co wzmaga namagnesowanie twornika, a więc i napięcie.