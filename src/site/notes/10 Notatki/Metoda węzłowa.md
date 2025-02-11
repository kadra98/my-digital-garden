---
{"dg-publish":true,"permalink":"/10 Notatki/Metoda węzłowa/","tags":["wiedza/zettel"]}
---

1. uziemiamy jeden węzeł, najlepiej taki, który jest z dupy strony gałęzi, na której jest źródło napięciowe, i na której gałęzi nie ma żadnych impedancji
	* bo wtedy automatycznie znamy wartość potencjału na kolejnym węźle, niech będzie to węzeł $V_{1}$
2. dla węzła, dla którego chcemy obliczyć potencjał ($V_{2}$)
	* $V_{2}\left( \frac{1}{R_{1}}+\frac{1}{R_{2}+R_{3}}+\frac{1}{R_{45}} \right)- \frac{V_{1}}{R_{1}}=\frac{\pm E}{R_{2}}\pm I$
		* 1 składnik
			* szukany potencjał węzła pomnożony przez sumę, na którą składają się odwrotności impedancji gałęzi, które schodzą się do węzła
				* jak widać, jeśli układ jest taki, że na jednej gałęzi schodzącej się do węzła jest więcej niż jeden rezystor, to trzeba uwzględnić rezystancję zastępczą dla tej gałęzi
			* **uwaga**
				* nie bierzemy do równania rezystancji, które znajdują się na gałęzi ze źródłem prądowym!
		* 2 składnik
			* odejmujemy potencjał węzła (węzłów), które sąsiadują z obliczanym węzłem $V_{2}$
				* w tym przypadku węzeł $V_{1}$
			* podzielony przez rezystancję, która oddziela oba węzły
		* prawa strona równania
			* źródła napięciowe dopływające do węzła podzielone przez rezystancję na tej gałęzi
				* znak jest zdeterminowany przez kierunek źródła
					* jeśli strzałka do obliczanego węzła – $+$
						* źródło *wspomaga* węzeł, dodaje do niego napięcie
					* jeśli od źródła, znak $–$
						* źródło zaciąga napięcie z węzła
			* jest to bazowo równanie prądów, więc dodajemy / odejmujemy połączone z węzłem źródła prądowe
				* wg zasady jak dla zwrotów źródeł napięciowych
3. rozwiązujemy równanie / układ równań, wyznaczając potencjał źródła / źródeł
4. Obliczamy prądy z prawa Ohma
	* $I_{n}=\frac{dV}{R_{n}}$
		* pamiętając, by w liczniku ułamka uwzględniać różnice potencjałów między węzłami plus ewentualne źródła
			* kierunek źródła zgodny ze zastrzałkowanym prądem
				* źródło ze znakiem $+$ i od niego odejmujemy obliczony potencjał węzła
5. obliczam prądy z prawa Kirchhoffa
6. nie zapominamy obliczyć spadku napięcia na źródle prądowym
7. Dla sprawdzenia rysujemy graf przepływu prądów
8. Obliczamy moc wydawaną
	* $P_{wyd}=\Sigma U_{źr}I_{źr}$
9. Obliczamy moc pobieraną przez odbiorniki
	* $P_{pob}=\Sigma R_{odb}I_{odb}^2$