## Description

<div><p>Let <span class="tex-span"><i>a</i></span> be an array consisting of <span class="tex-span"><i>n</i></span> numbers. The array's elements are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>even</i></span> is an array consisting of the numerals whose numbers are even in <span class="tex-span"><i>a</i></span> (<span class="tex-span"><i>even</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index">2<i>i</i></sub></span>, <span class="tex-span">1 ≤ 2<i>i</i> ≤ <i>n</i></span>), <span class="tex-span"><i>odd</i></span> is an array consisting of the numberals whose numbers are odd in <span class="tex-span"><i>а</i></span> (<span class="tex-span"><i>odd</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index">2<i>i</i> - 1</sub></span>, <span class="tex-span">1 ≤ 2<i>i</i> - 1 ≤ <i>n</i></span>). Then let's define the transformation of array <span class="tex-span"><i>F</i>(<i>a</i>)</span> in the following manner:</p><ul> <li> if <span class="tex-span"><i>n</i> &gt; 1</span>, <span class="tex-span"><i>F</i>(<i>a</i>) = <i>F</i>(<i>odd</i>) + <i>F</i>(<i>even</i>)</span>, where operation "<span class="tex-span"> + </span>" stands for the arrays' concatenation (joining together) </li><li> if <span class="tex-span"><i>n</i> = 1</span>, <span class="tex-span"><i>F</i>(<i>a</i>) = <i>a</i></span> </li></ul><p>Let <span class="tex-span"><i>a</i></span> be an array consisting of <span class="tex-span"><i>n</i></span> numbers <span class="tex-span">1, 2, 3, ..., <i>n</i></span>. Then <span class="tex-span"><i>b</i></span> is the result of applying the transformation to the array <span class="tex-span"><i>a</i></span> (so <span class="tex-span"><i>b</i> = <i>F</i>(<i>a</i>)</span>). You are given <span class="tex-span"><i>m</i></span> queries <span class="tex-span">(<i>l</i>, <i>r</i>, <i>u</i>, <i>v</i>)</span>. Your task is to find for each query the sum of numbers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, such that <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> and <span class="tex-span"><i>u</i> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>v</i></span>. You should print the query results modulo <span class="tex-span"><i>mod</i></span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>mod</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>mod</i> ≤ 10<sup class="upper-index">9</sup></span>). Next <span class="tex-span"><i>m</i></span> lines describe the queries. Each query is defined by four integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>u</i> ≤ <i>v</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. Use <span class="tex-font-style-tt">%I64d</span> specificator.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines each containing an integer — remainder modulo <span class="tex-span"><i>mod</i></span> of the query result.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>mod</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">18</sup>, 1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>mod</i> ≤ 10<sup class="upper-index">9</sup></span>). Next <span class="tex-span"><i>m</i></span> lines describe the queries. Each query is defined by four integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>u</i> ≤ <i>v</i> ≤ 10<sup class="upper-index">18</sup></span>).</p><p>Please do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. Use <span class="tex-font-style-tt">%I64d</span> specificator.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines each containing an integer — remainder modulo <span class="tex-span"><i>mod</i></span> of the query result.</p>





```input1
4 5 10000
2 3 4 5
2 4 1 3
1 2 2 4
2 3 3 5
1 3 3 4

```




```input2
2 5 10000
1 2 2 2
1 1 4 5
1 1 2 5
1 1 1 3
1 2 5 5

```




```output1
0
5
3
3
3

```




```output2
2
0
0
1
0

```



## Note

<p>Let's consider the first example. First let's construct an array <span class="tex-span"><i>b</i> = <i>F</i>(<i>a</i>) = <i>F</i>([1, 2, 3, 4])</span>. </p><ul> <li> Step 1. <span class="tex-span"><i>F</i>([1, 2, 3, 4]) = <i>F</i>([1, 3]) + <i>F</i>([2, 4])</span> </li><li> Step 2. <span class="tex-span"><i>F</i>([1, 3]) = <i>F</i>([1]) + <i>F</i>([3]) = [1] + [3] = [1, 3]</span> </li><li> Step 3. <span class="tex-span"><i>F</i>([2, 4]) = <i>F</i>([2]) + <i>F</i>([4]) = [2] + [4] = [2, 4]</span> </li><li> Step 4. <span class="tex-span"><i>b</i> = <i>F</i>([1, 2, 3, 4]) = <i>F</i>([1, 3]) + <i>F</i>([2, 4]) = [1, 3] + [2, 4] = [1, 3, 2, 4]</span> </li></ul> Thus <span class="tex-span"><i>b</i> = [1, 3, 2, 4]</span>. Let's consider the first query <span class="tex-span"><i>l</i> = 2, <i>r</i> = 3, <i>u</i> = 4, <i>v</i> = 5</span>. The second and third positions in the array <span class="tex-span"><i>b</i></span> do not have numbers in the range <span class="tex-span">[4, 5]</span>, so the sum obviously equals zero. Let's consider the second query <span class="tex-span"><i>l</i> = 2, <i>r</i> = 4, <i>u</i> = 1, <i>v</i> = 3</span>. The second and third positions have two numbers that belong to the range <span class="tex-span">[1, 3]</span>, their sum equals 5.
