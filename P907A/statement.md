## Description

<div><p>A family consisting of father bear, mother bear and son bear owns three cars. Father bear can climb into the largest car and he likes it. Also, mother bear can climb into the middle car and she likes it. Moreover, son bear can climb into the smallest car and he likes it. It's known that the largest car is strictly larger than the middle car, and the middle car is strictly larger than the smallest car. </p><p>Masha came to test these cars. She could climb into all cars, but she liked only the smallest car. </p><p>It's known that a character with size <span class="tex-span"><i>a</i></span> can climb into some car with size <span class="tex-span"><i>b</i></span> if and only if <span class="tex-span"><i>a</i> ≤ <i>b</i></span>, he or she likes it if and only if he can climb into this car and <span class="tex-span">2<i>a</i> ≥ <i>b</i></span>.</p><p>You are given sizes of bears and Masha. Find out some possible integer non-negative sizes of cars.</p></div><div class="input-specification"><p>You are given four integers <span class="tex-span"><i>V</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>V</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>V</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>V</i><sub class="lower-index"><i>m</i></sub></span>(<span class="tex-span">1 ≤ <i>V</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— sizes of father bear, mother bear, son bear and Masha, respectively. It's guaranteed that <span class="tex-span"><i>V</i><sub class="lower-index">1</sub> &gt; <i>V</i><sub class="lower-index">2</sub> &gt; <i>V</i><sub class="lower-index">3</sub></span>.</p></div><div class="output-specification"><p>Output three integers&nbsp;— sizes of father bear's car, mother bear's car and son bear's car, respectively.</p><p>If there are multiple possible solutions, print any.</p><p>If there is no solution, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p></div>

## Input

<p>You are given four integers <span class="tex-span"><i>V</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>V</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>V</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>V</i><sub class="lower-index"><i>m</i></sub></span>(<span class="tex-span">1 ≤ <i>V</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— sizes of father bear, mother bear, son bear and Masha, respectively. It's guaranteed that <span class="tex-span"><i>V</i><sub class="lower-index">1</sub> &gt; <i>V</i><sub class="lower-index">2</sub> &gt; <i>V</i><sub class="lower-index">3</sub></span>.</p>

## Output

<p>Output three integers&nbsp;— sizes of father bear's car, mother bear's car and son bear's car, respectively.</p><p>If there are multiple possible solutions, print any.</p><p>If there is no solution, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p>





```input1
50 30 10 10

```




```input2
100 50 10 21

```




```output1
50
30
10

```




```output2
-1

```



## Note

<p>In first test case all conditions for cars' sizes are satisfied.</p><p>In second test case there is no answer, because Masha should be able to climb into smallest car (so size of smallest car in not less than 21), but son bear should like it, so maximum possible size of it is 20.</p>
