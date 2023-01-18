## Description

<div><p>While Vasya finished eating his piece of pizza, the lesson has already started. For being late for the lesson, the teacher suggested Vasya to solve one interesting problem. Vasya has an array <span class="tex-span"><i>a</i></span> and integer <span class="tex-span"><i>x</i></span>. He should find the number of different ordered pairs of indexes <span class="tex-span">(<i>i</i>, <i>j</i>)</span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>j</i></sub></span> and there are exactly <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>y</i></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>y</i> ≤ <i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>y</i></span> is divisible by <span class="tex-span"><i>x</i></span>.</p><p>In this problem it is meant that pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is equal to <span class="tex-span">(<i>j</i>, <i>i</i>)</span> only if <span class="tex-span"><i>i</i></span> is equal to <span class="tex-span"><i>j</i></span>. For example pair <span class="tex-span">(1, 2)</span> is not the same as <span class="tex-span">(2, 1)</span>.</p></div><div class="input-specification"><p>The first line contains 3 integers <span class="tex-span"><i>n</i>, <i>x</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>n</i></span> is the size of the array <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>k</i></span> are numbers from the statement.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the array <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the answer to the problem.</p></div>

## Input

<p>The first line contains 3 integers <span class="tex-span"><i>n</i>, <i>x</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>, 0 ≤ <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>n</i></span> is the size of the array <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>k</i></span> are numbers from the statement.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the array <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Print one integer&nbsp;— the answer to the problem.</p>





```input1
4 2 1
1 3 5 7

```




```input2
4 2 0
5 3 1 7

```




```input3
5 3 1
3 3 3 3 3

```




```output1
3

```




```output2
4

```




```output3
25

```



## Note

<p>In first sample there are only three suitable pairs of indexes&nbsp;— <span class="tex-span">(1, 2), (2, 3), (3, 4)</span>.</p><p>In second sample there are four suitable pairs of indexes<span class="tex-span">(1, 1), (2, 2), (3, 3), (4, 4)</span>.</p><p>In third sample every pair <span class="tex-span">(<i>i</i>, <i>j</i>)</span> is suitable, so the answer is <span class="tex-span">5 * 5 = 25</span>.</p>
