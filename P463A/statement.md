## Description

<div><p>Caisa is going to have a party and he needs to buy the ingredients for a big chocolate cake. For that he is going to the biggest supermarket in town.</p><p>Unfortunately, he has just <span class="tex-span"><i>s</i></span> dollars for sugar. But that's not a reason to be sad, because there are <span class="tex-span"><i>n</i></span> types of sugar in the supermarket, maybe he able to buy one. But that's not all. The supermarket has very unusual exchange politics: instead of cents the sellers give sweets to a buyer as a change. Of course, the number of given sweets always doesn't exceed <span class="tex-span">99</span>, because each seller maximizes the number of dollars in the change (<span class="tex-span">100</span> cents can be replaced with a dollar).</p><p>Caisa wants to buy only one type of sugar, also he wants to maximize the number of sweets in the change. What is the maximum number of sweets he can get? Note, that Caisa doesn't want to minimize the cost of the sugar, he only wants to get maximum number of sweets as change. </p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>s</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>s</i> ≤ 100)</span>.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100;&nbsp;0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> &lt; 100)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> represents the number of dollars and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> the number of cents needed in order to buy the <span class="tex-span"><i>i</i></span>-th type of sugar.</p></div><div class="output-specification"><p>Print a single integer representing the maximum number of sweets he can buy, or <span class="tex-font-style-tt">-1</span> if he can't buy any type of sugar.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i>, <i>s</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>s</i> ≤ 100)</span>.</p><p>The <span class="tex-span"><i>i</i></span>-th of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 100;&nbsp;0 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> &lt; 100)</span>, where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> represents the number of dollars and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> the number of cents needed in order to buy the <span class="tex-span"><i>i</i></span>-th type of sugar.</p>

## Output

<p>Print a single integer representing the maximum number of sweets he can buy, or <span class="tex-font-style-tt">-1</span> if he can't buy any type of sugar.</p>





```input1
5 10
3 90
12 0
9 70
5 50
7 0

```




```input2
5 5
10 10
20 20
30 30
40 40
50 50

```




```output1
50

```




```output2
-1

```



## Note

<p>In the first test sample Caisa can buy the fourth type of sugar, in such a case he will take <span class="tex-span">50</span> sweets as a change.</p>
