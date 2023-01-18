## Description

<div><p><span class="tex-font-style-underline">Tavas is a strange creature. Usually "zzz" comes out of people's mouth while sleeping, but string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> comes out from Tavas' mouth instead.</span></p><center> <img class="tex-graphics" src="file://WVsUC0AL.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Today Tavas fell asleep in Malekas' place. While he was sleeping, Malekas did a little process on <span class="tex-span"><i>s</i></span>. Malekas has a favorite string <span class="tex-span"><i>p</i></span>. He determined all positions <span class="tex-span"><i>x</i><sub class="lower-index">1</sub> &lt; <i>x</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>x</i><sub class="lower-index"><i>k</i></sub></span> where <span class="tex-span"><i>p</i></span> matches <span class="tex-span"><i>s</i></span>. More formally, for each <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>k</i></span>) he condition <span class="tex-span"><i>s</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>i</i></sub></sub><i>s</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>i</i></sub> + 1</sub>... <i>s</i><sub class="lower-index"><i>x</i><sub class="lower-index"><i>i</i></sub> + |<i>p</i>| - 1</sub> = <i>p</i></span> is fullfilled.</p><p>Then Malekas wrote down one of subsequences of <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ... <i>x</i><sub class="lower-index"><i>k</i></sub></span> (possibly, he didn't write anything) on a piece of paper. Here a sequence <span class="tex-span"><i>b</i></span> is a subsequence of sequence <span class="tex-span"><i>a</i></span> if and only if we can turn <span class="tex-span"><i>a</i></span> into <span class="tex-span"><i>b</i></span> by removing some of its elements (maybe no one of them or all).</p><p>After Tavas woke up, Malekas told him everything. He couldn't remember string <span class="tex-span"><i>s</i></span>, but he knew that both <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>s</i></span> only contains lowercase English letters and also he had the subsequence he had written on that piece of paper.</p><p>Tavas wonders, what is the number of possible values of <span class="tex-span"><i>s</i></span>? He asked SaDDas, but he wasn't smart enough to solve this. So, Tavas asked you to calculate this number for him.</p><p>Answer can be very large, so Tavas wants you to print the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, the length of <span class="tex-span"><i>s</i></span> and the length of the subsequence Malekas wrote down (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span> and <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i> - |<i>p</i>| + 1</span>).</p><p>The second line contains string <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ |<i>p</i>| ≤ <i>n</i></span>).</p><p>The next line contains <span class="tex-span"><i>m</i></span> space separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>m</i></sub></span>, Malekas' subsequence (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>y</i><sub class="lower-index"><i>m</i></sub> ≤ <i>n</i> - |<i>p</i>| + 1</span>).</p></div><div class="output-specification"><p>In a single line print the answer modulo <span class="tex-span">1000 000 007</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, the length of <span class="tex-span"><i>s</i></span> and the length of the subsequence Malekas wrote down (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span> and <span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i> - |<i>p</i>| + 1</span>).</p><p>The second line contains string <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ |<i>p</i>| ≤ <i>n</i></span>).</p><p>The next line contains <span class="tex-span"><i>m</i></span> space separated integers <span class="tex-span"><i>y</i><sub class="lower-index">1</sub>, <i>y</i><sub class="lower-index">2</sub>, ..., <i>y</i><sub class="lower-index"><i>m</i></sub></span>, Malekas' subsequence (<span class="tex-span">1 ≤ <i>y</i><sub class="lower-index">1</sub> &lt; <i>y</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>y</i><sub class="lower-index"><i>m</i></sub> ≤ <i>n</i> - |<i>p</i>| + 1</span>).</p>

## Output

<p>In a single line print the answer modulo <span class="tex-span">1000 000 007</span>.</p>





```input1
6 2
ioi
1 3

```




```input2
5 2
ioi
1 2

```




```output1
26

```




```output2
0

```



## Note

<p>In the first sample test all strings of form <span class="tex-font-style-tt">"ioioi?"</span> where the question mark replaces arbitrary English letter satisfy.</p><p>Here <span class="tex-span">|<i>x</i>|</span> denotes the length of string x.</p><p>Please note that it's possible that there is no such string (answer is 0).</p>
