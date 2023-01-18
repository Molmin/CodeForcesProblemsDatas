## Description

<div><p>You are given the set of vectors on the plane, each of them starting at the origin. Your task is to find a pair of vectors with the minimal non-oriented angle between them.</p><p>Non-oriented angle is non-negative value, minimal between clockwise and counterclockwise direction angles. Non-oriented angle is always between <span class="tex-span">0</span> and <span class="tex-span">π</span>. For example, opposite directions vectors have angle equals to <span class="tex-span">π</span>.</p></div><div class="input-specification"><p>First line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of vectors.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i>|, |<i>y</i>| ≤ 10 000, <i>x</i><sup class="upper-index">2</sup> + <i>y</i><sup class="upper-index">2</sup> &gt; 0</span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th vector. Vectors are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in order of appearing in the input. It is guaranteed that no two vectors in the input share the same direction (but they still can have opposite directions).</p></div><div class="output-specification"><p>Print two integer numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> ≠ <i>b</i></span>)&nbsp;— a pair of indices of vectors with the minimal non-oriented angle. You can print the numbers in any order. If there are many possible answers, print any.</p></div>

## Input

<p>First line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of vectors.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>x</i>|, |<i>y</i>| ≤ 10 000, <i>x</i><sup class="upper-index">2</sup> + <i>y</i><sup class="upper-index">2</sup> &gt; 0</span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th vector. Vectors are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in order of appearing in the input. It is guaranteed that no two vectors in the input share the same direction (but they still can have opposite directions).</p>

## Output

<p>Print two integer numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> ≠ <i>b</i></span>)&nbsp;— a pair of indices of vectors with the minimal non-oriented angle. You can print the numbers in any order. If there are many possible answers, print any.</p>





```input1
4
-1 0
0 -1
1 0
1 1

```




```input2
6
-1 0
0 -1
1 0
1 1
-4 -5
-4 -6

```




```output1
3 4

```




```output2
6 5
```


