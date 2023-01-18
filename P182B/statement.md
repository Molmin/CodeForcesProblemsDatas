## Description

<div><p>Vasya lives in a strange world. The year has <span class="tex-span"><i>n</i></span> months and the <span class="tex-span"><i>i</i></span>-th month has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> days. Vasya got a New Year present — the clock that shows not only the time, but also the date.</p><p>The clock's face can display any number from <span class="tex-span">1</span> to <span class="tex-span"><i>d</i></span>. It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i></span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The clock does not keep information about the current month, so when a new day comes, it simply increases the current day number by one. The clock cannot display number <span class="tex-span"><i>d</i> + 1</span>, so after day number <span class="tex-span"><i>d</i></span> it shows day <span class="tex-span">1</span> (the current day counter resets). The mechanism of the clock allows you to increase the day number by one manually. When you execute this operation, day <span class="tex-span"><i>d</i></span> is also followed by day <span class="tex-span">1</span>.</p><p>Vasya begins each day checking the day number on the clock. If the day number on the clock does not match the actual day number in the current month, then Vasya manually increases it by one. Vasya is persistent and repeats this operation until the day number on the clock matches the actual number of the current day in the current month.</p><p>A year passed and Vasya wonders how many times he manually increased the day number by one, from the first day of the first month to the last day of the <span class="tex-span"><i>n</i></span>-th month inclusive, considering that on the first day of the first month the clock display showed day <span class="tex-span">1</span>.</p></div><div class="input-specification"><p>The first line contains the single number <span class="tex-span"><i>d</i></span> — the maximum number of the day that Vasya's clock can show <span class="tex-span">(1 ≤ <i>d</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> — the number of months in the year <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000)</span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i>)</span> — the number of days in each month in the order in which they follow, starting from the first one. </p></div><div class="output-specification"><p>Print a single number — the number of times Vasya manually increased the day number by one throughout the last year.</p></div>

## Input

<p>The first line contains the single number <span class="tex-span"><i>d</i></span> — the maximum number of the day that Vasya's clock can show <span class="tex-span">(1 ≤ <i>d</i> ≤ 10<sup class="upper-index">6</sup>)</span>.</p><p>The second line contains a single integer <span class="tex-span"><i>n</i></span> — the number of months in the year <span class="tex-span">(1 ≤ <i>n</i> ≤ 2000)</span>.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i>)</span> — the number of days in each month in the order in which they follow, starting from the first one. </p>

## Output

<p>Print a single number — the number of times Vasya manually increased the day number by one throughout the last year.</p>





```input1
4
2
2 2

```




```input2
5
3
3 4 3

```




```input3
31
12
31 28 31 30 31 30 31 31 30 31 30 31

```




```output1
2

```




```output2
3

```




```output3
7

```



## Note

<p>In the first sample the situation is like this: </p><ul> <li> Day 1. Month 1. The clock shows <span class="tex-span">1</span>. Vasya changes nothing. </li><li> Day 2. Month 1. The clock shows <span class="tex-span">2</span>. Vasya changes nothing. </li><li> Day 1. Month 2. The clock shows <span class="tex-span">3</span>. Vasya manually increases the day number by <span class="tex-span">1</span>. After that the clock shows <span class="tex-span">4</span>. Vasya increases the day number by <span class="tex-span">1</span> manually. After that the clock shows <span class="tex-span">1</span>. </li><li> Day 2. Month 2. The clock shows <span class="tex-span">2</span>. Vasya changes nothing. </li></ul> In total, Vasya manually changed the day number by <span class="tex-span">1</span> exactly <span class="tex-span">2</span> times.
