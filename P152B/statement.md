## Description

<div><p>One day Vasya went out for a walk in the yard but there weren't any of his friends outside and he had no one to play touch and run. But the boy didn't lose the high spirits and decided to play touch and run with himself. You may ask: "How did he do that?" The answer is simple.</p><p>Vasya noticed that the yard is a rectangular <span class="tex-span"><i>n</i> × <i>m</i></span> field. The squares have coordinates <span class="tex-span">(<i>x</i>, <i>y</i>)</span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i>, 1 ≤ <i>y</i> ≤ <i>m</i></span>), where <span class="tex-span"><i>x</i></span> is the index of the row and <span class="tex-span"><i>y</i></span> is the index of the column.</p><p>Initially Vasya stands in the square with coordinates (<span class="tex-span"><i>x</i><sub class="lower-index"><i>c</i></sub>, <i>y</i><sub class="lower-index"><i>c</i></sub></span>). To play, he has got a list of <span class="tex-span"><i>k</i></span> vectors <span class="tex-span">(<i>dx</i><sub class="lower-index"><i>i</i></sub>, <i>dy</i><sub class="lower-index"><i>i</i></sub>)</span> of non-zero length. The game goes like this. The boy considers all vectors in the order from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>, and consecutively chooses each vector as the current one. After the boy has chosen a current vector, he makes the maximally possible number of valid steps in the vector's direction (it is possible that he makes zero steps).</p><p>A <span class="tex-font-style-it">step</span> is defined as one movement from the square where the boy is standing now, in the direction of the current vector. That is, if Vasya is positioned in square <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, and the current vector is <span class="tex-span">(<i>dx</i>, <i>dy</i>)</span>, one step moves Vasya to square <span class="tex-span">(<i>x</i> + <i>dx</i>, <i>y</i> + <i>dy</i>)</span>. A step is considered <span class="tex-font-style-it">valid</span>, if the boy does not go out of the yard if he performs the step.</p><p>Vasya stepped on and on, on and on until he ran out of vectors in his list. Ha had been stepping for so long that he completely forgot how many steps he had made. Help the boy and count how many steps he had made.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>) — the yard's sizes. The second line contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>c</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>c</i></sub></span> — the initial square's coordinates (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>c</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>c</i></sub> ≤ <i>m</i></span>).</p><p>The third line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of vectors. Then follow <span class="tex-span"><i>k</i></span> lines, each of them contains two integers <span class="tex-span"><i>dx</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>dy</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>dx</i><sub class="lower-index"><i>i</i></sub>|, |<i>dy</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>, |<i>dx</i>| + |<i>dy</i>| ≥ 1)</span>.</p></div><div class="output-specification"><p>Print the single number — the number of steps Vasya had made.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>) — the yard's sizes. The second line contains integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>c</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>c</i></sub></span> — the initial square's coordinates (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>c</i></sub> ≤ <i>n</i>, 1 ≤ <i>y</i><sub class="lower-index"><i>c</i></sub> ≤ <i>m</i></span>).</p><p>The third line contains an integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of vectors. Then follow <span class="tex-span"><i>k</i></span> lines, each of them contains two integers <span class="tex-span"><i>dx</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>dy</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(|<i>dx</i><sub class="lower-index"><i>i</i></sub>|, |<i>dy</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup>, |<i>dx</i>| + |<i>dy</i>| ≥ 1)</span>.</p>

## Output

<p>Print the single number — the number of steps Vasya had made.</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specificator.</p>





```input1
4 5
1 1
3
1 1
1 1
0 -2

```




```input2
10 10
1 2
1
-1 0

```




```output1
4

```




```output2
0

```



## Note

<p>In the first sample Vasya is initially positioned at square <span class="tex-span">(1, 1)</span> and makes <span class="tex-span">3</span> steps by the first vector <span class="tex-span">(1, 1)</span>. So, he consecutively visits the squares <span class="tex-span">(2, 2), (3, 3), (4, 4)</span>. Then he makes <span class="tex-span">0</span> steps by the second vector <span class="tex-span">(1, 1)</span>. He makes <span class="tex-span">1</span> more step by the third vector <span class="tex-span">(0,  - 2)</span> and he ends up in square <span class="tex-span">(4, 2)</span>. Overall, Vasya makes <span class="tex-span">4</span> steps.</p><p>In the second sample Vasya is initially positioned in square <span class="tex-span">(1, 2)</span> and makes <span class="tex-span">0</span> steps by vector <span class="tex-span">( - 1, 0)</span>, as the square with coordinates <span class="tex-span">(0, 2)</span> is located outside the yard.</p>
