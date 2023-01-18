## Description

<div><p>Andrew and Eugene are playing a game. Initially, Andrew has string <span class="tex-span"><i>s</i></span>, consisting of digits. Eugene sends Andrew multiple queries of type "<span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> → <i>t</i><sub class="lower-index"><i>i</i></sub></span>", that means "replace all digits <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> in string <span class="tex-span"><i>s</i></span> with substrings equal to <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>". For example, if <span class="tex-span"><i>s</i> = 123123</span>, then query "<span class="tex-span">2 → 00</span>" transforms <span class="tex-span"><i>s</i></span> to <span class="tex-span">10031003</span>, and query "<span class="tex-span">3 → </span>" ("replace 3 by an empty string") transforms it to <span class="tex-span"><i>s</i> = 1212</span>. After all the queries Eugene asks Andrew to find the remainder after division of number with decimal representation equal to <span class="tex-span"><i>s</i></span> by <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>. When you represent <span class="tex-span"><i>s</i></span> as a decimal number, please ignore the leading zeroes; also if <span class="tex-span"><i>s</i></span> is an empty string, then it's assumed that the number equals to zero.</p><p>Andrew got tired of processing Eugene's requests manually and he asked you to write a program for that. Help him!</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>), consisting of digits&nbsp;— the string before processing all the requests.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the queries. The <span class="tex-span"><i>i</i></span>-th query is described by string "<span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span><span class="tex-font-style-tt">-&gt;</span><span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is exactly one digit (from 0 to 9), <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is a string consisting of digits (<span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> can be an empty string). The sum of lengths of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> for all queries doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The queries are written in the order in which they need to be performed.</p></div><div class="output-specification"><p>Print a single integer — remainder of division of the resulting number by <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>), consisting of digits&nbsp;— the string before processing all the requests.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of queries.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the descriptions of the queries. The <span class="tex-span"><i>i</i></span>-th query is described by string "<span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span><span class="tex-font-style-tt">-&gt;</span><span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is exactly one digit (from 0 to 9), <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is a string consisting of digits (<span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> can be an empty string). The sum of lengths of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> for all queries doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. The queries are written in the order in which they need to be performed.</p>

## Output

<p>Print a single integer — remainder of division of the resulting number by <span class="tex-span">1000000007&nbsp;(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
123123
1
2-&gt;00

```




```input2
123123
1
3-&gt;

```




```input3
222
2
2-&gt;0
0-&gt;7

```




```input4
1000000008
0

```




```output1
10031003

```




```output2
1212

```




```output3
777

```




```output4
1

```



## Note

<p>Note that the leading zeroes are not removed from string <span class="tex-span"><i>s</i></span> after the replacement (you can see it in the third sample).</p>
