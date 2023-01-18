## Description

<div><p>Eugeny has <span class="tex-span"><i>n</i></span> cards, each of them has exactly one integer written on it. Eugeny wants to exchange some cards with Nikolay so that the number of even integers on his cards would equal the number of odd integers, and that all these numbers would be <span class="tex-font-style-bf">distinct</span>. </p><p>Nikolay has <span class="tex-span"><i>m</i></span> cards, distinct numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> are written on them, one per card. It means that Nikolay has exactly one card with number <span class="tex-span">1</span>, exactly one card with number <span class="tex-span">2</span> and so on. </p><p>A single exchange is a process in which Eugeny gives one card to Nikolay and takes another one from those Nikolay has. Your task is to find the minimum number of card exchanges and determine which cards Eugeny should exchange.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of cards Eugeny has and the number of cards Nikolay has. It is guaranteed that <span class="tex-span"><i>n</i></span> is even.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the numbers on Eugeny's cards.</p></div><div class="output-specification"><p>If there is no answer, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, in the first line print the minimum number of exchanges. In the second line print <span class="tex-span"><i>n</i></span> integers&nbsp;— Eugeny's cards after all the exchanges with Nikolay. The order of cards should coincide with the card's order in the input data. If the <span class="tex-span"><i>i</i></span>-th card wasn't exchanged then the <span class="tex-span"><i>i</i></span>-th number should coincide with the number from the input data. Otherwise, it is considered that this card was exchanged, and the <span class="tex-span"><i>i</i></span>-th number should be equal to the number on the card it was exchanged to.</p><p>If there are multiple answers, it is allowed to print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of cards Eugeny has and the number of cards Nikolay has. It is guaranteed that <span class="tex-span"><i>n</i></span> is even.</p><p>The second line contains a sequence of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the numbers on Eugeny's cards.</p>

## Output

<p>If there is no answer, print <span class="tex-font-style-tt">-1</span>.</p><p>Otherwise, in the first line print the minimum number of exchanges. In the second line print <span class="tex-span"><i>n</i></span> integers&nbsp;— Eugeny's cards after all the exchanges with Nikolay. The order of cards should coincide with the card's order in the input data. If the <span class="tex-span"><i>i</i></span>-th card wasn't exchanged then the <span class="tex-span"><i>i</i></span>-th number should coincide with the number from the input data. Otherwise, it is considered that this card was exchanged, and the <span class="tex-span"><i>i</i></span>-th number should be equal to the number on the card it was exchanged to.</p><p>If there are multiple answers, it is allowed to print any of them.</p>





```input1
6 2
5 6 7 9 4 5

```




```input2
8 6
7 7 7 7 8 8 8 8

```




```input3
4 1
4 2 1 10

```




```output1
1
5 6 7 9 4 2 

```




```output2
6
7 2 4 6 8 1 3 5 

```




```output3
-1

```


