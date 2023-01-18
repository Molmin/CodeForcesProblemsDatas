## Description

<div><p>Appleman has <span class="tex-span"><i>n</i></span> cards. Each card has an uppercase letter written on it. Toastman must choose <span class="tex-span"><i>k</i></span> cards from Appleman's cards. Then Appleman should give Toastman some coins depending on the chosen cards. Formally, for each Toastman's card <span class="tex-span"><i>i</i></span> you should calculate how much Toastman's cards have the letter equal to letter on <span class="tex-span"><i>i</i></span>th, then sum up all these quantities, such a number of coins Appleman should give to Toastman.</p><p>Given the description of Appleman's cards. What is the maximum number of coins Toastman can get?</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> uppercase letters without spaces — the <span class="tex-span"><i>i</i></span>-th letter describes the <span class="tex-span"><i>i</i></span>-th card of the Appleman.</p></div><div class="output-specification"><p>Print a single integer – the answer to the problem.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> uppercase letters without spaces — the <span class="tex-span"><i>i</i></span>-th letter describes the <span class="tex-span"><i>i</i></span>-th card of the Appleman.</p>

## Output

<p>Print a single integer – the answer to the problem.</p>





```input1
15 10
DZFDFZDFDDDDDDF

```




```input2
6 4
YJSNPI

```




```output1
82

```




```output2
4

```



## Note

<p>In the first test example Toastman can choose nine cards with letter <span class="tex-font-style-tt">D</span> and one additional card with any letter. For each card with <span class="tex-font-style-tt">D</span> he will get 9 coins and for the additional card he will get 1 coin.</p>
