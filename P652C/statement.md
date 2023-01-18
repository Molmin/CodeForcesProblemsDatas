## Description

<div><p>You are given a permutation <span class="tex-span"><i>p</i></span> of length <span class="tex-span"><i>n</i></span>. Also you are given <span class="tex-span"><i>m</i></span> foe pairs <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). </p><p>Your task is to count the number of different intervals <span class="tex-span">(<i>x</i>, <i>y</i>)</span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>y</i> ≤ <i>n</i></span>) that do not contain any foe pairs. So you shouldn't count intervals <span class="tex-span">(<i>x</i>, <i>y</i>)</span> that contain at least one foe pair in it (the positions and order of the values from the foe pair are not important).</p><p>Consider some example: <span class="tex-span"><i>p</i> = [1, 3, 2, 4]</span> and foe pairs are <span class="tex-span">{(3, 2), (4, 2)}</span>. The interval <span class="tex-span">(1, 3)</span> is incorrect because it contains a foe pair <span class="tex-span">(3, 2)</span>. The interval <span class="tex-span">(1, 4)</span> is also incorrect because it contains two foe pairs <span class="tex-span">(3, 2)</span> and <span class="tex-span">(4, 2)</span>. But the interval <span class="tex-span">(1, 2)</span> is correct because it doesn't contain any foe pair.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the length of the permutation <span class="tex-span"><i>p</i></span> and the number of foe pairs.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the elements of the permutation <span class="tex-span"><i>p</i></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — the <span class="tex-span"><i>i</i></span>-th foe pair. Note a foe pair can appear multiple times in the given list.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>c</i></span> — the number of different intervals <span class="tex-span">(<i>x</i>, <i>y</i>)</span> that does not contain any foe pairs.</p><p>Note that the answer can be too large, so you should use <span class="tex-span">64</span>-bit integer type to store it. In <span class="tex-font-style-tt">C++</span> you can use the <span class="tex-font-style-tt">long long</span> integer type and in <span class="tex-font-style-tt">Java</span> you can use <span class="tex-font-style-tt">long</span> integer type.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the length of the permutation <span class="tex-span"><i>p</i></span> and the number of foe pairs.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the elements of the permutation <span class="tex-span"><i>p</i></span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>) — the <span class="tex-span"><i>i</i></span>-th foe pair. Note a foe pair can appear multiple times in the given list.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>c</i></span> — the number of different intervals <span class="tex-span">(<i>x</i>, <i>y</i>)</span> that does not contain any foe pairs.</p><p>Note that the answer can be too large, so you should use <span class="tex-span">64</span>-bit integer type to store it. In <span class="tex-font-style-tt">C++</span> you can use the <span class="tex-font-style-tt">long long</span> integer type and in <span class="tex-font-style-tt">Java</span> you can use <span class="tex-font-style-tt">long</span> integer type.</p>





```input1
4 2
1 3 2 4
3 2
2 4

```




```input2
9 5
9 7 2 3 1 4 6 5 8
1 6
4 5
2 7
7 2
2 7

```




```output1
5

```




```output2
20

```



## Note

<p>In the first example the intervals from the answer are <span class="tex-span">(1, 1)</span>, <span class="tex-span">(1, 2)</span>, <span class="tex-span">(2, 2)</span>, <span class="tex-span">(3, 3)</span> and <span class="tex-span">(4, 4)</span>.</p>
