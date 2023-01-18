## Description

<div><p>The Trinitarian kingdom has exactly <span class="tex-span"><i>n</i> = 3<i>k</i></span> cities. All of them are located on the shores of river Trissisipi, which flows through the whole kingdom. Some of the cities are located on one side of the river, and all the rest are on the other side.</p><p>Some cities are connected by bridges built between them. Each bridge connects two cities that are located on the opposite sides of the river. Between any two cities exists no more than one bridge.</p><p>The recently inaugurated King Tristan the Third is busy distributing his deputies among cities. In total there are <span class="tex-span"><i>k</i></span> deputies and the king wants to commission each of them to control exactly three cities. However, no deputy can be entrusted to manage the cities, which are connected by a bridge — the deputy can set a too high fee for travelling over the bridge to benefit his pocket, which is bad for the reputation of the king.</p><p>Help King Tristan the Third distribute the deputies between the cities, if it is possible.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the number of cities and bridges (<span class="tex-span">3 ≤ <i>n</i> &lt; 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> = 3<i>k</i></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). Next <span class="tex-span"><i>m</i></span> lines describe the bridges. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — the numbers of cities that are connected by the <span class="tex-span"><i>i</i></span>-th bridge (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>).</p><p>It is guaranteed that no bridge connects a city with itself and that any two cities are connected with no more than one bridge.</p></div><div class="output-specification"><p>If distributing the deputies in the required manner is impossible, print in a single line "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), and in the second line print which deputy should be put in charge of each city. The <span class="tex-span"><i>i</i></span>-th number should represent the number of the deputy (from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>), who should be in charge of city numbered <span class="tex-span"><i>i</i></span>-th in the input — overall there should be <span class="tex-span"><i>n</i></span> numbers.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> — the number of cities and bridges (<span class="tex-span">3 ≤ <i>n</i> &lt; 10<sup class="upper-index">5</sup></span>, <span class="tex-span"><i>n</i> = 3<i>k</i></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>). Next <span class="tex-span"><i>m</i></span> lines describe the bridges. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> — the numbers of cities that are connected by the <span class="tex-span"><i>i</i></span>-th bridge (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>i</i> ≤ <i>m</i></span>).</p><p>It is guaranteed that no bridge connects a city with itself and that any two cities are connected with no more than one bridge.</p>

## Output

<p>If distributing the deputies in the required manner is impossible, print in a single line "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p><p>Otherwise, in the first line print "<span class="tex-font-style-tt">YES</span>" (without the quotes), and in the second line print which deputy should be put in charge of each city. The <span class="tex-span"><i>i</i></span>-th number should represent the number of the deputy (from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>), who should be in charge of city numbered <span class="tex-span"><i>i</i></span>-th in the input — overall there should be <span class="tex-span"><i>n</i></span> numbers.</p><p>If there are multiple solutions, print any of them.</p>





```input1
6 6
1 2
4 1
3 5
6 5
2 6
4 6

```




```input2
3 1
1 2

```




```output1
YES
1 2 1 2 2 1
```




```output2
NO
```


