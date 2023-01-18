## Description

<div><p>Oleg the bank client lives in Bankopolia. There are <span class="tex-span"><i>n</i></span> cities in Bankopolia and some pair of cities are connected directly by bi-directional roads. The cities are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. There are a total of <span class="tex-span"><i>m</i></span> roads in Bankopolia, the <span class="tex-span"><i>i</i></span>-th road connects cities <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. It is guaranteed that from each city it is possible to travel to any other city using some of the roads.</p><p>Oleg wants to give a label to each city. Suppose the label of city <span class="tex-span"><i>i</i></span> is equal to <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Then, it must hold that for all pairs of cities <span class="tex-span">(<i>u</i>, <i>v</i>)</span> the condition <span class="tex-span">|<i>x</i><sub class="lower-index"><i>u</i></sub> - <i>x</i><sub class="lower-index"><i>v</i></sub>| ≤ 1</span> holds if and only if there is a road connecting <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p><p>Oleg wonders if such a labeling is possible. Find an example of such labeling if the task is possible and state that it is impossible otherwise.</p></div><div class="input-specification"><p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cities and the number of roads.</p><p>Next, <span class="tex-span"><i>m</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the cities connected by the <span class="tex-span"><i>i</i></span>-th road. It is guaranteed that there is at most one road between each pair of cities and it is possible to travel from any city to any other city using some roads.</p></div><div class="output-specification"><p>If the required labeling is not possible, output a single line containing the string "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, output the string "<span class="tex-font-style-tt">YES</span>" (without quotes) on the first line. On the next line, output <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. The condition <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> must hold for all <span class="tex-span"><i>i</i></span>, and for all pairs of cities <span class="tex-span">(<i>u</i>, <i>v</i>)</span> the condition <span class="tex-span">|<i>x</i><sub class="lower-index"><i>u</i></sub> - <i>x</i><sub class="lower-index"><i>v</i></sub>| ≤ 1</span> must hold if and only if there is a road connecting <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p></div>

## Input

<p>The first line of input contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of cities and the number of roads.</p><p>Next, <span class="tex-span"><i>m</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— the cities connected by the <span class="tex-span"><i>i</i></span>-th road. It is guaranteed that there is at most one road between each pair of cities and it is possible to travel from any city to any other city using some roads.</p>

## Output

<p>If the required labeling is not possible, output a single line containing the string "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>Otherwise, output the string "<span class="tex-font-style-tt">YES</span>" (without quotes) on the first line. On the next line, output <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>n</i></sub></span>. The condition <span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span> must hold for all <span class="tex-span"><i>i</i></span>, and for all pairs of cities <span class="tex-span">(<i>u</i>, <i>v</i>)</span> the condition <span class="tex-span">|<i>x</i><sub class="lower-index"><i>u</i></sub> - <i>x</i><sub class="lower-index"><i>v</i></sub>| ≤ 1</span> must hold if and only if there is a road connecting <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span>.</p>





```input1
4 4
1 2
1 3
1 4
3 4

```




```input2
5 10
1 2
1 3
1 4
1 5
2 3
2 4
2 5
3 4
3 5
5 4

```




```input3
4 3
1 2
1 3
1 4

```




```output1
YES
2 3 1 1 

```




```output2
YES
1 1 1 1 1 

```




```output3
NO

```



## Note

<p>For the first sample, <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = 2</span>, <span class="tex-span"><i>x</i><sub class="lower-index">2</sub> = 3</span>, <span class="tex-span"><i>x</i><sub class="lower-index">3</sub> = <i>x</i><sub class="lower-index">4</sub> = 1</span> is a valid labeling. Indeed, <span class="tex-span">(3, 4)</span>, <span class="tex-span">(1, 2)</span>, <span class="tex-span">(1, 3)</span>, <span class="tex-span">(1, 4)</span> are the only pairs of cities with difference of labels not greater than <span class="tex-span">1</span>, and these are precisely the roads of Bankopolia.</p><p>For the second sample, all pairs of cities have difference of labels not greater than <span class="tex-span">1</span> and all pairs of cities have a road connecting them.</p><p>For the last sample, it is impossible to construct a labeling satisfying the given constraints.</p>
