## Description

<div><p>After a team finished their training session on Euro football championship, Valeric was commissioned to gather the balls and sort them into baskets. Overall the stadium has <span class="tex-span"><i>n</i></span> balls and <span class="tex-span"><i>m</i></span> baskets. The baskets are positioned in a row from left to right and they are numbered with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>, correspondingly. The balls are numbered with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>Valeric decided to sort the balls in the order of increasing of their numbers by the following scheme. He will put each new ball in the basket with the least number of balls. And if he's got several variants, he chooses the basket which stands closer to the middle. That means that he chooses the basket for which <img align="middle" class="tex-formula" src="file://KKKcjuFx.png" style="max-width: 100.0%;max-height: 100.0%;"> is minimum, where <span class="tex-span"><i>i</i></span> is the number of the basket. If in this case Valeric still has multiple variants, he chooses the basket with the minimum number.</p><p>For every ball print the number of the basket where it will go according to Valeric's scheme.</p><p>Note that the balls are sorted into baskets in the order of increasing numbers, that is, the first ball goes first, then goes the second ball and so on.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of balls and baskets, correspondingly.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> numbers, one per line. The <span class="tex-span"><i>i</i></span>-th line must contain the number of the basket for the <span class="tex-span"><i>i</i></span>-th ball.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of balls and baskets, correspondingly.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> numbers, one per line. The <span class="tex-span"><i>i</i></span>-th line must contain the number of the basket for the <span class="tex-span"><i>i</i></span>-th ball.</p>





```input1
4 3

```




```input2
3 1

```




```output1
2
1
3
2

```




```output2
1
1
1

```


