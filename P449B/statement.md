## Description

<div><p>Jzzhu is the president of country A. There are <span class="tex-span"><i>n</i></span> cities numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in his country. City <span class="tex-span">1</span> is the capital of A. Also there are <span class="tex-span"><i>m</i></span> roads connecting the cities. One can go from city <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (and vise versa) using the <span class="tex-span"><i>i</i></span>-th road, the length of this road is <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. Finally, there are <span class="tex-span"><i>k</i></span> train routes in the country. One can use the <span class="tex-span"><i>i</i></span>-th train route to go from capital of the country to city <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (and vise versa), the length of this route is <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Jzzhu doesn't want to waste the money of the country, so he is going to close some of the train routes. Please tell Jzzhu the maximum number of the train routes which can be closed under the following condition: the length of the shortest path from every city to the capital mustn't change.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>;&nbsp;1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(2 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>It is guaranteed that there is at least one way from every city to the capital. Note, that there can be multiple roads between two cities. Also, there can be multiple routes going to the same city from the capital.</p></div><div class="output-specification"><p>Output a single integer representing the maximum number of the train routes which can be closed.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>m</i> ≤ 3·10<sup class="upper-index">5</sup>;&nbsp;1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;<i>u</i><sub class="lower-index"><i>i</i></sub> ≠ <i>v</i><sub class="lower-index"><i>i</i></sub>;&nbsp;1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines contains two integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(2 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p><p>It is guaranteed that there is at least one way from every city to the capital. Note, that there can be multiple roads between two cities. Also, there can be multiple routes going to the same city from the capital.</p>

## Output

<p>Output a single integer representing the maximum number of the train routes which can be closed.</p>





```input1
5 5 3
1 2 1
2 3 2
1 3 3
3 4 4
1 5 5
3 5
4 5
5 5

```




```input2
2 2 3
1 2 2
2 1 3
2 1
2 2
2 3

```




```output1
2

```




```output2
2

```


