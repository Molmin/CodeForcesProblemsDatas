## Description

<div><p>This winter is so cold in Nvodsk! A group of <span class="tex-span"><i>n</i></span> friends decided to buy <span class="tex-span"><i>k</i></span> bottles of a soft drink called "Take-It-Light" to warm up a bit. Each bottle has <span class="tex-span"><i>l</i></span> milliliters of the drink. Also they bought <span class="tex-span"><i>c</i></span> limes and cut each of them into <span class="tex-span"><i>d</i></span> slices. After that they found <span class="tex-span"><i>p</i></span> grams of salt.</p><p>To make a toast, each friend needs <span class="tex-span"><i>nl</i></span> milliliters of the drink, a slice of lime and <span class="tex-span"><i>np</i></span> grams of salt. The friends want to make as many toasts as they can, provided they all drink the same amount. How many toasts can each friend make?</p></div><div class="input-specification"><p>The first and only line contains <span class="tex-font-style-bf">positive</span> integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>nl</i></span>, <span class="tex-span"><i>np</i></span>, not exceeding <span class="tex-span">1000</span> and no less than <span class="tex-span">1</span>. The numbers are separated by exactly one space.</p></div><div class="output-specification"><p>Print a single integer — the number of toasts each friend can make.</p></div>

## Input

<p>The first and only line contains <span class="tex-font-style-bf">positive</span> integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>c</i></span>, <span class="tex-span"><i>d</i></span>, <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>nl</i></span>, <span class="tex-span"><i>np</i></span>, not exceeding <span class="tex-span">1000</span> and no less than <span class="tex-span">1</span>. The numbers are separated by exactly one space.</p>

## Output

<p>Print a single integer — the number of toasts each friend can make.</p>





```input1
3 4 5 10 8 100 3 1

```




```input2
5 100 10 1 19 90 4 3

```




```input3
10 1000 1000 25 23 1 50 1

```




```output1
2

```




```output2
3

```




```output3
0

```



## Note

<p>A comment to the first sample: </p><p>Overall the friends have <span class="tex-span">4 * 5 = 20</span> milliliters of the drink, it is enough to make <span class="tex-span">20 / 3 = 6</span> toasts. The limes are enough for <span class="tex-span">10 * 8 = 80</span> toasts and the salt is enough for <span class="tex-span">100 / 1 = 100</span> toasts. However, there are 3 friends in the group, so the answer is <span class="tex-span"><i>min</i>(6, 80, 100) / 3 = 2</span>.</p>
