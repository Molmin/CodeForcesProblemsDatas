## Description

<div><p>Now it's time of Olympiads. Vanya and Egor decided to make his own team to take part in a programming Olympiad. They've been best friends ever since primary school and hopefully, that can somehow help them in teamwork.</p><p>For each team Olympiad, Vanya takes his play cards with numbers. He takes only the cards containing numbers 1 and 0. The boys are very superstitious. They think that they can do well at the Olympiad if they begin with laying <span class="tex-font-style-bf">all</span> the cards in a row so that:</p><ul> <li> there wouldn't be a pair of any side-adjacent cards with zeroes in a row; </li><li> there wouldn't be a group of three consecutive cards containing numbers one. </li></ul><p>Today Vanya brought <span class="tex-span"><i>n</i></span> cards with zeroes and <span class="tex-span"><i>m</i></span> cards with numbers one. The number of cards was so much that the friends do not know how to put all those cards in the described way. Help them find the required arrangement of the cards or else tell the guys that it is impossible to arrange cards in such a way.</p></div><div class="input-specification"><p>The first line contains two integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of cards containing number 0; <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of cards containing number 1.</p></div><div class="output-specification"><p>In a single line print the required sequence of zeroes and ones without any spaces. If such sequence is impossible to obtain, print -1.</p></div>

## Input

<p>The first line contains two integers: <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of cards containing number 0; <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>) — the number of cards containing number 1.</p>

## Output

<p>In a single line print the required sequence of zeroes and ones without any spaces. If such sequence is impossible to obtain, print -1.</p>





```input1
1 2

```




```input2
4 8

```




```input3
4 10

```




```input4
1 5

```




```output1
101

```




```output2
110110110101

```




```output3
11011011011011

```




```output4
-1

```


