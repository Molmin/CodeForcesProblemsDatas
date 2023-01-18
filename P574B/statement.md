## Description

<div><p>Do you know a story about the three musketeers? Anyway, you will learn about its origins now.</p><p>Richelimakieu is a cardinal in the city of Bearis. He is tired of dealing with crime by himself. He needs three brave warriors to help him to fight against bad guys.</p><p>There are <span class="tex-span"><i>n</i></span> warriors. Richelimakieu wants to choose three of them to become musketeers but it's not that easy. The most important condition is that musketeers must know each other to cooperate efficiently. And they shouldn't be too well known because they could be betrayed by old friends. For each musketeer his <span class="tex-font-style-it">recognition</span> is the number of warriors he knows, excluding other two musketeers.</p><p>Help Richelimakieu! Find if it is possible to choose three musketeers knowing each other, and what is minimum possible sum of their recognitions.</p></div><div class="input-specification"><p>The first line contains two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 4000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 4000</span>) — respectively number of warriors and number of pairs of warriors knowing each other.</p><p><span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). Warriors <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> know each other. Each pair of warriors will be listed at most once.</p></div><div class="output-specification"><p>If Richelimakieu can choose three musketeers, print the minimum possible sum of their recognitions. Otherwise, print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p></div>

## Input

<p>The first line contains two space-separated integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 4000</span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 4000</span>) — respectively number of warriors and number of pairs of warriors knowing each other.</p><p><span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>m</i></span> lines contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). Warriors <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> know each other. Each pair of warriors will be listed at most once.</p>

## Output

<p>If Richelimakieu can choose three musketeers, print the minimum possible sum of their recognitions. Otherwise, print "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p>





```input1
5 6
1 2
1 3
2 3
2 4
3 4
4 5

```




```input2
7 4
2 1
3 6
5 1
1 7

```




```output1
2

```




```output2
-1

```



## Note

<p>In the first sample Richelimakieu should choose a triple <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>. The first musketeer doesn't know anyone except other two musketeers so his recognition is <span class="tex-span">0</span>. The second musketeer has recognition <span class="tex-span">1</span> because he knows warrior number <span class="tex-span">4</span>. The third musketeer also has recognition <span class="tex-span">1</span> because he knows warrior <span class="tex-span">4</span>. Sum of recognitions is <span class="tex-span">0 + 1 + 1 = 2</span>.</p><p>The other possible triple is <span class="tex-span">2, 3, 4</span> but it has greater sum of recognitions, equal to <span class="tex-span">1 + 1 + 1 = 3</span>.</p><p>In the second sample there is no triple of warriors knowing each other.</p>
