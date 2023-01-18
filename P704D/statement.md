## Description

<div><p>Steve Rogers is fascinated with new vibranium shields S.H.I.E.L.D gave him. They're all uncolored. There are <span class="tex-span"><i>n</i></span> shields in total, the <span class="tex-span"><i>i</i></span>-th shield is located at point <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> of the coordinate plane. It's possible that two or more shields share the same location.</p><p>Steve wants to paint all these shields. He paints each shield in either red or blue. Painting a shield in red costs <span class="tex-span"><i>r</i></span> dollars while painting it in blue costs <span class="tex-span"><i>b</i></span> dollars.</p><p>Additionally, there are <span class="tex-span"><i>m</i></span> constraints Steve wants to be satisfied. The <span class="tex-span"><i>i</i></span>-th constraint is provided by three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>:</p><ul> <li> If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then the absolute difference between the number of red and blue shields on line <span class="tex-span"><i>x</i> = <i>l</i><sub class="lower-index"><i>i</i></sub></span> should not exceed <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>, then the absolute difference between the number of red and blue shields on line <span class="tex-span"><i>y</i> = <i>l</i><sub class="lower-index"><i>i</i></sub></span> should not exceed <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>. </li></ul><p>Steve gave you the task of finding the painting that satisfies all the condition and the total cost is minimum.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the number of shields and the number of constraints respectively.</p><p>The second line contains two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>r</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the shields coordinates. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the constrains. The <span class="tex-span"><i>j</i></span>-th of these lines contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ 2, 1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>d</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>If satisfying all the constraints is impossible print <span class="tex-font-style-tt">-1</span> in first and only line of the output.</p><p>Otherwise, print the minimum total cost in the first line of output. In the second line print a string of length <span class="tex-span"><i>n</i></span> consisting of letters '<span class="tex-font-style-tt">r</span>' and '<span class="tex-font-style-tt">b</span>' only. The <span class="tex-span"><i>i</i></span>-th character should be '<span class="tex-font-style-tt">r</span>' if the <span class="tex-span"><i>i</i></span>-th shield should be painted red in the optimal answer and '<span class="tex-font-style-tt">b</span>' if it should be painted blue. The cost of painting shields in these colors should be equal the minimum cost you printed on the first line.</p><p>If there exist more than one optimal solution, print any of them.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100 000</span>)&nbsp;— the number of shields and the number of constraints respectively.</p><p>The second line contains two integers <span class="tex-span"><i>r</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>r</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the shields coordinates. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the constrains. The <span class="tex-span"><i>j</i></span>-th of these lines contains three integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ 2, 1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>d</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>If satisfying all the constraints is impossible print <span class="tex-font-style-tt">-1</span> in first and only line of the output.</p><p>Otherwise, print the minimum total cost in the first line of output. In the second line print a string of length <span class="tex-span"><i>n</i></span> consisting of letters '<span class="tex-font-style-tt">r</span>' and '<span class="tex-font-style-tt">b</span>' only. The <span class="tex-span"><i>i</i></span>-th character should be '<span class="tex-font-style-tt">r</span>' if the <span class="tex-span"><i>i</i></span>-th shield should be painted red in the optimal answer and '<span class="tex-font-style-tt">b</span>' if it should be painted blue. The cost of painting shields in these colors should be equal the minimum cost you printed on the first line.</p><p>If there exist more than one optimal solution, print any of them.</p>





```input1
5 6
8 3
2 10
1 5
9 10
9 10
2 8
1 9 1
1 2 1
2 10 3
2 10 2
1 1 1
2 5 2

```




```input2
4 4
7 3
10 3
9 8
10 3
2 8
2 8 0
2 8 0
1 2 0
1 9 0

```




```output1
25
rbrbb

```




```output2
-1

```


