## Description

<div><p>A string <span class="tex-span"><i>t</i></span> is called <span class="tex-font-style-it">nice</span> if a string "<span class="tex-font-style-tt">2017</span>" occurs in <span class="tex-span"><i>t</i></span> as a <span class="tex-font-style-bf">subsequence</span> but a string "<span class="tex-font-style-tt">2016</span>" doesn't occur in <span class="tex-span"><i>t</i></span> as a <span class="tex-font-style-bf">subsequence</span>. For example, strings "<span class="tex-font-style-tt">203434107</span>" and "<span class="tex-font-style-tt">9220617</span>" are nice, while strings "<span class="tex-font-style-tt">20016</span>", "<span class="tex-font-style-tt">1234</span>" and "<span class="tex-font-style-tt">20167</span>" aren't nice.</p><p>The <span class="tex-font-style-it">ugliness</span> of a string is the minimum possible number of characters to remove, in order to obtain a nice string. If it's impossible to make a string nice by removing characters, its ugliness is <span class="tex-span"> - 1</span>.</p><p>Limak has a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, with characters indexed <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. He asks you <span class="tex-span"><i>q</i></span> queries. In the <span class="tex-span"><i>i</i></span>-th query you should compute and print the ugliness of a <span class="tex-font-style-bf">substring</span> (continuous subsequence) of <span class="tex-span"><i>s</i></span> starting at the index <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and ending at the index <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (inclusive).</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the length of the string <span class="tex-span"><i>s</i></span> and the number of queries respectively.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. Every character is one of digits '<span class="tex-font-style-tt">0</span>'–'<span class="tex-font-style-tt">9</span>'.</p><p>The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), describing a substring in the <span class="tex-span"><i>i</i></span>-th query.</p></div><div class="output-specification"><p>For each query print the ugliness of the given substring.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the length of the string <span class="tex-span"><i>s</i></span> and the number of queries respectively.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>. Every character is one of digits '<span class="tex-font-style-tt">0</span>'–'<span class="tex-font-style-tt">9</span>'.</p><p>The <span class="tex-span"><i>i</i></span>-th of next <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), describing a substring in the <span class="tex-span"><i>i</i></span>-th query.</p>

## Output

<p>For each query print the ugliness of the given substring.</p>





```input1
8 3
20166766
1 8
1 7
2 8

```




```input2
15 5
012016662091670
3 4
1 14
4 15
1 13
10 15

```




```input3
4 2
1234
2 4
1 2

```




```output1
4
3
-1

```




```output2
-1
2
1
-1
-1

```




```output3
-1
-1

```



## Note

<p>In the first sample:</p><ul> <li> In the first query, <span class="tex-span"><i>ugliness</i>(</span>"<span class="tex-font-style-tt">20166766</span>"<span class="tex-span">) = 4</span> because all four sixes must be removed. </li><li> In the second query, <span class="tex-span"><i>ugliness</i>(</span>"<span class="tex-font-style-tt">2016676</span>"<span class="tex-span">) = 3</span> because all three sixes must be removed. </li><li> In the third query, <span class="tex-span"><i>ugliness</i>(</span>"<span class="tex-font-style-tt">0166766</span>"<span class="tex-span">) =  - 1</span> because it's impossible to remove some digits to get a nice string. </li></ul><p>In the second sample:</p><ul> <li> In the second query, <span class="tex-span"><i>ugliness</i>(</span>"<span class="tex-font-style-tt">01201666209167</span>"<span class="tex-span">) = 2</span>. It's optimal to remove the first digit '<span class="tex-font-style-tt">2</span>' and the last digit '<span class="tex-font-style-tt">6</span>', what gives a string "<span class="tex-font-style-tt">010166620917</span>", which is nice. </li><li> In the third query, <span class="tex-span"><i>ugliness</i>(</span>"<span class="tex-font-style-tt">016662091670</span>"<span class="tex-span">) = 1</span>. It's optimal to remove the last digit '<span class="tex-font-style-tt">6</span>', what gives a nice string "<span class="tex-font-style-tt">01666209170</span>". </li></ul>
