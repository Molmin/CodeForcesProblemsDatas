## Description

<div><p>Today at the lesson Vitya learned a very interesting function&nbsp;— <span class="tex-font-style-it">mex</span>. <span class="tex-font-style-it">Mex</span> of a sequence of numbers is the minimum non-negative number that is not present in the sequence as element. For example, <span class="tex-span"><i>mex</i>([4, 33, 0, 1, 1, 5]) = 2</span> and <span class="tex-span"><i>mex</i>([1, 2, 3]) = 0</span>.</p><p>Vitya quickly understood all tasks of the teacher, but can you do the same?</p><p>You are given an array consisting of <span class="tex-span"><i>n</i></span> non-negative integers, and <span class="tex-span"><i>m</i></span> queries. Each query is characterized by one number <span class="tex-span"><i>x</i></span> and consists of the following consecutive steps:</p><ul> <li> Perform the bitwise addition operation modulo <span class="tex-span">2</span> (<span class="tex-font-style-it">xor</span>) of each array element with the number <span class="tex-span"><i>x</i></span>. </li><li> Find <span class="tex-font-style-it">mex</span> of the resulting array. </li></ul><p><span class="tex-font-style-it">Note that after each query the array changes.</span></p></div><div class="input-specification"><p>First line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— number of elements in array and number of queries.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— elements of then array.</p><p>Each of next <span class="tex-span"><i>m</i></span> lines contains query&nbsp;— one integer number <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>For each query print the answer on a separate line.</p></div>

## Input

<p>First line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— number of elements in array and number of queries.</p><p>Next line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 3·10<sup class="upper-index">5</sup></span>)&nbsp;— elements of then array.</p><p>Each of next <span class="tex-span"><i>m</i></span> lines contains query&nbsp;— one integer number <span class="tex-span"><i>x</i></span> (<span class="tex-span">0 ≤ <i>x</i> ≤ 3·10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>For each query print the answer on a separate line.</p>





```input1
2 2
1 3
1
3

```




```input2
4 3
0 1 5 6
1
2
4

```




```input3
5 4
0 1 5 6 7
1
1
4
5

```




```output1
1
0

```




```output2
2
0
0

```




```output3
2
2
0
2

```


