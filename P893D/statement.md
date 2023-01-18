## Description

<div><p>Recenlty Luba got a credit card and started to use it. Let's consider <span class="tex-span"><i>n</i></span> consecutive days Luba uses the card.</p><p><span class="tex-font-style-bf">She starts with <span class="tex-span">0</span> money on her account.</span></p><p>In the <span class="tex-font-style-bf">evening</span> of <span class="tex-span"><i>i</i></span>-th day a transaction <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> occurs. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; 0</span>, then <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> bourles are deposited to Luba's account. If <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 0</span>, then <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> bourles are withdrawn. And if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span>, then the amount of money on Luba's account is checked.</p><p>In the <span class="tex-font-style-bf">morning</span> of any of <span class="tex-span"><i>n</i></span> days Luba can go to the bank and deposit any <span class="tex-font-style-bf">positive</span> integer amount of burles to her account. But there is a limitation: the amount of money on the account can never exceed <span class="tex-span"><i>d</i></span>.</p><p><span class="tex-font-style-bf">It can happen that the amount of money goes greater than <span class="tex-span"><i>d</i></span> by some transaction in the evening. In this case answer will be «-1».</span></p><p>Luba must not exceed this limit, and also she wants that <span class="tex-font-style-bf">every day her account is checked</span> (the days when <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span>) the amount of money on her account is non-negative. It takes a lot of time to go to the bank, so Luba wants to know the minimum number of days she needs to deposit some money to her account (if it is possible to meet all the requirements). Help her!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>) —the number of days and the money limitation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the transaction in <span class="tex-span"><i>i</i></span>-th day.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">-1</span> if Luba cannot deposit the money to her account in such a way that the requirements are met. Otherwise print the minimum number of days Luba has to deposit money.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">9</sup></span>) —the number of days and the money limitation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> represents the transaction in <span class="tex-span"><i>i</i></span>-th day.</p>

## Output

<p>Print <span class="tex-font-style-tt">-1</span> if Luba cannot deposit the money to her account in such a way that the requirements are met. Otherwise print the minimum number of days Luba has to deposit money.</p>





```input1
5 10
-1 5 0 -5 3

```




```input2
3 4
-10 0 20

```




```input3
5 10
-5 0 10 -11 0

```




```output1
0

```




```output2
-1

```




```output3
2

```


