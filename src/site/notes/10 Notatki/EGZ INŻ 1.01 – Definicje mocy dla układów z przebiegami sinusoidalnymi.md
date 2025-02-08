---
{"dg-publish":true,"permalink":"/10 Notatki/EGZ INŻ 1.01 – Definicje mocy dla układów z przebiegami sinusoidalnymi/","tags":["wiedza/zettel"]}
---

* ## Moc chwilowa
	* $p=u*i$
	* moc jest dodatnia, gdy prąd i napięcie mają ten sam znak (są ze sobą w fazie)
	* ujemna moc możliwa jest wtedy, gdy układ jest odbiornikiem o charakterze reaktancyjnym
		* bo prąd jest wtedy przesunięty względem napięcia; istnieje więc taka chwila, gdy mają one przeciwne znaki
	* ![Pasted image 20250208211654.png](/img/user/80%20Zasoby/Pasted%20image%2020250208211654.png)
		* obwód o charakterze indukcyjnym
* ## Energia czynna $E_{P}$
	* to całka mocy chwilowej $p$ za okres $T_{0}$
		* $$E_{p}=\int p \space \text{d}t$$
* ## Moc czynna P
	* uzyskujemy dzieląc energię przez długość trwania okresu
	* $$P=\frac{1}{T}*\int p \space \text{d}t$$
	* dla przebiegu sinusoidalnego otrzymujemy równanie:
		* $$P=\frac{1}{T}* \int[UI\cos\varphi-UI\cos\varphi(2\omega t-\varphi))]\space \text{d}t$$
			* im przesunięcie fazowe między napięciem i prądem jest mniejsze, tym większą moc czynną uzyskujemy (przy zerowym przesunięciu $2\omega t-\varphi = 0$)
* ## Moc pozorna S
	* iloczyn **wartości skutecznych** prądu i napięcia
		* $S=U*I$
* ## [[10 Notatki/Moc bierna\|Moc bierna]] Q
	* $Q=UI\sin\varphi$
	* ponieważ kąt $\varphi$ jest dodatni w przypadku obwodów o charakterze indukcyjnym i ujemny w obwodach o charakterze pojemnościowym, to
		* moc bierna indukcyjna ozaczana jest jako dodatnia
			* (co oznacza, że w danym obwodzie występuje jej pobór)
		* moc bierna pojemnościowa jest oznaczana jako dodatnia
			* co oznacza, że występuje jakby jej produkcja
	* [[10 Notatki/Moc bierna – co ją pobiera, a co ją oddaje\|Moc bierna – co ją pobiera, a co ją oddaje]]