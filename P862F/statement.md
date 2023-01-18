## Description

<div><p>Mahmoud and Ehab solved Dr. Evil's questions so he gave them the password of the door of the evil land. When they tried to open the door using it, the door gave them a final question to solve before they leave (yes, the door is digital, Dr. Evil is modern). If they don't solve it, all the work will be useless and they won't leave the evil land forever. Will you help them?</p><p>Mahmoud and Ehab are given <span class="tex-span"><i>n</i></span> strings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ... , <i>s</i><sub class="lower-index"><i>n</i></sub></span> numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> queries, Each query has one of the following forms:</p><ul> <li> <span class="tex-span">1</span> <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span> <span class="tex-span">(1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>n</i>)</span>, For all the intervals <span class="tex-span">[<i>l</i>;<i>r</i>]</span> where <span class="tex-span">(<i>a</i> ≤ <i>l</i> ≤ <i>r</i> ≤ <i>b</i>)</span> find the maximum value of this expression:<p><span class="tex-span">(<i>r</i> - <i>l</i> + 1) * <i>LCP</i>(<i>s</i><sub class="lower-index"><i>l</i></sub>, <i>s</i><sub class="lower-index"><i>l</i> + 1</sub>, ... , <i>s</i><sub class="lower-index"><i>r</i> - 1</sub>, <i>s</i><sub class="lower-index"><i>r</i></sub>)</span> where <span class="tex-span"><i>LCP</i>(<i>str</i><sub class="lower-index">1</sub>, <i>str</i><sub class="lower-index">2</sub>, <i>str</i><sub class="lower-index">3</sub>, ... )</span> is the length of the longest common prefix of the strings <span class="tex-span"><i>str</i><sub class="lower-index">1</sub>, <i>str</i><sub class="lower-index">2</sub>, <i>str</i><sub class="lower-index">3</sub>, ... </span>.</p></li><li> <span class="tex-span">2</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>)</span> where <span class="tex-span"><i>y</i></span> is a string, consisting of lowercase English letters. Change the string at position <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span>.</li></ul></div><div class="input-specification"><p>The first line of input contains 2 integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>&nbsp;– The number of strings and the number of queries, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> strings <span class="tex-span"><i>str</i><sub class="lower-index"><i>i</i></sub></span> consisting of lowercase English letters.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the queries and may have one of the 2 forms:</p><ul> <li> <span class="tex-span">1</span> <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>n</i></span>).</li><li> <span class="tex-span">2</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>), where <span class="tex-span"><i>y</i></span> is a string consisting of lowercase English letters.</li></ul><p><span class="tex-font-style-bf">the total length of all strings in input won't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span></span></p></div><div class="output-specification"><p>For each query of first type output its answer in a new line.</p></div>

## Input

<p>The first line of input contains 2 integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>&nbsp;– The number of strings and the number of queries, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> strings <span class="tex-span"><i>str</i><sub class="lower-index"><i>i</i></sub></span> consisting of lowercase English letters.</p><p>The next <span class="tex-span"><i>q</i></span> lines describe the queries and may have one of the 2 forms:</p><ul> <li> <span class="tex-span">1</span> <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ <i>n</i></span>).</li><li> <span class="tex-span">2</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>), where <span class="tex-span"><i>y</i></span> is a string consisting of lowercase English letters.</li></ul><p><span class="tex-font-style-bf">the total length of all strings in input won't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span></span></p>

## Output

<p>For each query of first type output its answer in a new line.</p>





```input1
5 9
mahmoud mahmoudbadawy drmahmoud drevil mahmoud
1 1 5
1 1 2
1 2 3
2 3 mahmoud
2 4 mahmoud
2 2 mahmouu
1 1 5
1 2 3
1 1 1

```




```output1
14
14
13
30
12
7

```


