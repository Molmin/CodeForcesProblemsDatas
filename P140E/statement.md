## Description

<div><p>As Gerald, Alexander, Sergey and Gennady are already busy with the usual New Year chores, Edward hastily decorates the New Year Tree. And any decent New Year Tree must be decorated with a good garland. Edward has lamps of <span class="tex-span"><i>m</i></span> colors and he wants to make a garland from them. That garland should represent a sequence whose length equals <span class="tex-span"><i>L</i></span>. Edward's tree is <span class="tex-span"><i>n</i></span> layers high and Edward plans to hang the garland so as to decorate the first layer with the first <span class="tex-span"><i>l</i><sub class="lower-index">1</sub></span> lamps, the second layer — with the next <span class="tex-span"><i>l</i><sub class="lower-index">2</sub></span> lamps and so on. The last <span class="tex-span"><i>n</i></span>-th layer should be decorated with the last <span class="tex-span"><i>l</i><sub class="lower-index"><i>n</i></sub></span> lamps, <img align="middle" class="tex-formula" src="file://WJJempjL.png" style="max-width: 100.0%;max-height: 100.0%;"> </p><p>Edward adores all sorts of math puzzles, so he suddenly wondered: how many different ways to assemble the garland are there given that the both following two conditions are met: </p><ol> <li> Any two lamps that follow consecutively in the same layer should have different colors. </li><li> The sets of used colors in every two <span class="tex-font-style-bf">neighbouring</span> layers must be different. We consider unordered sets (not multisets), where every color occurs no more than once. So the number of lamps of particular color does not matter. </li></ol><p>Help Edward find the answer to this nagging problem or else he won't manage to decorate the Tree by New Year. You may consider that Edward has an unlimited number of lamps of each of <span class="tex-span"><i>m</i></span> colors and it is not obligatory to use all <span class="tex-span"><i>m</i></span> colors. The garlands are considered different if they differ in at least one position when represented as sequences. Calculate the answer modulo <span class="tex-span"><i>p</i></span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>) which are the number of the tree's layers, the number of the lamps' colors and module correspondingly. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>, <img align="middle" class="tex-formula" src="file://EiVZg2el.png" style="max-width: 100.0%;max-height: 100.0%;">).</p></div><div class="output-specification"><p>Print the only integer — the number of garlands modulo <span class="tex-span"><i>p</i></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>) which are the number of the tree's layers, the number of the lamps' colors and module correspondingly. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>, <img align="middle" class="tex-formula" src="file://EiVZg2el.png" style="max-width: 100.0%;max-height: 100.0%;">).</p>

## Output

<p>Print the only integer — the number of garlands modulo <span class="tex-span"><i>p</i></span>.</p>





```input1
3 2 1000
3 1 2

```




```input2
2 3 1000
2 2

```




```input3
1 1 1000
5

```




```output1
8

```




```output2
24

```




```output3
0

```



## Note

<p>In the first sample the following variants are possible: 121|1|12, 121|1|21, 121|2|12, 121|2|21, 212|1|12, 212|1|21, 212|2|12, 212|2|21. In the second sample the following variants are possible: 12|13, 12|23, 12|31, 12|32 and so on. </p><center> Figure for the first sample: <img class="tex-graphics" src="file://mJI2xBn1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
