## Description

<div><p>At the Byteland State University marks are strings of the same length. Mark <span class="tex-span"><i>x</i></span> is considered better than <span class="tex-span"><i>y</i></span> if string <span class="tex-span"><i>y</i></span> is lexicographically smaller than <span class="tex-span"><i>x</i></span>.</p><p>Recently at the BSU was an important test work on which Vasya recived the mark <span class="tex-span"><i>a</i></span>. It is very hard for the teacher to remember the exact mark of every student, but he knows the mark <span class="tex-span"><i>b</i></span>, such that every student recieved mark strictly smaller than <span class="tex-span"><i>b</i></span>.</p><p>Vasya isn't satisfied with his mark so he decided to improve it. He can swap characters in the string corresponding to his mark as many times as he like. Now he want to know only the number of different ways to improve his mark so that his teacher didn't notice something suspicious.</p><p>More formally: you are given two strings <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> of the same length and you need to figure out the number of different strings <span class="tex-span"><i>c</i></span> such that:</p><p>1) <span class="tex-span"><i>c</i></span> can be obtained from <span class="tex-span"><i>a</i></span> by swapping some characters, in other words <span class="tex-span"><i>c</i></span> is a permutation of <span class="tex-span"><i>a</i></span>.</p><p>2) String <span class="tex-span"><i>a</i></span> is lexicographically smaller than <span class="tex-span"><i>c</i></span>.</p><p>3) String <span class="tex-span"><i>c</i></span> is lexicographically smaller than <span class="tex-span"><i>b</i></span>.</p><p>For two strings <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> of the same length it is true that <span class="tex-span"><i>x</i></span> is lexicographically smaller than <span class="tex-span"><i>y</i></span> if there exists such <span class="tex-span"><i>i</i></span>, that <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> = <i>y</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub> = <i>y</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>i</i> - 1</sub> = <i>y</i><sub class="lower-index"><i>i</i> - 1</sub>, <i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Since the answer can be very large, you need to find answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>First line contains string <span class="tex-span"><i>a</i></span>, second line contains string <span class="tex-span"><i>b</i></span>. Strings <span class="tex-span"><i>a</i>, <i>b</i></span> consist of lowercase English letters. Their lengths are equal and don't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>It is guaranteed that <span class="tex-span"><i>a</i></span> is lexicographically smaller than <span class="tex-span"><i>b</i></span>.</p></div><div class="output-specification"><p>Print one integer &nbsp;— the number of different strings satisfying the condition of the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>First line contains string <span class="tex-span"><i>a</i></span>, second line contains string <span class="tex-span"><i>b</i></span>. Strings <span class="tex-span"><i>a</i>, <i>b</i></span> consist of lowercase English letters. Their lengths are equal and don't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p><p>It is guaranteed that <span class="tex-span"><i>a</i></span> is lexicographically smaller than <span class="tex-span"><i>b</i></span>.</p>

## Output

<p>Print one integer &nbsp;— the number of different strings satisfying the condition of the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
abc
ddd

```




```input2
abcdef
abcdeg

```




```input3
abacaba
ubuduba

```




```output1
5

```




```output2
0

```




```output3
64

```



## Note

<p>In first sample from string <span class="tex-span"><i>abc</i></span> can be obtained strings <span class="tex-span"><i>acb</i>, <i>bac</i>, <i>bca</i>, <i>cab</i>, <i>cba</i></span>, all of them are larger than <span class="tex-span"><i>abc</i></span>, but smaller than <span class="tex-span"><i>ddd</i></span>. So the answer is <span class="tex-span">5</span>.</p><p>In second sample any string obtained from <span class="tex-span"><i>abcdef</i></span> is larger than <span class="tex-span"><i>abcdeg</i></span>. So the answer is <span class="tex-span">0</span>.</p>
