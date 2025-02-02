---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 2.01 – Diody – rodzaje, właściwości i zastosowanie/","tags":["wiedza/zettel"]}
---

* ## Właściwości [[10 Notatki/Dioda\|diod]] mocy
	* ### Wysoka wytrzymałość prądowa
		* #### Duża powierzchnia złącz półprzewodnikowego
			* Obniża gęstość prądu
			* Zapobiega lokalnym przegrzaniom
		* #### Zastosowanie półprzewodników o niskiej rezystywności (gruba warstwa typu N)
			* np. krzem  o małej domieszce
			* obniżenie rezystancji przewodzenia zmniejsza spadek napięcia w kierunku przewodzenia
	* ### Duże napięcie przebicia
		* #### Gruba warstwa półprzewodnikowa w obszarze złącza P-N
			* Większa odległość między warstwami P i N oznacza, że pole elektryczne rozkłada się na większej przestrzeni, co podnosi wartość napięcia przebicia
		* #### Specjalne domieszkowanie warstwy półprzewodnikowej
			* Gradientowe przejście między warstwami P i N sprawia, że złącze lepiej rozprasza pole elektryczne, zmniejszając ryzyko przebicia lawinowego
			* Dioda ma strukturę P+, N-, N+ – warstwa N- (słabo domieszkowana) zwiększa napięcie przebicia
		* #### Konstrukcja ograniczająca efekt koncentracji pola elektrycznego
			* Zaokrąglone krawędzi złącza P-N – zapobiegają miejscowej koncentracji pola elektrycznego, co mogłoby powodować przedwczesne przebicie
		* #### Zastosowanie odpowiedniego materiału półprzewodnikowego
			* Zastosowanie węglika krzemu (przy diodach bardzo wysokiego napięcia), który pozwala osiągnąć napięcie przebicia > 1kV przy mniejszej rezystancji i wyższej sprawności
	* ### Odprowadzanie ciepła
		* #### Mocne połączenia z elektrodami
			* Warstwa metaliczna na powierzchni diody zapewnia dobre połączenie z obwodem i szybkie odprowadzanie ciepła
			* Stosuje się grube wyprowadzenia, które są w stanie przewodzić duży prąd bez przegrzewania się
		* #### Efektywne odprowadzanie ciepła
			* podłoże miedziane lub molibdenowe, które dobrze przewodzi ciepło i zapewnia szybkie chłodzenie struktury P-N
			* Montaż na radiatorze lub kapsuły metalowe
* ## Podział diod ze względu na czas przełączania i ich zastosowania

| nazwa diody       | konwencjonalna prostownicza        | szybkie                                                | Ultraszybkie                 | Schottky'ego                                  |
| ----------------- | ---------------------------------- | ------------------------------------------------------ | ---------------------------- | --------------------------------------------- |
| czas przełączania | $50\div 20 \space \micro \text{s}$ | $200\div 25 \space \micro \text{s}$                    | $50\div 10 \space \text{ns}$ | $5\div 1 \space \text{ns}$                    |
| zastosowanie      | – prostowniki<br>– zasilacze       | – zasilacze impulsowe<br>– przetworniki<br>– inwertery |                              | – zasilacze impulsowe<br>– przetworniki DC-DC |
* ## Omówienie rodzajów diod
	* ### Dioda prostownicza
	* 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/10-notatki/dioda-prostownicza/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




* najbardziej standardowy typ [[10 Notatki/Dioda\|diody]], używany głównie do prostowania prądu zmiennego na stały w aplikacjach takich jak zasilacze i układy energetyczne
* Charakteryzują się stosunkowo wysokim napięciem przewodzenia i przeznczone są do pracy w dużych prądach i napięciach
* #### Zastosowanie
	* prostowniki
	* zasilacze
* ![Pasted image 20250202111318.png](/img/user/80%20Zasoby/Pasted%20image%2020250202111318.png)
* ![Pasted image 20250202111327.png](/img/user/80%20Zasoby/Pasted%20image%2020250202111327.png)

</div></div>

	* ### Dioda szybkia
	* 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/10-notatki/dioda-szybka/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




* krótki czas przełączania [[10 Notatki/Dioda\|diody]], co pozwala na ich zastosowanie , gdzie kluczowa jest szybka odpowiedź przy przełączaniu
	* Wysoka szybkość wyłączania jest kluczowa w systemach zasilania impulsowego
* #### Zastosowanie
	* przetwornice
	* Inwertery
	* Zasilacze impulsowe

</div></div>

	* ### Dioda Schottky'ego
	* 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/10-notatki/dioda-schottky-ego/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




* [[10 Notatki/Dioda\|Diody]] te wykorzystują złącze metal-półprzewodnik zamiast złącza P-N, co pozwala na osiągnięcie
	* niskiego napięcia przewodzenia ($0,2\div 0,3 \space \text{V}$)
	* szybkiego czasu przełączania
* Z powodu niskich strat mocy często stosowane w aplikacjach o wysokiej częstotliwości
* #### Zastosowanie
	* Zasilacze impulsowe
	* Przetwornice DC-DC
* ![Pasted image 20250202111904.png](/img/user/80%20Zasoby/Pasted%20image%2020250202111904.png)
* ![Pasted image 20250202111911.png](/img/user/80%20Zasoby/Pasted%20image%2020250202111911.png)

</div></div>
