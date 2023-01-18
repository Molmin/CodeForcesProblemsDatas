## Description

<div><p>Ivan has an array consisting of <span class="tex-span"><i>n</i></span> elements. Each of the elements is an integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>Recently Ivan learned about permutations and their lexicographical order. Now he wants to change (replace) <span class="tex-font-style-it">minimum</span> number of elements in his array in such a way that his array becomes a <span class="tex-font-style-it">permutation</span> (i.e. each of the integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> was encountered in his array exactly once). If there are multiple ways to do it he wants to find the <span class="tex-font-style-it">lexicographically minimal</span> permutation among them.</p><p>Thus minimizing the number of changes has the first priority, lexicographical minimizing has the second priority.</p><p>In order to determine which of the two permutations is lexicographically smaller, we compare their first elements. If they are equal — compare the second, and so on. If we have two permutations <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>, then <span class="tex-span"><i>x</i></span> is lexicographically smaller if <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>i</i></span> is the first index in which the permutations <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> differ.</p><p>Determine the array Ivan will obtain after performing all the changes.</p></div><div class="input-specification"><p>The first line contains an single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>) — the number of elements in Ivan's array.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the description of Ivan's array.</p></div><div class="output-specification"><p>In the first line print <span class="tex-span"><i>q</i></span> — the minimum number of elements that need to be changed in Ivan's array in order to make his array a permutation. In the second line, print the <span class="tex-font-style-it">lexicographically minimal</span> permutation which can be obtained from array with <span class="tex-span"><i>q</i></span> changes.</p></div>

## Input

<p>The first line contains an single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 200 000</span>) — the number of elements in Ivan's array.</p><p>The second line contains a sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the description of Ivan's array.</p>

## Output

<p>In the first line print <span class="tex-span"><i>q</i></span> — the minimum number of elements that need to be changed in Ivan's array in order to make his array a permutation. In the second line, print the <span class="tex-font-style-it">lexicographically minimal</span> permutation which can be obtained from array with <span class="tex-span"><i>q</i></span> changes.</p>





```input1
4
3 2 2 3

```




```input2
6
4 5 6 3 2 1

```




```input3
10
6 8 4 6 7 1 6 3 4 5

```




```output1
2
1 2 4 3 

```




```output2
0
4 5 6 3 2 1 

```




```output3
3
2 8 4 6 7 1 9 3 10 5 

```



## Note

<p>In the first example Ivan needs to replace number three in position <span class="tex-span">1</span> with number one, and number two in position <span class="tex-span">3</span> with number four. Then he will get a permutation <span class="tex-font-style-tt">[1, 2, 4, 3]</span> with only two changed numbers — this permutation is lexicographically minimal among all suitable. </p><p>In the second example Ivan does not need to change anything because his array already is a permutation.</p>
