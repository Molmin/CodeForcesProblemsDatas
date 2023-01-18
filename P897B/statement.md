## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"> — Thanks a lot for today.<p>— I experienced so many great things.</p><p>— You gave me memories like dreams... But I have to leave now...</p><p>— One last request, can you...</p><p>— Help me solve a Codeforces problem?</p><p>— ......</p><p>— What?</p></span></div></div><p>Chtholly has been thinking about a problem for days:</p><p>If a number is <span class="tex-font-style-it">palindrome</span> and length of its decimal representation without leading zeros is even, we call it a zcy number. A number is <span class="tex-font-style-it">palindrome</span> means when written in decimal representation, it contains no leading zeros and reads the same forwards and backwards. For example <span class="tex-font-style-tt">12321</span> and <span class="tex-font-style-tt">1221</span> are palindromes and <span class="tex-font-style-tt">123</span> and <span class="tex-font-style-tt">12451</span> are not. Moreover, <span class="tex-font-style-tt">1221</span> is zcy number and <span class="tex-font-style-tt">12321</span> is not.</p><p>Given integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span>, calculate the sum of the <span class="tex-span"><i>k</i></span> smallest zcy numbers and output this sum modulo <span class="tex-span"><i>p</i></span>.</p><p>Unfortunately, Willem isn't good at solving this kind of problems, so he asks you for help!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Output single integer&nbsp;— answer to the problem.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Output single integer&nbsp;— answer to the problem.</p>





```input1
2 100

```




```input2
5 30

```




```output1
33

```




```output2
15

```



## Note

<p>In the first example, the smallest zcy number is <span class="tex-span">11</span>, and the second smallest zcy number is <span class="tex-span">22</span>.</p><p>In the second example, <img align="middle" class="tex-formula" src="file://Lf0DojcA.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
