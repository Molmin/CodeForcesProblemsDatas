## Description

<div><p>Everybody in Russia uses Gregorian calendar. In this calendar there are <span class="tex-span">31</span> days in January, <span class="tex-span">28</span> or <span class="tex-span">29</span> days in February (depending on whether the year is leap or not), <span class="tex-span">31</span> days in March, <span class="tex-span">30</span> days in April, <span class="tex-span">31</span> days in May, <span class="tex-span">30</span> in June, <span class="tex-span">31</span> in July, <span class="tex-span">31</span> in August, <span class="tex-span">30</span> in September, <span class="tex-span">31</span> in October, <span class="tex-span">30</span> in November, <span class="tex-span">31</span> in December.</p><p>A year is leap in one of two cases: either its number is divisible by <span class="tex-span">4</span>, but not divisible by <span class="tex-span">100</span>, or is divisible by <span class="tex-span">400</span>. For example, the following years are leap: <span class="tex-span">2000</span>, <span class="tex-span">2004</span>, but years <span class="tex-span">1900</span> and <span class="tex-span">2018</span> are not leap.</p><p>In this problem you are given <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 24</span>) integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, and you have to check if these integers could be durations in days of <span class="tex-span"><i>n</i></span> consecutive months, according to Gregorian calendar. Note that these months could belong to several consecutive years. In other words, check if there is a month in some year, such that its duration is <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> days, duration of the next month is <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span> days, and so on.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 24</span>) — the number of integers.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">28 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 31</span>) — the numbers you are to check.</p></div><div class="output-specification"><p>If there are several consecutive months that fit the sequence, print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in arbitrary case (small or large).</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 24</span>) — the number of integers.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">28 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 31</span>) — the numbers you are to check.</p>

## Output

<p>If there are several consecutive months that fit the sequence, print "<span class="tex-font-style-tt">YES</span>" (without quotes). Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p><p>You can print each letter in arbitrary case (small or large).</p>





```input1
4
31 31 30 31

```




```input2
2
30 30

```




```input3
5
29 31 30 31 30

```




```input4
3
31 28 30

```




```input5
3
31 31 28

```




```output1
Yes


```




```output2
No


```




```output3
Yes


```




```output4
No


```




```output5
Yes


```



## Note

<p>In the first example the integers can denote months July, August, September and October.</p><p>In the second example the answer is no, because there are no two consecutive months each having <span class="tex-span">30</span> days.</p><p>In the third example the months are: February (leap year) — March — April – May — June.</p><p>In the fourth example the number of days in the second month is <span class="tex-span">28</span>, so this is February. March follows February and has <span class="tex-span">31</span> days, but not <span class="tex-span">30</span>, so the answer is <span class="tex-font-style-tt">NO</span>.</p><p>In the fifth example the months are: December — January — February (non-leap year).</p>
