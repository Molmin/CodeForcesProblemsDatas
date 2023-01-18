## Description

<div><p>In Gregorian calendar a typical year consists of <span class="tex-span">365</span> days and <span class="tex-span">12</span> months. The numbers of days in the months are: <span class="tex-span">31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31</span>. If year index is divisible by <span class="tex-span">400</span>, or divisible by <span class="tex-span">4</span> but not by <span class="tex-span">100</span>, the year becomes leap year, with one extra day in the second month (the one which typically has <span class="tex-span">28</span> days).</p><p>You are given the index of the year and the index of the day in the year. Find out the date of this day (day and month it will fall upon).</p></div><div class="input-specification"><p>The first line of input contains the year index, between <span class="tex-span">1600</span> and <span class="tex-span">2400</span>, inclusive. The second line contains the day index, between <span class="tex-span">1</span> and <span class="tex-span">366</span>, inclusive. It is guaranteed that the day index will be valid for this year, i.e., day <span class="tex-span">366</span> will occur only in a leap year.</p></div><div class="output-specification"><p>Output the index of the day and the index of the month, separated with a space.</p></div>

## Input

<p>The first line of input contains the year index, between <span class="tex-span">1600</span> and <span class="tex-span">2400</span>, inclusive. The second line contains the day index, between <span class="tex-span">1</span> and <span class="tex-span">366</span>, inclusive. It is guaranteed that the day index will be valid for this year, i.e., day <span class="tex-span">366</span> will occur only in a leap year.</p>

## Output

<p>Output the index of the day and the index of the month, separated with a space.</p>





```input1
2011
324

```




```input2
2012
274

```




```output1
20 11

```




```output2
30 9

```



## Note

<p>All indexes are <span class="tex-span">1</span>-based.</p>
