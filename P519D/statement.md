## Description

<div><p><span class="tex-font-style-it">A and B are preparing themselves for programming contests.</span></p><p>After several years of doing sports programming and solving many problems that require calculating all sorts of abstract objects, A and B also developed rather peculiar tastes.</p><p>A likes lowercase letters of the Latin alphabet. He has assigned to each letter a number that shows how much he likes that letter (he has assigned negative numbers to the letters he dislikes). </p><p>B likes substrings. He especially likes the ones that start and end with the same letter (their length must exceed one).</p><p>Also, A and B have a string <span class="tex-span"><i>s</i></span>. Now they are trying to find out how many substrings <span class="tex-span"><i>t</i></span> of a string <span class="tex-span"><i>s</i></span> are interesting to B (that is, <span class="tex-span"><i>t</i></span> starts and ends with the same letter and its length is larger than one), and also the sum of values of all letters (assigned by A), <span class="tex-font-style-it">except for the first and the last one</span> is equal to zero.</p><p>Naturally, A and B have quickly found the number of substrings <span class="tex-span"><i>t</i></span> that are interesting to them. Can you do it? </p></div><div class="input-specification"><p>The first line contains <span class="tex-span">26</span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i></sub>, <i>x</i><sub class="lower-index"><i>b</i></sub>, ..., <i>x</i><sub class="lower-index"><i>z</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — the value assigned to letters <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, ..., <i>z</i></span> respectively.</p><p>The second line contains string <span class="tex-span"><i>s</i></span> of length between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">5</sup></span> characters, consisting of Lating lowercase letters— the string for which you need to calculate the answer. </p></div><div class="output-specification"><p>Print the answer to the problem. </p></div>

## Input

<p>The first line contains <span class="tex-span">26</span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>a</i></sub>, <i>x</i><sub class="lower-index"><i>b</i></sub>, ..., <i>x</i><sub class="lower-index"><i>z</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">5</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — the value assigned to letters <span class="tex-span"><i>a</i>, <i>b</i>, <i>c</i>, ..., <i>z</i></span> respectively.</p><p>The second line contains string <span class="tex-span"><i>s</i></span> of length between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">5</sup></span> characters, consisting of Lating lowercase letters— the string for which you need to calculate the answer. </p>

## Output

<p>Print the answer to the problem. </p>





```input1
1 1 -1 1 1 1 1 1 1 1 1 1 1 1 1 7 1 1 1 8 1 1 1 1 1 1
xabcab

```




```input2
1 1 -1 1 1 1 1 1 1 1 1 1 1 1 1 7 1 1 1 8 1 1 1 1 1 1
aaa

```




```output1
2

```




```output2
2

```



## Note

<p>In the first sample test strings satisfying the condition above are <span class="tex-span"><i>abca</i></span> and <span class="tex-span"><i>bcab</i></span>.</p><p>In the second sample test strings satisfying the condition above are two occurences of <span class="tex-span"><i>aa</i></span>.</p>
