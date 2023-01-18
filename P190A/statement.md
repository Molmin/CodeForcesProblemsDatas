## Description

<div><p>One day Vasya heard a story: "In the city of High Bertown a bus number 62 left from the bus station. It had <span class="tex-span"><i>n</i></span> grown-ups and <span class="tex-span"><i>m</i></span> kids..."</p><p>The latter events happen to be of no importance to us. Vasya is an accountant and he loves counting money. So he wondered what maximum and minimum sum of money these passengers could have paid for the ride.</p><p>The bus fare equals one berland ruble in High Bertown. However, not everything is that easy — <span class="tex-font-style-bf">no more than one</span> child can ride for free with each grown-up passenger. That means that a grown-up passenger who rides with his <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> &gt; 0)</span> children, pays overall <span class="tex-span"><i>k</i></span> rubles: a ticket for himself and <span class="tex-span">(<i>k</i> - 1)</span> tickets for his children. Also, a grown-up can ride without children, in this case he only pays one ruble.</p><p>We know that in High Bertown children can't ride in a bus unaccompanied by grown-ups.</p><p>Help Vasya count the minimum and the maximum sum in Berland rubles, that all passengers of this bus could have paid in total.</p></div><div class="input-specification"><p>The input file consists of a single line containing two space-separated numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of the grown-ups and the number of the children in the bus, correspondingly.</p></div><div class="output-specification"><p>If <span class="tex-span"><i>n</i></span> grown-ups and <span class="tex-span"><i>m</i></span> children could have ridden in the bus, then print on a single line two space-separated integers — the minimum and the maximum possible total bus fare, correspondingly. </p><p>Otherwise, print "<span class="tex-font-style-tt">Impossible</span>" (without the quotes).</p></div>

## Input

<p>The input file consists of a single line containing two space-separated numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(0 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of the grown-ups and the number of the children in the bus, correspondingly.</p>

## Output

<p>If <span class="tex-span"><i>n</i></span> grown-ups and <span class="tex-span"><i>m</i></span> children could have ridden in the bus, then print on a single line two space-separated integers — the minimum and the maximum possible total bus fare, correspondingly. </p><p>Otherwise, print "<span class="tex-font-style-tt">Impossible</span>" (without the quotes).</p>





```input1
1 2

```




```input2
0 5

```




```input3
2 2

```




```output1
2 2
```




```output2
Impossible
```




```output3
2 3
```



## Note

<p>In the first sample a grown-up rides with two children and pays two rubles.</p><p>In the second sample there are only children in the bus, so the situation is impossible.</p><ul> In the third sample there are two cases: <li> Each of the two grown-ups rides with one children and pays one ruble for the tickets. In this case the passengers pay two rubles in total. </li><li> One of the grown-ups ride with two children's and pays two rubles, the another one rides alone and pays one ruble for himself. So, they pay three rubles in total. </li></ul>
