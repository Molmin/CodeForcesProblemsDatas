## Description

<div><p>Iahub is a big fan of tourists. He wants to become a tourist himself, so he planned a trip. There are <span class="tex-span"><i>n</i></span> destinations on a straight road that Iahub wants to visit. Iahub starts the excursion from kilometer 0. The <span class="tex-span"><i>n</i></span> destinations are described by a non-negative integers sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. The number <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> represents that the <span class="tex-span"><i>k</i></span>th destination is at distance <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> kilometers from the starting point. No two destinations are located in the same place. </p><p>Iahub wants to visit each destination only once. Note that, crossing through a destination is not considered visiting, unless Iahub explicitly wants to visit it at that point. Also, after Iahub visits his last destination, he doesn't come back to kilometer 0, as he stops his trip at the last destination. </p><p>The distance between destination located at kilometer <span class="tex-span"><i>x</i></span> and next destination, located at kilometer <span class="tex-span"><i>y</i></span>, is <span class="tex-span">|<i>x</i> - <i>y</i>|</span> kilometers. We call a "route" an order of visiting the destinations. Iahub can visit destinations in any order he wants, as long as he visits all <span class="tex-span"><i>n</i></span> destinations and he doesn't visit a destination more than once. </p><p>Iahub starts writing out on a paper all possible routes and for each of them, he notes the total distance he would walk. He's interested in the average number of kilometers he would walk by choosing a route. As he got bored of writing out all the routes, he asks you to help him.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>).</p></div><div class="output-specification"><p>Output two integers — the numerator and denominator of a fraction which is equal to the wanted average number. The fraction must be irreducible.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). Next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>).</p>

## Output

<p>Output two integers — the numerator and denominator of a fraction which is equal to the wanted average number. The fraction must be irreducible.</p>





```input1
3
2 3 5

```




```output1
22 3
```



## Note

<p>Consider 6 possible routes:</p><ul> <li> [2, 3, 5]: total distance traveled: |2 – 0| + |3 – 2| + |5 – 3| = 5; </li><li> [2, 5, 3]: |2 – 0| + |5 – 2| + |3 – 5| = 7; </li><li> [3, 2, 5]: |3 – 0| + |2 – 3| + |5 – 2| = 7; </li><li> [3, 5, 2]: |3 – 0| + |5 – 3| + |2 – 5| = 8; </li><li> [5, 2, 3]: |5 – 0| + |2 – 5| + |3 – 2| = 9; </li><li> [5, 3, 2]: |5 – 0| + |3 – 5| + |2 – 3| = 8. </li></ul><p>The average travel distance is <img align="middle" class="tex-formula" src="file://uhMAG0gF.png" style="max-width: 100.0%;max-height: 100.0%;"> = <img align="middle" class="tex-formula" src="file://oZxWbCNC.png" style="max-width: 100.0%;max-height: 100.0%;"> = <img align="middle" class="tex-formula" src="file://rEkmiYdg.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
