## Description

<div><p>For each string <span class="tex-span"><i>s</i></span> consisting of characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>' one can define four integers <span class="tex-span"><i>a</i><sub class="lower-index">00</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">01</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">10</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">11</sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>xy</i></sub></span> is the number of <span class="tex-font-style-bf">subsequences</span> of length <span class="tex-span">2</span> of the string <span class="tex-span"><i>s</i></span> equal to the sequence <span class="tex-span">{<i>x</i>, <i>y</i>}</span>. </p><p>In these problem you are given four integers <span class="tex-span"><i>a</i><sub class="lower-index">00</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">01</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">10</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">11</sub></span> and have to find any non-empty string <span class="tex-span"><i>s</i></span> that matches them, or determine that there is no such string. One can prove that if at least one answer exists, there exists an answer of length no more than <span class="tex-span">1 000 000</span>.</p></div><div class="input-specification"><p>The only line of the input contains four non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">00</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">01</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">10</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">11</sub></span>. Each of them doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>If there exists a non-empty string that matches four integers from the input, print it in the only line of the output. Otherwise, print "<span class="tex-font-style-tt">Impossible</span>". The length of your answer must not exceed <span class="tex-span">1 000 000</span>.</p></div>

## Input

<p>The only line of the input contains four non-negative integers <span class="tex-span"><i>a</i><sub class="lower-index">00</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">01</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">10</sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index">11</sub></span>. Each of them doesn't exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>If there exists a non-empty string that matches four integers from the input, print it in the only line of the output. Otherwise, print "<span class="tex-font-style-tt">Impossible</span>". The length of your answer must not exceed <span class="tex-span">1 000 000</span>.</p>





```input1
1 2 3 4

```




```input2
1 2 2 1

```




```output1
Impossible

```




```output2
0110

```


