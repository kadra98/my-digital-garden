---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 1.06 – Rozwiązywanie obwodów elektrycznych liniowych - twierdzenie Thevenina (Nortona) na przykładzie (obwód co najmniej z 3 oczkami i przynajmniej jedną gałęzią osobliwą)/","tags":["wiedza/zettel"]}
---

1. Rozwieramy impedancję, która chcemy policzyć $Z$ i obliczamy dla niej spadek napięcia $U_{Z}$
	* np. stosują [[10 Notatki/Metoda węzłowa\|Metoda węzłowa]]
2. Przekształcamy schemat do postaci:
	* źródła napięciowe zwieramy
	* źródła prądowe rozwieramy
3. Obliczamy impedancję zastępczą $Z_{Z}$ widzianą z punktu widzenia obliczanej rezystancji $Z$
4. Zgodnie z [[10 Notatki/Twierdzenie Thevenina i Nortona\|twierdzeniem Thevenina]], konstruujemy obwód z elementów połączonych szeregowo
	* źródła napięciowego o wartości $U_{Z}$
	* obliczonej impedancji zastępczej $Z_{Z}$
	* obliczanej impedancji $Z$
		* $Z$=$Z_{Z}$
	* alternatywnie zgodnie z [[10 Notatki/Twierdzenie Thevenina i Nortona\|twierdzeniem Nortona]] moglibyśmy obliczyć prąd, który płynie przez impedancję $Z$ i skonstruować obwód z równolegle połączonym źródłem prądowym i zastępczą impedancją
5. Obliczamy widzialną moc na impedancji $Z$
	* $P_{MAX}=\frac{|U_{0}|^2}{4*\text{Re} \{Z}$
		* moduł wartości zespolonej to
			* $U=a+jb$
			* $|U|=\sqrt{ a^2+b^2 }$