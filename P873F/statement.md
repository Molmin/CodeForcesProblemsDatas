## Description

<div><p>You are given a string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters. Some indices in this string are marked as <span class="tex-font-style-it">forbidden</span>.</p><p>You want to find a string <span class="tex-span"><i>a</i></span> such that the value of <span class="tex-span">|<i>a</i>|·<i>f</i>(<i>a</i>)</span> is maximum possible, where <span class="tex-span"><i>f</i>(<i>a</i>)</span> is the number of occurences of <span class="tex-span"><i>a</i></span> in <span class="tex-span"><i>s</i></span> such that these occurences end in non-forbidden indices. So, for example, if <span class="tex-span"><i>s</i></span> is <span class="tex-font-style-tt">aaaa</span>, <span class="tex-span"><i>a</i></span> is <span class="tex-font-style-tt">aa</span> and index <span class="tex-span">3</span> is forbidden, then <span class="tex-span"><i>f</i>(<i>a</i>) = 2</span> because there are three occurences of <span class="tex-span"><i>a</i></span> in <span class="tex-span"><i>s</i></span> (starting in indices <span class="tex-span">1</span>, <span class="tex-span">2</span> and <span class="tex-span">3</span>), but one of them (starting in index <span class="tex-span">2</span>) ends in a forbidden index.</p><p>Calculate the maximum possible value of <span class="tex-span">|<i>a</i>|·<i>f</i>(<i>a</i>)</span> you can get.</p></div><div class="input-specification"><p>The first line contains an integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the length of <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters.</p><p>The third line contains a string <span class="tex-span"><i>t</i></span>, consisting of <span class="tex-span"><i>n</i></span> characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. If <span class="tex-span"><i>i</i></span>-th character in <span class="tex-span"><i>t</i></span> is <span class="tex-font-style-tt">1</span>, then <span class="tex-span"><i>i</i></span> is a forbidden index (otherwise <span class="tex-span"><i>i</i></span> is not forbidden).</p></div><div class="output-specification"><p>Print the maximum possible value of <span class="tex-span">|<i>a</i>|·<i>f</i>(<i>a</i>)</span>.</p></div>

## Input

<p>The first line contains an integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>) — the length of <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span>, consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters.</p><p>The third line contains a string <span class="tex-span"><i>t</i></span>, consisting of <span class="tex-span"><i>n</i></span> characters <span class="tex-font-style-tt">0</span> and <span class="tex-font-style-tt">1</span>. If <span class="tex-span"><i>i</i></span>-th character in <span class="tex-span"><i>t</i></span> is <span class="tex-font-style-tt">1</span>, then <span class="tex-span"><i>i</i></span> is a forbidden index (otherwise <span class="tex-span"><i>i</i></span> is not forbidden).</p>

## Output

<p>Print the maximum possible value of <span class="tex-span">|<i>a</i>|·<i>f</i>(<i>a</i>)</span>.</p>





```input1
5
ababa
00100

```




```input2
5
ababa
00000

```




```input3
5
ababa
11111

```




```output1
5

```




```output2
6

```




```output3
0

```


