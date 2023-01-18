## Description

<div><p>Vasya has <span class="tex-span"><i>n</i></span> burles. One bottle of Ber-Cola costs <span class="tex-span"><i>a</i></span> burles and one Bars bar costs <span class="tex-span"><i>b</i></span> burles. He can buy any non-negative integer number of bottles of Ber-Cola and any non-negative integer number of Bars bars.</p><p>Find out if it's possible to buy some amount of bottles of Ber-Cola and Bars bars and spend <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>n</i></span> burles.</p><p>In other words, you should find two non-negative integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> such that Vasya can buy <span class="tex-span"><i>x</i></span> bottles of Ber-Cola and <span class="tex-span"><i>y</i></span> Bars bars and <span class="tex-span"><i>x</i>·<i>a</i> + <i>y</i>·<i>b</i> = <i>n</i></span> or tell that it's impossible.</p></div><div class="input-specification"><p>First line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000 000</span>)&nbsp;— amount of money, that Vasya has.</p><p>Second line contains single integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 10 000 000</span>)&nbsp;— cost of one bottle of Ber-Cola.</p><p>Third line contains single integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ 10 000 000</span>)&nbsp;— cost of one Bars bar.</p></div><div class="output-specification"><p>If Vasya can't buy Bars and Ber-Cola in such a way to spend exactly <span class="tex-span"><i>n</i></span> burles print «<span class="tex-font-style-tt">NO</span>» (without quotes).</p><p>Otherwise in first line print «<span class="tex-font-style-tt">YES</span>» (without quotes). In second line print two non-negative integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>&nbsp;— number of bottles of Ber-Cola and number of Bars bars Vasya should buy in order to spend exactly <span class="tex-span"><i>n</i></span> burles, i.e. <span class="tex-span"><i>x</i>·<i>a</i> + <i>y</i>·<i>b</i> = <i>n</i></span>. If there are multiple answers print any of them.</p><p>Any of numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> can be equal <span class="tex-span">0</span>.</p></div>

## Input

<p>First line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000 000</span>)&nbsp;— amount of money, that Vasya has.</p><p>Second line contains single integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 10 000 000</span>)&nbsp;— cost of one bottle of Ber-Cola.</p><p>Third line contains single integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ 10 000 000</span>)&nbsp;— cost of one Bars bar.</p>

## Output

<p>If Vasya can't buy Bars and Ber-Cola in such a way to spend exactly <span class="tex-span"><i>n</i></span> burles print «<span class="tex-font-style-tt">NO</span>» (without quotes).</p><p>Otherwise in first line print «<span class="tex-font-style-tt">YES</span>» (without quotes). In second line print two non-negative integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>&nbsp;— number of bottles of Ber-Cola and number of Bars bars Vasya should buy in order to spend exactly <span class="tex-span"><i>n</i></span> burles, i.e. <span class="tex-span"><i>x</i>·<i>a</i> + <i>y</i>·<i>b</i> = <i>n</i></span>. If there are multiple answers print any of them.</p><p>Any of numbers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> can be equal <span class="tex-span">0</span>.</p>





```input1
7
2
3

```




```input2
100
25
10

```




```input3
15
4
8

```




```input4
9960594
2551
2557

```




```output1
YES
2 1

```




```output2
YES
0 10

```




```output3
NO

```




```output4
YES
1951 1949

```



## Note

<p>In first example Vasya can buy two bottles of Ber-Cola and one Bars bar. He will spend exactly <span class="tex-span">2·2 + 1·3 = 7</span> burles.</p><p>In second example Vasya can spend exactly <span class="tex-span"><i>n</i></span> burles multiple ways: </p><ul> <li> buy two bottles of Ber-Cola and five Bars bars; </li><li> buy four bottles of Ber-Cola and don't buy Bars bars; </li><li> don't buy Ber-Cola and buy <span class="tex-span">10</span> Bars bars. </li></ul><p>In third example it's impossible to but Ber-Cola and Bars bars in order to spend exactly <span class="tex-span"><i>n</i></span> burles.</p>
