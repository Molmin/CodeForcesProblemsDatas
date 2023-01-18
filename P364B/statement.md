## Description

<div><p>John Doe has recently found a "Free Market" in his city — that is the place where you can exchange some of your possessions for other things for free. </p><p>John knows that his city has <span class="tex-span"><i>n</i></span> items in total (each item is unique). You can bring any number of items to the market and exchange them for any other one. Note that each item is one of a kind and that means that you cannot exchange set <span class="tex-span">{<i>a</i>, <i>b</i>}</span> for set <span class="tex-span">{<i>v</i>, <i>a</i>}</span>. However, you can always exchange set <span class="tex-span"><i>x</i></span> for any set <span class="tex-span"><i>y</i></span>, unless there is item <span class="tex-span"><i>p</i></span>, such that <span class="tex-span"><i>p</i></span> occurs in <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>p</i></span> occurs in <span class="tex-span"><i>y</i></span>.</p><p>For each item, John knows its value <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. John's sense of justice doesn't let him exchange a set of items <span class="tex-span"><i>x</i></span> for a set of items <span class="tex-span"><i>y</i></span>, if <span class="tex-span"><i>s</i>(<i>x</i>) + <i>d</i> &lt; <i>s</i>(<i>y</i>)</span> (<span class="tex-span"><i>s</i>(<i>x</i>)</span> is the total price of items in the set <span class="tex-span"><i>x</i></span>). </p><p>During one day John can exchange only one set of items for something else. Initially, he has no items. John wants to get a set of items with the maximum total price. Find the cost of such set and the minimum number of days John can get it in. </p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of items on the market and John's sense of justice value, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>).</p></div><div class="output-specification"><p>Print two space-separated integers: the maximum possible price in the set of items John can get and the minimum number of days needed to get such set.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">4</sup></span>) — the number of items on the market and John's sense of justice value, correspondingly. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>).</p>

## Output

<p>Print two space-separated integers: the maximum possible price in the set of items John can get and the minimum number of days needed to get such set.</p>





```input1
3 2
1 3 10

```




```input2
3 5
1 2 3

```




```input3
10 10000
10000 9999 1 10000 10000 10000 1 2 3 4

```




```output1
4 3

```




```output2
6 2

```




```output3
50010 6

```



## Note

<p>In the first sample John can act like this: </p><ul> <li> Take the first item (<span class="tex-span">1 - 0 ≤ 2</span>). </li><li> Exchange the first item for the second one (<span class="tex-span">3 - 1 ≤ 2</span>). </li><li> Take the first item (<span class="tex-span">1 - 0 ≤ 2</span>). </li></ul>
