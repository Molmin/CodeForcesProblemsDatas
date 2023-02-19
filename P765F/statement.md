## Description

<div><p>Artsem is on vacation and wants to buy souvenirs for his two teammates. There are <span class="tex-span"><i>n</i></span> souvenir shops along the street. In <span class="tex-span"><i>i</i></span>-th shop Artsem can buy one souvenir for <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> dollars, and he cannot buy more than one souvenir in one shop. He doesn't want to introduce envy in his team, so he wants to buy two souvenirs with least possible difference in price.</p><p>Artsem has visited the shopping street <span class="tex-span"><i>m</i></span> times. For some strange reason on the <span class="tex-span"><i>i</i></span>-th day only shops with numbers from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> were operating (weird? yes it is, but have you ever tried to come up with a reasonable legend for a range query problem?). For each visit, Artsem wants to know the minimum possible difference in prices of two different souvenirs he can buy in the opened shops.</p><p>In other words, for each Artsem's visit you should find the minimum possible value of <span class="tex-span">|<i>a</i><sub class="lower-index"><i>s</i></sub> - <i>a</i><sub class="lower-index"><i>t</i></sub>|</span> where <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>s</i>, <i>t</i> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>s</i> ≠ <i>t</i></span>.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains the number of queries <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the queries. <span class="tex-span"><i>i</i></span>-th of these lines contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> denoting the range of shops working on <span class="tex-span"><i>i</i></span>-th day (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print the answer to each query in a separate line.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The third line contains the number of queries <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>m</i></span> lines describe the queries. <span class="tex-span"><i>i</i></span>-th of these lines contains two space-separated integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> denoting the range of shops working on <span class="tex-span"><i>i</i></span>-th day (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>Print the answer to each query in a separate line.</p>





```input1
8
3 1 4 1 5 9 2 6
4
1 8
1 3
4 8
5 7

```




```output1
0
1
1
3

```


