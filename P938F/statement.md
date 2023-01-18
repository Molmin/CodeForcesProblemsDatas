## Description

<div><p>You are given a string <span class="tex-span"><i>s</i></span>, initially consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters. After that, you perform <span class="tex-span"><i>k</i></span> operations with it, where <img align="middle" class="tex-formula" src="file://NcMqfS88.png" style="max-width: 100.0%;max-height: 100.0%;">. During <span class="tex-span"><i>i</i></span>-th operation you <span class="tex-font-style-bf">must</span> erase some substring of length exactly <span class="tex-span">2<sup class="upper-index"><i>i</i> - 1</sup></span> from <span class="tex-span"><i>s</i></span>.</p><p>Print the lexicographically minimal string you may obtain after performing <span class="tex-span"><i>k</i></span> such operations.</p></div><div class="input-specification"><p>The only line contains one string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>).</p></div><div class="output-specification"><p>Print the lexicographically minimal string you may obtain after performing <span class="tex-span"><i>k</i></span> operations.</p></div>

## Input

<p>The only line contains one string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase Latin letters (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>).</p>

## Output

<p>Print the lexicographically minimal string you may obtain after performing <span class="tex-span"><i>k</i></span> operations.</p>





```input1
adcbca

```




```input2
abacabadabacaba

```




```output1
aba

```




```output2
aabacaba

```



## Note

<p>Possible operations in examples:</p><ol> <li> adcb<span class="tex-font-style-bf">c</span>a <img align="middle" class="tex-formula" src="file://UxTgvrPT.png" style="max-width: 100.0%;max-height: 100.0%;"> a<span class="tex-font-style-bf">dc</span>ba <img align="middle" class="tex-formula" src="file://9SyO4brA.png" style="max-width: 100.0%;max-height: 100.0%;"> aba; </li><li> ab<span class="tex-font-style-bf">a</span>cabadabacaba <img align="middle" class="tex-formula" src="file://74DLB60V.png" style="max-width: 100.0%;max-height: 100.0%;"> a<span class="tex-font-style-bf">bc</span>abadabacaba <img align="middle" class="tex-formula" src="file://5TMmwBJ7.png" style="max-width: 100.0%;max-height: 100.0%;"> aaba<span class="tex-font-style-bf">daba</span>caba <img align="middle" class="tex-formula" src="file://S4Yum2tR.png" style="max-width: 100.0%;max-height: 100.0%;"> aabacaba. </li></ol>
