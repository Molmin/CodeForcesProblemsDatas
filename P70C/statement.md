## Description

<div><p>In Walrusland public transport tickets are characterized by two integers: by the number of the series and by the number of the ticket in the series. Let the series number be represented by <span class="tex-span"><i>a</i></span> and the ticket number — by <span class="tex-span"><i>b</i></span>, then a ticket is described by the ordered pair of numbers <span class="tex-span">(<i>a</i>, <i>b</i>)</span>. </p><p>The walruses believe that a ticket is lucky if <span class="tex-span"><i>a</i> * <i>b</i> = <i>rev</i>(<i>a</i>) * <i>rev</i>(<i>b</i>)</span>. The function <span class="tex-span"><i>rev</i>(<i>x</i>)</span> reverses a number written in the decimal system, at that the leading zeroes disappear. For example, <span class="tex-span"><i>rev</i>(12343) = 34321</span>, <span class="tex-span"><i>rev</i>(1200) = 21</span>.</p><p>The Public Transport Management Committee wants to release <span class="tex-span"><i>x</i></span> series, each containing <span class="tex-span"><i>y</i></span> tickets, so that <span class="tex-font-style-bf">at</span> <span class="tex-font-style-bf">least</span> <span class="tex-span"><i>w</i></span> lucky tickets were released and the total number of released tickets (<span class="tex-span"><i>x</i> * <i>y</i></span>) were minimum. The series are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>x</i></span> inclusive. The tickets in each series are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>y</i></span> inclusive. The Transport Committee cannot release more than <span class="tex-span"><i>max</i><sub class="lower-index"><i>x</i></sub></span> series and more than <span class="tex-span"><i>max</i><sub class="lower-index"><i>y</i></sub></span> tickets in one series.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>max</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>max</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>max</i><sub class="lower-index"><i>x</i></sub>, <i>max</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">7</sup></span>).</p></div><div class="output-specification"><p>Print on a single line two space-separated numbers, the <span class="tex-span"><i>x</i></span> and the <span class="tex-span"><i>y</i></span>. If there are several possible variants, print any of them. If such <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> do not exist, print a single number <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>max</i><sub class="lower-index"><i>x</i></sub></span>, <span class="tex-span"><i>max</i><sub class="lower-index"><i>y</i></sub></span>, <span class="tex-span"><i>w</i></span> (<span class="tex-span">1 ≤ <i>max</i><sub class="lower-index"><i>x</i></sub>, <i>max</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>w</i> ≤ 10<sup class="upper-index">7</sup></span>).</p>

## Output

<p>Print on a single line two space-separated numbers, the <span class="tex-span"><i>x</i></span> and the <span class="tex-span"><i>y</i></span>. If there are several possible variants, print any of them. If such <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> do not exist, print a single number <span class="tex-span"> - 1</span>.</p>





```input1
2 2 1

```




```input2
132 10 35

```




```input3
5 18 1000

```




```input4
48 132 235

```




```output1
1 1
```




```output2
7 5
```




```output3
-1

```




```output4
22 111
```


