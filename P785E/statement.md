## Description

<div><p>Anton likes permutations, especially he likes to permute their elements. Note that a permutation of <span class="tex-span"><i>n</i></span> elements is a sequence of numbers <span class="tex-span">{<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>}</span>, in which every number from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> appears exactly once.</p><p>One day Anton got a new permutation and started to play with it. He does the following operation <span class="tex-span"><i>q</i></span> times: he takes two elements of the permutation and swaps these elements. After each operation he asks his friend Vanya, how many inversions there are in the new permutation. The number of inversions in a permutation is the number of distinct pairs <span class="tex-span">(<i>i</i>, <i>j</i>)</span> such that <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; <i>a</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>Vanya is tired of answering Anton's silly questions. So he asked you to write a program that would answer these questions instead of him.</p><p>Initially Anton's permutation was <span class="tex-span">{1, 2, ..., <i>n</i>}</span>, that is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>i</i></span> for all <span class="tex-span"><i>i</i></span> such that <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200 000, 1 ≤ <i>q</i> ≤ 50 000)</span>&nbsp;— the length of the permutation and the number of operations that Anton does.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines of the input contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>&nbsp;— the indices of elements that Anton swaps during the <span class="tex-span"><i>i</i></span>-th operation. Note that indices of elements that Anton swaps during the <span class="tex-span"><i>i</i></span>-th operation can coincide. Elements in the permutation are numbered starting with one.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>q</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line of the output is the number of inversions in the Anton's permutation after the <span class="tex-span"><i>i</i></span>-th operation.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 200 000, 1 ≤ <i>q</i> ≤ 50 000)</span>&nbsp;— the length of the permutation and the number of operations that Anton does.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines of the input contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>&nbsp;— the indices of elements that Anton swaps during the <span class="tex-span"><i>i</i></span>-th operation. Note that indices of elements that Anton swaps during the <span class="tex-span"><i>i</i></span>-th operation can coincide. Elements in the permutation are numbered starting with one.</p>

## Output

<p>Output <span class="tex-span"><i>q</i></span> lines. The <span class="tex-span"><i>i</i></span>-th line of the output is the number of inversions in the Anton's permutation after the <span class="tex-span"><i>i</i></span>-th operation.</p>





```input1
5 4
4 5
2 4
2 5
2 2

```




```input2
2 1
2 1

```




```input3
6 7
1 4
3 5
2 3
3 3
3 6
2 1
5 1

```




```output1
1
4
3
3

```




```output2
1

```




```output3
5
6
7
7
10
11
8

```



## Note

<p>Consider the first sample.</p><p>After the first Anton's operation the permutation will be <span class="tex-span">{1, 2, 3, 5, 4}</span>. There is only one inversion in it: <span class="tex-span">(4, 5)</span>.</p><p>After the second Anton's operation the permutation will be <span class="tex-span">{1, 5, 3, 2, 4}</span>. There are four inversions: <span class="tex-span">(2, 3)</span>, <span class="tex-span">(2, 4)</span>, <span class="tex-span">(2, 5)</span> and <span class="tex-span">(3, 4)</span>.</p><p>After the third Anton's operation the permutation will be <span class="tex-span">{1, 4, 3, 2, 5}</span>. There are three inversions: <span class="tex-span">(2, 3)</span>, <span class="tex-span">(2, 4)</span> and <span class="tex-span">(3, 4)</span>.</p><p>After the fourth Anton's operation the permutation doesn't change, so there are still three inversions.</p>
