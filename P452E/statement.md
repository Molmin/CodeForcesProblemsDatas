## Description

<div><p>You are given three strings <span class="tex-span">(<i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, <i>s</i><sub class="lower-index">3</sub>)</span>. For each integer <span class="tex-span"><i>l</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>min</i>(|<i>s</i><sub class="lower-index">1</sub>|, |<i>s</i><sub class="lower-index">2</sub>|, |<i>s</i><sub class="lower-index">3</sub>|)</span> you need to find how many triples (<span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, <i>i</i><sub class="lower-index">3</sub></span>) exist such that three strings <span class="tex-span"><i>s</i><sub class="lower-index"><i>k</i></sub>[<i>i</i><sub class="lower-index"><i>k</i></sub>... <i>i</i><sub class="lower-index"><i>k</i></sub> + <i>l</i> - 1]</span> <span class="tex-span">(<i>k</i> = 1, 2, 3)</span> are pairwise equal. Print all found numbers modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p><p>See notes if you are not sure about some of the denotions used in the statement.</p></div><div class="input-specification"><p>First three lines contain three non-empty input strings. The sum of lengths of all strings is no more than <span class="tex-span">3·10<sup class="upper-index">5</sup></span>. All strings consist only of lowercase English letters.</p></div><div class="output-specification"><p>You need to output <span class="tex-span"><i>min</i>(|<i>s</i><sub class="lower-index">1</sub>|, |<i>s</i><sub class="lower-index">2</sub>|, |<i>s</i><sub class="lower-index">3</sub>|)</span> numbers separated by spaces — answers for the problem modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>First three lines contain three non-empty input strings. The sum of lengths of all strings is no more than <span class="tex-span">3·10<sup class="upper-index">5</sup></span>. All strings consist only of lowercase English letters.</p>

## Output

<p>You need to output <span class="tex-span"><i>min</i>(|<i>s</i><sub class="lower-index">1</sub>|, |<i>s</i><sub class="lower-index">2</sub>|, |<i>s</i><sub class="lower-index">3</sub>|)</span> numbers separated by spaces — answers for the problem modulo <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
abc
bc
cbc

```




```input2
abacaba
abac
abcd

```




```output1
3 1 

```




```output2
11 2 0 0 

```



## Note

<p>Consider a string <span class="tex-span"><i>t</i> = <i>t</i><sub class="lower-index">1</sub><i>t</i><sub class="lower-index">2</sub>... <i>t</i><sub class="lower-index">|<i>t</i>|</sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes the <span class="tex-span"><i>i</i></span>-th character of the string, and <span class="tex-span">|<i>t</i>|</span> denotes the length of the string.</p><p>Then <span class="tex-span"><i>t</i>[<i>i</i>... <i>j</i>]</span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>j</i> ≤ |<i>t</i>|)</span> represents the string <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub><i>t</i><sub class="lower-index"><i>i</i> + 1</sub>... <i>t</i><sub class="lower-index"><i>j</i></sub></span> (substring of <span class="tex-span"><i>t</i></span> from position <span class="tex-span"><i>i</i></span> to position <span class="tex-span"><i>j</i></span> inclusive).</p>
