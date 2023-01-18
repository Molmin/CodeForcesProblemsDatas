## Description

<div><p>There are <span class="tex-span"><i>n</i></span> cities located along the one-way road. Cities are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the direction of the road.</p><p>The <span class="tex-span"><i>i</i></span>-th city had produced <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> units of goods. No more than <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> units of goods can be sold in the <span class="tex-span"><i>i</i></span>-th city.</p><p>For each pair of cities <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> such that <span class="tex-font-style-bf"><span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span></span> you can <span class="tex-font-style-bf">no more than once</span> transport <span class="tex-font-style-bf">no more than</span> <span class="tex-span"><i>c</i></span> units of goods from the city <span class="tex-span"><i>i</i></span> to the city <span class="tex-span"><i>j</i></span>. Note that goods can only be transported from a city with a lesser index to the city with a larger index. <span class="tex-font-style-bf">You can transport goods between cities in any order.</span></p><p>Determine the maximum number of produced goods that can be sold in total in all the cities after a sequence of transportations.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and&nbsp;<span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">0 ≤ <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of cities and the maximum amount of goods for a single transportation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of units of goods that were produced in each city.</p><p>The third line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of units of goods that can be sold in each city.</p></div><div class="output-specification"><p>Print the maximum total number of produced goods that can be sold in all cities after a sequence of transportations.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and&nbsp;<span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10 000</span>, <span class="tex-span">0 ≤ <i>c</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of cities and the maximum amount of goods for a single transportation.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of units of goods that were produced in each city.</p><p>The third line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of units of goods that can be sold in each city.</p>

## Output

<p>Print the maximum total number of produced goods that can be sold in all cities after a sequence of transportations.</p>





```input1
3 0
1 2 3
3 2 1

```




```input2
5 1
7 4 2 1 0
1 2 3 4 5

```




```input3
4 3
13 10 7 4
4 7 10 13

```




```output1
4

```




```output2
12

```




```output3
34

```


