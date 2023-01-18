## Description

<div><p>Pari wants to buy an expensive chocolate from Arya. She has <span class="tex-span"><i>n</i></span> coins, the value of the <span class="tex-span"><i>i</i></span>-th coin is <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. The price of the chocolate is <span class="tex-span"><i>k</i></span>, so Pari will take a subset of her coins with sum equal to <span class="tex-span"><i>k</i></span> and give it to Arya.</p><p>Looking at her coins, a question came to her mind: after giving the coins to Arya, what values does Arya can make with them? She is jealous and she doesn't want Arya to make a lot of values. So she wants to know all the values <span class="tex-span"><i>x</i></span>, such that Arya will be able to make <span class="tex-span"><i>x</i></span> using some subset of coins with the sum <span class="tex-span"><i>k</i></span>.</p><p>Formally, Pari wants to know the values <span class="tex-span"><i>x</i></span> such that there exists a subset of coins with the sum <span class="tex-span"><i>k</i></span> such that some subset of this subset has the sum <span class="tex-span"><i>x</i></span>, i.e. there is exists some way to pay for the chocolate, such that Arya will be able to make the sum <span class="tex-span"><i>x</i></span> using these coins.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1  ≤  <i>n</i>, <i>k</i>  ≤  500</span>)&nbsp;— the number of coins and the price of the chocolate, respectively.</p><p>Next line will contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>)&nbsp;— the values of Pari's coins.</p><p>It's guaranteed that one can make value <span class="tex-span"><i>k</i></span> using these coins.</p></div><div class="output-specification"><p>First line of the output must contain a single integer <span class="tex-span"><i>q</i></span>— the number of suitable values <span class="tex-span"><i>x</i></span>. Then print <span class="tex-span"><i>q</i></span> integers in ascending order&nbsp;— the values that Arya can make for some subset of coins of Pari that pays for the chocolate.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1  ≤  <i>n</i>, <i>k</i>  ≤  500</span>)&nbsp;— the number of coins and the price of the chocolate, respectively.</p><p>Next line will contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 500</span>)&nbsp;— the values of Pari's coins.</p><p>It's guaranteed that one can make value <span class="tex-span"><i>k</i></span> using these coins.</p>

## Output

<p>First line of the output must contain a single integer <span class="tex-span"><i>q</i></span>— the number of suitable values <span class="tex-span"><i>x</i></span>. Then print <span class="tex-span"><i>q</i></span> integers in ascending order&nbsp;— the values that Arya can make for some subset of coins of Pari that pays for the chocolate.</p>





```input1
6 18
5 6 1 10 12 2

```




```input2
3 50
25 25 50

```




```output1
16
0 1 2 3 5 6 7 8 10 11 12 13 15 16 17 18 

```




```output2
3
0 25 50 

```


