## Description

<div><p>Polycarp invited all his friends to the tea party to celebrate the holiday. He has <span class="tex-span"><i>n</i></span> cups, one for each of his <span class="tex-span"><i>n</i></span> friends, with volumes <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. His teapot stores <span class="tex-span"><i>w</i></span> milliliters of tea (<span class="tex-span"><i>w</i> ≤ <i>a</i><sub class="lower-index">1</sub> + <i>a</i><sub class="lower-index">2</sub> + ... + <i>a</i><sub class="lower-index"><i>n</i></sub></span>). Polycarp wants to pour tea in cups in such a way that:</p><ul> <li> Every cup will contain tea for at least half of its volume </li><li> Every cup will contain integer number of milliliters of tea </li><li> All the tea from the teapot will be poured into cups </li><li> All friends will be <span class="tex-font-style-it">satisfied</span>. </li></ul><p>Friend with cup <span class="tex-span"><i>i</i></span> won't be <span class="tex-font-style-it">satisfied</span>, if there exists such cup <span class="tex-span"><i>j</i></span> that cup <span class="tex-span"><i>i</i></span> contains less tea than cup <span class="tex-span"><i>j</i></span> but <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; <i>a</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>For each cup output how many milliliters of tea should be poured in it. If it's impossible to pour all the tea and satisfy all conditions then output <span class="tex-font-style-tt">-1</span>.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <img align="middle" class="tex-formula" src="file://vI75RysO.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p></div><div class="output-specification"><p>Output how many milliliters of tea every cup should contain. If there are multiple answers, print any of them.</p><p>If it's impossible to pour all the tea and satisfy all conditions then output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>, <img align="middle" class="tex-formula" src="file://vI75RysO.png" style="max-width: 100.0%;max-height: 100.0%;">).</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>).</p>

## Output

<p>Output how many milliliters of tea every cup should contain. If there are multiple answers, print any of them.</p><p>If it's impossible to pour all the tea and satisfy all conditions then output <span class="tex-font-style-tt">-1</span>.</p>





```input1
2 10
8 7

```




```input2
4 4
1 1 1 1

```




```input3
3 10
9 8 10

```




```output1
6 4 

```




```output2
1 1 1 1 

```




```output3
-1

```



## Note

<p>In the third example you should pour to the first cup at least 5 milliliters, to the second one at least 4, to the third one at least 5. It sums up to 14, which is greater than 10 milliliters available.</p>
