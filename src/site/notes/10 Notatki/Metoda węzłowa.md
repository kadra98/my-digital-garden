---
{"dg-publish":true,"permalink":"/10 Notatki/Metoda węzłowa/","tags":["wiedza/zettel"]}
---

1. uziemiamy jeden węzeł, najlepiej taki, który jest z dupy strony gałęzi, na której jest źródło napięciowe, i na której gałęzi nie ma żadnych impedancji
	* bo wtedy automatycznie znamy wartość potencjału na kolejnym węźle, niech będzie to węzeł $V_{1}$
2. dla węzła, dla którego chcemy obliczyć potencjał ($V_{2}$)
	* $V_{2}\left( \frac{1}{R_{1}}+\frac{1}{R_{2}+R_{3}}+\frac{1}{R_{45}} \right)\pm \frac{V_{1}}{R_{1}}=\frac{\pm E}{R_{2}}\pm I$
		* 1 składnik
			* szukany potencjał węzła pomnożony przez sumę, na kórą składają się odwrotności impedancji gałęzi, które schodza się do węzła
				* jak widać, jeśli układ jest taki, że na jednej gałęzi schodzacej się do węzła jest więcej niz jeden rezystor, to trzeba uwzględnić rezystancję zastępczą dla tej gałęzi
			* **uwaga**
				* nie bierzemy do równania rezystancji, które znajduja się na gałęzi ze źródłem praadowym!
			* 
3. dsc