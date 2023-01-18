## Description

<div><p>Yasin has an array <span class="tex-span"><i>a</i></span> containing <span class="tex-span"><i>n</i></span> integers. Yasin is a 5 year old, so he loves ultimate weird things.</p><p>Yasin denotes <span class="tex-font-style-it">weirdness</span> of an array as maximum <span class="tex-span"><i>gcd</i>(<i>a</i><sub class="lower-index"><i>i</i></sub>,  <i>a</i><sub class="lower-index"><i>j</i></sub>)</span> value among all <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>. For <span class="tex-span"><i>n</i> ≤ 1</span> weirdness is equal to <span class="tex-span">0</span>, <span class="tex-span"><i>gcd</i>(<i>x</i>,  <i>y</i>)</span> is the greatest common divisor of integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>.</p><p>He also defines the <span class="tex-font-style-it">ultimate weirdness</span> of an array. Ultimate weirdness is <img align="middle" class="tex-formula" src="file://zZ3br75O.png" style="max-width: 100.0%;max-height: 100.0%;"> where <span class="tex-span"><i>f</i>(<i>i</i>,  <i>j</i>)</span> is weirdness of the new array <span class="tex-span"><i>a</i></span> obtained by removing all elements between <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> inclusive, so new array is <span class="tex-span">[<i>a</i><sub class="lower-index">1</sub>... <i>a</i><sub class="lower-index"><i>i</i> - 1</sub>, <i>a</i><sub class="lower-index"><i>j</i> + 1</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub>]</span>.</p><p>Since 5 year old boys can't code, Yasin asks for your help to find the value of ultimate weirdness of the given array <span class="tex-span"><i>a</i></span>!</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of elements in <span class="tex-span"><i>a</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 200 000</span>), where the <span class="tex-span"><i>i</i></span>-th number is equal to the <span class="tex-span"><i>i</i></span>-th element of the array <span class="tex-span"><i>a</i></span>. It is guaranteed that all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p></div><div class="output-specification"><p>Print a single line containing the value of ultimate weirdness of the array <span class="tex-span"><i>a</i></span>. </p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of elements in <span class="tex-span"><i>a</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 200 000</span>), where the <span class="tex-span"><i>i</i></span>-th number is equal to the <span class="tex-span"><i>i</i></span>-th element of the array <span class="tex-span"><i>a</i></span>. It is guaranteed that all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are distinct.</p>

## Output

<p>Print a single line containing the value of ultimate weirdness of the array <span class="tex-span"><i>a</i></span>. </p>





```input1
3
2 6 3

```




```output1
6

```



## Note

<p>Consider the first sample.</p><ul> <li> <span class="tex-span"><i>f</i>(1,  1)</span> is equal to <span class="tex-span">3</span>. </li><li> <span class="tex-span"><i>f</i>(2,  2)</span> is equal to <span class="tex-span">1</span>. </li><li> <span class="tex-span"><i>f</i>(3,  3)</span> is equal to <span class="tex-span">2</span>. </li><li> <span class="tex-span"><i>f</i>(1,  2)</span>, <span class="tex-span"><i>f</i>(1,  3)</span> and <span class="tex-span"><i>f</i>(2,  3)</span> are equal to <span class="tex-span">0</span>. </li></ul> Thus the answer is <span class="tex-span">3 + 0 + 0 + 1 + 0 + 2 = 6</span>.
