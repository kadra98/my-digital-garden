---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 1.08 – Analiza obwodu szeregowego i równoległego RLC prądu przemiennego, zjawisko rezonansu, częstotliwość rezonansowa obwodu/","tags":["wiedza/zettel"]}
---

* ## Równania rezonansu
	* $f=\frac{1}{2\pi \sqrt{ LC }}$
		* $f$ – częstotliwość rezonansowa, częstotliwość zasilania z sieci
	* $X_{L}=X_{C}$
	* $\omega L=\frac{1}{\omega C}$
		* ze wzoru na impedancję
		* $Z=R+j(X_{L}-X_{C})$
* ## Rezonans szeregowy
{ #8def59}

	* cewka i kondensator podłączone szeregowo
	* w całym obwodzie (oczku) płynie maksymalny prąd
		* dla rezystancji $R$ tego obwodu
	* tj. reaktancje znoszą się w pewnym sensie i nie mają wpływu na resztę obwodu
	* w uproszczonej analizie [[10 Notatki/P TO\|P TO]] taki układ traktujemy, jakby był zwarciem
* ## Rezonans równoległy
{ #3bc521}

	* cewka i kondensator podłączone równolegle
	* prąd przepływa między jedną okładką kondensatora przez cewkę do drugiej i z powrotem
	* prąd ten zamyka się w tym oczku
	* w uproszczonej analizie [[10 Notatki/P TO\|P TO]] taki układ traktujemy jako przerwę (bo prąd krąży sobie po prostu między cewką i kondensatorem)
* ## Dobroć
	* Miara tego, jak długo układ RLC może przechowywać zgromadzoną energię w postaci energii pola leketrycznego (dl akondesnatora) i pola magnetycznego (dla cewki)
		* czyli ile drgań pola elektrycznego musi upłynąć, by układ RLC stracił przechowywaną energię
	* ### Dobroć w [[10 Notatki/EGZ INŻ 1.08 – Analiza obwodu szeregowego i równoległego RLC prądu przemiennego, zjawisko rezonansu, częstotliwość rezonansowa obwodu#^8def59\|układzie z rezonansem szeregowym]]
		* $Q=\frac{\\sqrt{ \frac{L}{C} }}{R}$
	* ### Dobroć w [[10 Notatki/EGZ INŻ 1.08 – Analiza obwodu szeregowego i równoległego RLC prądu przemiennego, zjawisko rezonansu, częstotliwość rezonansowa obwodu#^3bc521\|układzie z rezonansem równoległym]]
		* $Q=\frac{R}{\sqrt{ \frac{L}{C} }}$
		* 