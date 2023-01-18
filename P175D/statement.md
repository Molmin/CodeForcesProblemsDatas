## Description

<div><p>Vasya plays the Plane of Tanks.</p><p>Tanks are described with the following attributes: </p><ul> <li> the number of hit points; </li><li> the interval between two gun shots (the time required to recharge the gun); </li><li> the probability that the gun shot will not pierce armor of the enemy tank; </li><li> the damage to the enemy's tank. </li></ul><p>The gun damage is described with a segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>, where <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> are integer numbers. The potential gun damage <span class="tex-span"><i>x</i></span> is chosen with equal probability among all integer numbers of the segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span>. If the shot pierces the armor of an enemy's tank then the enemy loses <span class="tex-span"><i>x</i></span> hit points. If the number of hit points becomes non-positive then the enemy tank is considered destroyed. </p><p>It is possible that the shot does not pierce the armor of a tank. In this case the number of hit points doesn't change. The probability that the armor will not be pierced is considered as the shooting tank attribute and does not depend on players' behavior.</p><p>The victory is near and there is only one enemy tank left. Vasya is ready for the battle — one more battle between the Good and the Evil is inevitable! Two enemies saw each other and each of them fired a shot at the same moment... The last battle has begun! Help Vasya to determine what is the probability that he will win the battle by destroying the enemy tank? </p><p>If both tanks are destroyed (after simultaneous shots), then Vasya is considered a winner. You can assume that each player fires a shot just after the gun recharge and each tank has infinite number of ammo.</p></div><div class="input-specification"><p>The first line contains five integer numbers separated with spaces describing Vasya's tank: the number of hit points <span class="tex-span"><i>hp</i></span> <span class="tex-span">(10 ≤ <i>hp</i> ≤ 200)</span>, the interval between two shots <span class="tex-span"><i>dt</i></span> <span class="tex-span">(1 ≤ <i>dt</i> ≤ 30)</span>, gun damage segment <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(10 ≤ <i>l</i> ≤ <i>r</i> ≤ 100)</span>, the probability that the enemy's tank armor will not be pierced <span class="tex-span"><i>p</i></span> <span class="tex-span">(0 ≤ <i>p</i> ≤ 100)</span> (percents).</p><p>The second line describes the tank of Vasya's enemy in the same format.</p></div><div class="output-specification"><p>Print the only number with absolute or relative error no more than <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> — probability of Vasya's victory.</p></div>

## Input

<p>The first line contains five integer numbers separated with spaces describing Vasya's tank: the number of hit points <span class="tex-span"><i>hp</i></span> <span class="tex-span">(10 ≤ <i>hp</i> ≤ 200)</span>, the interval between two shots <span class="tex-span"><i>dt</i></span> <span class="tex-span">(1 ≤ <i>dt</i> ≤ 30)</span>, gun damage segment <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(10 ≤ <i>l</i> ≤ <i>r</i> ≤ 100)</span>, the probability that the enemy's tank armor will not be pierced <span class="tex-span"><i>p</i></span> <span class="tex-span">(0 ≤ <i>p</i> ≤ 100)</span> (percents).</p><p>The second line describes the tank of Vasya's enemy in the same format.</p>

## Output

<p>Print the only number with absolute or relative error no more than <span class="tex-span">10<sup class="upper-index"> - 4</sup></span> — probability of Vasya's victory.</p>





```input1
100 3 50 50 0
100 3 50 50 0

```




```input2
100 3 50 50 0
100 2 48 50 0

```




```input3
100 3 50 50 0
100 1 50 50 50

```




```output1
1.000000

```




```output2
0.888889

```




```output3
0.500000

```



## Note

<p>In the first example both tanks are destroyed at once after the second shot. The probability of destroying the enemy tank is <span class="tex-span">1</span>.</p><p>In the second example Vasya's enemy tank fires the second shot before Vasya's tank, but has no time for the third shot. In order to destroy Vasya's tank it is necessary to fire two shots with damage 50. The probability of that event is <img align="middle" class="tex-formula" src="file://Otlocm11.png" style="max-width: 100.0%;max-height: 100.0%;"> = <img align="middle" class="tex-formula" src="file://zrOUi8Af.png" style="max-width: 100.0%;max-height: 100.0%;">. Otherwise, Vasya wins.</p><p>In the third example Vasya's enemy tank fires three shots with probability of armor piercing <span class="tex-span">0.5</span>. In order to destroy Vasya's tank it is necessary that at least 2 of 3 shots pierce the armor of Vasya's tank. The probability of this event is <span class="tex-span">0.5</span>.</p>
