## Description

<div><p>Misha and Vasya participated in a Codeforces contest. Unfortunately, each of them solved only one problem, though successfully submitted it at the first attempt. Misha solved the problem that costs <span class="tex-span"><i>a</i></span> points and Vasya solved the problem that costs <span class="tex-span"><i>b</i></span> points. Besides, Misha submitted the problem <span class="tex-span"><i>c</i></span> minutes after the contest started and Vasya submitted the problem <span class="tex-span"><i>d</i></span> minutes after the contest started. As you know, on Codeforces the cost of a problem reduces as a round continues. That is, if you submit a problem that costs <span class="tex-span"><i>p</i></span> points <span class="tex-span"><i>t</i></span> minutes after the contest started, you get <img align="middle" class="tex-formula" src="file://vwD31Nz9.png" style="max-width: 100.0%;max-height: 100.0%;"> points. </p><p>Misha and Vasya are having an argument trying to find out who got more points. Help them to find out the truth.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">250 ≤ <i>a</i>, <i>b</i> ≤ 3500</span>, <span class="tex-span">0 ≤ <i>c</i>, <i>d</i> ≤ 180</span>). </p><p>It is guaranteed that numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are divisible by <span class="tex-span">250</span> (just like on any real Codeforces round).</p></div><div class="output-specification"><p>Output on a single line: </p><p>"<span class="tex-font-style-tt">Misha</span>" (without the quotes), if Misha got more points than Vasya.</p><p>"<span class="tex-font-style-tt">Vasya</span>" (without the quotes), if Vasya got more points than Misha.</p><p>"<span class="tex-font-style-tt">Tie</span>" (without the quotes), if both of them got the same number of points.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">250 ≤ <i>a</i>, <i>b</i> ≤ 3500</span>, <span class="tex-span">0 ≤ <i>c</i>, <i>d</i> ≤ 180</span>). </p><p>It is guaranteed that numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are divisible by <span class="tex-span">250</span> (just like on any real Codeforces round).</p>

## Output

<p>Output on a single line: </p><p>"<span class="tex-font-style-tt">Misha</span>" (without the quotes), if Misha got more points than Vasya.</p><p>"<span class="tex-font-style-tt">Vasya</span>" (without the quotes), if Vasya got more points than Misha.</p><p>"<span class="tex-font-style-tt">Tie</span>" (without the quotes), if both of them got the same number of points.</p>





```input1
500 1000 20 30

```




```input2
1000 1000 1 1

```




```input3
1500 1000 176 177

```




```output1
Vasya

```




```output2
Tie

```




```output3
Misha

```


