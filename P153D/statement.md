## Description

<div><p>You are given a date in "<span class="tex-font-style-tt">DD.MM.YYYY</span>" ("day.month.year") format and a number of days <span class="tex-span"><i>shift</i></span> you have to add to this date. Output the resulting date.</p></div><div class="input-specification"><p>The first line of input contains the date in "<span class="tex-font-style-tt">DD.MM.YYYY</span>" format: two digits for day (with leading zero if needed), dot, two digits for month (with leading zero if needed), dot, four digits for year. The notation is guaranteed to give a valid date between 1980 and 2020, inclusive.</p><p>The second line contains an integer <span class="tex-span"><i>shift</i></span> (<span class="tex-span"> - 1000 ≤ <i>shift</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>Output a date equal to the given one + <span class="tex-span"><i>shift</i></span> days, in the same format "<span class="tex-font-style-tt">DD.MM.YYYY</span>".</p></div>

## Input

<p>The first line of input contains the date in "<span class="tex-font-style-tt">DD.MM.YYYY</span>" format: two digits for day (with leading zero if needed), dot, two digits for month (with leading zero if needed), dot, four digits for year. The notation is guaranteed to give a valid date between 1980 and 2020, inclusive.</p><p>The second line contains an integer <span class="tex-span"><i>shift</i></span> (<span class="tex-span"> - 1000 ≤ <i>shift</i> ≤ 1000</span>).</p>

## Output

<p>Output a date equal to the given one + <span class="tex-span"><i>shift</i></span> days, in the same format "<span class="tex-font-style-tt">DD.MM.YYYY</span>".</p>





```input1
10.02.2012
12

```




```input2
01.02.2010
-40

```




```input3
01.01.2000
365

```




```input4
13.08.1990
-609

```




```output1
22.02.2012

```




```output2
23.12.2009

```




```output3
31.12.2000

```




```output4
12.12.1988

```



## Note

<p>When manipulating the dates, take into account leap years; don't care about time zones/daylight saving time.</p>
