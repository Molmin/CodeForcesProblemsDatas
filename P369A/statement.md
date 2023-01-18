## Description

<div><p>Valera is a lazy student. He has <span class="tex-span"><i>m</i></span> clean bowls and <span class="tex-span"><i>k</i></span> clean plates. </p><p>Valera has made an eating plan for the next <span class="tex-span"><i>n</i></span> days. As Valera is lazy, he will eat exactly one dish per day. At that, in order to eat a dish, he needs exactly one <span class="tex-font-style-it">clean</span> plate or bowl. We know that Valera can cook only two types of dishes. He can eat dishes of the first type from bowls and dishes of the second type from either bowls or plates. </p><p>When Valera finishes eating, he leaves a dirty plate/bowl behind. His life philosophy doesn't let him eat from dirty kitchenware. So sometimes he needs to wash his plate/bowl <span class="tex-font-style-bf">before eating</span>. Find the minimum number of times Valera will need to wash a plate/bowl, if he acts optimally.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 1000</span>)&nbsp;— the number of the planned days, the number of clean bowls and the number of clean plates.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>). If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals one, then on day <span class="tex-span"><i>i</i></span> Valera will eat a first type dish. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals two, then on day <span class="tex-span"><i>i</i></span> Valera will eat a second type dish. </p></div><div class="output-specification"><p>Print a single integer — the minimum number of times Valera will need to wash a plate/bowl.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 1000</span>)&nbsp;— the number of the planned days, the number of clean bowls and the number of clean plates.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 2</span>). If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals one, then on day <span class="tex-span"><i>i</i></span> Valera will eat a first type dish. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals two, then on day <span class="tex-span"><i>i</i></span> Valera will eat a second type dish. </p>

## Output

<p>Print a single integer — the minimum number of times Valera will need to wash a plate/bowl.</p>





```input1
3 1 1
1 2 1

```




```input2
4 3 1
1 1 1 1

```




```input3
3 1 2
2 2 2

```




```input4
8 2 2
1 2 1 2 1 2 1 2

```




```output1
1

```




```output2
1

```




```output3
0

```




```output4
4

```



## Note

<p>In the first sample Valera will wash a bowl only on the third day, so the answer is one.</p><p>In the second sample, Valera will have the first type of the dish during all four days, and since there are only three bowls, he will wash a bowl exactly once.</p><p>In the third sample, Valera will have the second type of dish for all three days, and as they can be eaten from either a plate or a bowl, he will never need to wash a plate/bowl.</p>
