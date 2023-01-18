## Description

<div><p>Arkady and Masha want to choose decorations for thier aquarium in Fishdom game. They have <span class="tex-span"><i>n</i></span> decorations to choose from, each of them has some cost. To complete a task Arkady and Masha need to choose <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>m</i></span> decorations from given, and they want to spend as little money as possible.</p><p>There is one difficulty: Masha likes some <span class="tex-span"><i>a</i></span> of the given decorations, Arkady likes some <span class="tex-span"><i>b</i></span> of the given decorations. Some decorations may be liked by both Arkady and Masha, or not be liked by both. The friends want to choose such decorations so that each of them likes <span class="tex-font-style-bf">at least</span> <span class="tex-span"><i>k</i></span> decorations among the chosen. Help Masha and Arkady find the minimum sum of money they need to spend.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of decorations, how many decorations the friends should choose, how many decorations each of them should like among the chosen.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— decorations costs.</p><p>The third line contains single integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i></span>)&nbsp;— the number of decorations liked by Masha. The fourth line contains <span class="tex-span"><i>a</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>a</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the ids of decorations liked by Masha.</p><p>The next two lines describe decorations liked by Arkady in the same format.</p></div><div class="output-specification"><p>Print single integer: the minimum sum of money the friends should spend to fulfill all constraints. If it is not possible, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of decorations, how many decorations the friends should choose, how many decorations each of them should like among the chosen.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— decorations costs.</p><p>The third line contains single integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i></span>)&nbsp;— the number of decorations liked by Masha. The fourth line contains <span class="tex-span"><i>a</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>a</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the ids of decorations liked by Masha.</p><p>The next two lines describe decorations liked by Arkady in the same format.</p>

## Output

<p>Print single integer: the minimum sum of money the friends should spend to fulfill all constraints. If it is not possible, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
4 3 2
3 2 2 1
2
1 2
2
1 3

```




```input2
4 3 2
3 2 2 1
2
1 2
3
4 1 3

```




```input3
4 2 2
3 2 2 1
2
1 2
3
4 1 3

```




```output1
7

```




```output2
6

```




```output3
-1

```



## Note

<p>In the first example the only possible variant to choose <span class="tex-span">3</span> decorations having all conditions satisfied is to choose decorations <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>.</p><p>In the second example friends can choose decoration <span class="tex-span">4</span> instead of decoration <span class="tex-span">3</span>, because this one is one coin cheaper.</p><p>In the third example it's not possible to choose <span class="tex-span">2</span> decorations in a way that both are liked by both Masha and Arkady.</p>
