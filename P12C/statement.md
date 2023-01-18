## Description

<div><p>The spring is coming and it means that a lot of fruits appear on the counters. One sunny day little boy Valera decided to go shopping. He made a list of <span class="tex-span"><i>m</i></span> fruits he wanted to buy. If Valera want to buy more than one fruit of some kind, he includes it into the list several times. </p><p>When he came to the fruit stall of Ashot, he saw that the seller hadn't distributed price tags to the goods, but put all price tags on the counter. Later Ashot will attach every price tag to some kind of fruits, and Valera will be able to count the total price of all fruits from his list. But Valera wants to know now what can be the smallest total price (in case of the most «lucky» for him distribution of price tags) and the largest total price (in case of the most «unlucky» for him distribution of price tags).</p></div><div class="input-specification"><p>The first line of the input contains two integer number <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of price tags (which is equal to the number of different kinds of fruits that Ashot sells) and the number of items in Valera's list. The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integer numbers. Each of them doesn't exceed <span class="tex-span">100</span> and stands for the price of one fruit of some kind. The following <span class="tex-span"><i>m</i></span> lines contain names of the fruits from the list. Each name is a non-empty string of small Latin letters which length doesn't exceed 32. It is guaranteed that the number of distinct fruits from the list is less of equal to <span class="tex-span"><i>n</i></span>. Also it is known that the seller has in stock all fruits that Valera wants to buy.</p></div><div class="output-specification"><p>Print two numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> ≤ <i>b</i></span>) — the minimum and the maximum possible sum which Valera may need to buy all fruits from his list.</p></div>

## Input

<p>The first line of the input contains two integer number <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of price tags (which is equal to the number of different kinds of fruits that Ashot sells) and the number of items in Valera's list. The second line contains <span class="tex-span"><i>n</i></span> space-separated positive integer numbers. Each of them doesn't exceed <span class="tex-span">100</span> and stands for the price of one fruit of some kind. The following <span class="tex-span"><i>m</i></span> lines contain names of the fruits from the list. Each name is a non-empty string of small Latin letters which length doesn't exceed 32. It is guaranteed that the number of distinct fruits from the list is less of equal to <span class="tex-span"><i>n</i></span>. Also it is known that the seller has in stock all fruits that Valera wants to buy.</p>

## Output

<p>Print two numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span"><i>a</i> ≤ <i>b</i></span>) — the minimum and the maximum possible sum which Valera may need to buy all fruits from his list.</p>





```input1
5 3
4 2 1 10 5
apple
orange
mango

```




```input2
6 5
3 5 1 6 8 1
peach
grapefruit
banana
orange
orange

```




```output1
7 19

```




```output2
11 30

```


