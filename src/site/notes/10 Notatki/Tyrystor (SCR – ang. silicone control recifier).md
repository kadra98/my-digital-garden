---
{"dg-publish":true,"permalink":"/10 Notatki/Tyrystor (SCR – ang. silicone control recifier)/","tags":["wiedza/zettel"]}
---

* składa się z czterech złączy (N-P-N-P)
* Ciągła konieczność przepływania prądu bazy w [[10 Notatki/Tranzystor bipolarny (BJT– ang. Bipolar junction transistor)\|Tranzystor bipolarny (BJT– ang. Bipolar junction transistor)]] tworzy dosyć duże straty energii
* zależnie od polaryzacji przyłożonego źródła napięcia, istnieje albo jedna, albo dwie bariery
	* ![Pasted image 20250206183320.png](/img/user/80%20Zasoby/Pasted%20image%2020250206183320.png)
	* ![Pasted image 20250206183327.png](/img/user/80%20Zasoby/Pasted%20image%2020250206183327.png)
* By umożliwić przepływ prądu, stosujemy tzw. metodę *gate triggering*
	* Polega to na wyzwoleniu przepływu prądu między dwoma skrajnymi warstwami P i N
	* Niewielkie ilości wolnych elektronów w warstwie P *są zaciągane* przez źródło i wpychane do warstwy N, w której już znajdują się wolne elektrony
	* Podłączone źródło wymusza przepływ elektronów z warstwy N do warstwy P, gdzie część elektronów wypełnia wolne dziury, a pozostała pozostaje wolna.
	* Ta część P staje się więc *de facto* warstwą typu N (z dodatkowymi elektronami)
	* Elektrony te przepływają do kolejnej warsstwy N, a z niej do ostatniej warstwy P i dalej do owbodu
	* ![Pasted image 20250206183921.png](/img/user/80%20Zasoby/Pasted%20image%2020250206183921.png)
	* Całość staje się więc diodą o jedynie dwóch złączach: P i N
		* ![Pasted image 20250206184034.png](/img/user/80%20Zasoby/Pasted%20image%2020250206184034.png)
	* **Co istotne:** nawet po usunięciu źródła zasilania wywołującego *gate triggering*, tyrystor będzie nadal przewodził prąd
		* o ile nie zmienia się polaryzacja źródła napięcia – więc problem nie dotyczy układów AC
		* Natomiast w układach DC stosuje się wpięty szeregowo do tyrystora układ LC, który wywołuje przepływ prądu w drugim kierunku
			* (W idealnym układzie LC, prąd przepływa między jedną okładką, przez cewkę do drugiej okładki, a następnie z powrotem)