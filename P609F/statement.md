## Description

<div><p>There are <span class="tex-span"><i>n</i></span> frogs sitting on the coordinate axis <span class="tex-span"><i>Ox</i></span>. For each frog two values <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span> are known — the position and the initial length of the tongue of the <span class="tex-span"><i>i</i></span>-th frog (it is guaranteed that all positions <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are different). <span class="tex-span"><i>m</i></span> mosquitoes one by one are landing to the coordinate axis. For each mosquito two values are known <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub></span> — the coordinate of the position where the <span class="tex-span"><i>j</i></span>-th mosquito lands and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> — the size of the <span class="tex-span"><i>j</i></span>-th mosquito. Frogs and mosquitoes are represented as points on the coordinate axis.</p><p>The frog can eat mosquito if mosquito is in the same position with the frog or to the right, and the distance between them is not greater than the length of the tongue of the frog.</p><p>If at some moment several frogs can eat a mosquito the leftmost frog will eat it (with minimal <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>). After eating a mosquito the length of the tongue of a frog increases with the value of the size of eaten mosquito. It's possible that after it the frog will be able to eat some other mosquitoes (the frog should eat them in this case).</p><p>For each frog print two values — the number of eaten mosquitoes and the length of the tongue after landing all mosquitoes and after eating all possible mosquitoes by frogs.</p><p>Each mosquito is landing to the coordinate axis only after frogs eat all possible mosquitoes landed before. Mosquitoes are given in order of their landing to the coordinate axis.</p></div><div class="input-specification"><p>First line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of frogs and mosquitoes.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the position and the initial length of the tongue of the <span class="tex-span"><i>i</i></span>-th frog. It is guaranteed that all <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are different.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain two integers each <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the position and the size of the <span class="tex-span"><i>j</i></span>-th mosquito.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain two integer values <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> — the number of mosquitoes eaten by the <span class="tex-span"><i>i</i></span>-th frog and the length of the tongue of the <span class="tex-span"><i>i</i></span>-th frog.</p></div>

## Input

<p>First line contains two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of frogs and mosquitoes.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the position and the initial length of the tongue of the <span class="tex-span"><i>i</i></span>-th frog. It is guaranteed that all <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> are different.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain two integers each <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the position and the size of the <span class="tex-span"><i>j</i></span>-th mosquito.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line should contain two integer values <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub></span> — the number of mosquitoes eaten by the <span class="tex-span"><i>i</i></span>-th frog and the length of the tongue of the <span class="tex-span"><i>i</i></span>-th frog.</p>





```input1
4 6
10 2
15 0
6 1
0 1
110 10
1 1
6 0
15 10
14 100
12 2

```




```input2
1 2
10 2
20 2
12 1

```




```output1
3 114
1 10
1 1
1 2

```




```output2
1 3

```


