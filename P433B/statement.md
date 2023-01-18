## Description

<div><p>Kuriyama Mirai has killed many monsters and got many (namely <span class="tex-span"><i>n</i></span>) stones. She numbers the stones from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The cost of the <span class="tex-span"><i>i</i></span>-th stone is <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. Kuriyama Mirai wants to know something about these stones so she will ask you two kinds of questions:</p><ol> <li> She will tell you two numbers, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span>, and you should tell her <img align="middle" class="tex-formula" src="file://OOWLCNjf.png" style="max-width: 100.0%;max-height: 100.0%;">. </li><li> Let <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> be the cost of the <span class="tex-span"><i>i</i></span>-th cheapest stone (the cost that will be on the <span class="tex-span"><i>i</i></span>-th place if we arrange all the stone costs in non-decreasing order). This time she will tell you two numbers, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>)</span>, and you should tell her <img align="middle" class="tex-formula" src="file://iVxq5WmV.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ol><p>For every question you should give the correct answer, or Kuriyama Mirai will say "fuyukai desu" and then become unhappy.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — costs of the stones. </p><p>The third line contains an integer <span class="tex-span"><i>m</i>&nbsp;(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of Kuriyama Mirai's questions. Then follow <span class="tex-span"><i>m</i></span> lines, each line contains three integers <span class="tex-span"><i>type</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>type</i> ≤ 2)</span>, describing a question. If <span class="tex-span"><i>type</i></span> equal to <span class="tex-span">1</span>, then you should output the answer for the first question, else you should output the answer for the second one.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines. Each line must contain an integer — the answer to Kuriyama Mirai's question. Print the answers to the questions in the order of input.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i>&nbsp;(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers: <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub>&nbsp;(1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — costs of the stones. </p><p>The third line contains an integer <span class="tex-span"><i>m</i>&nbsp;(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of Kuriyama Mirai's questions. Then follow <span class="tex-span"><i>m</i></span> lines, each line contains three integers <span class="tex-span"><i>type</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i>&nbsp;(1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>type</i> ≤ 2)</span>, describing a question. If <span class="tex-span"><i>type</i></span> equal to <span class="tex-span">1</span>, then you should output the answer for the first question, else you should output the answer for the second one.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines. Each line must contain an integer — the answer to Kuriyama Mirai's question. Print the answers to the questions in the order of input.</p>





```input1
6
6 4 2 7 2 7
3
2 3 6
1 3 4
1 1 6

```




```input2
4
5 5 2 3
10
1 2 4
2 1 4
1 1 1
2 1 4
2 1 2
1 1 1
1 3 3
1 1 3
1 4 4
1 2 2

```




```output1
24
9
28

```




```output2
10
15
5
15
5
5
2
12
3
5

```



## Note

<p>Please note that the answers to the questions may overflow 32-bit integer type.</p>
