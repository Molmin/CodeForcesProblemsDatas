## Description

<div><p>You are given names of two days of the week.</p><p>Please, determine whether it is possible that during some <span class="tex-font-style-bf">non-leap year</span> the first day of some month was equal to the first day of the week you are given, while the first day of <span class="tex-font-style-bf">the next month</span> was equal to the second day of the week you are given. <span class="tex-font-style-bf">Both months should belong to one year</span>.</p><p>In this problem, we consider the Gregorian calendar to be used. The number of months in this calendar is equal to 12. The number of days in months during any non-leap year is: <span class="tex-span">31</span>, <span class="tex-span">28</span>, <span class="tex-span">31</span>, <span class="tex-span">30</span>, <span class="tex-span">31</span>, <span class="tex-span">30</span>, <span class="tex-span">31</span>, <span class="tex-span">31</span>, <span class="tex-span">30</span>, <span class="tex-span">31</span>, <span class="tex-span">30</span>, <span class="tex-span">31</span>.</p><p>Names of the days of the week are given with lowercase English letters: "<span class="tex-font-style-tt">monday</span>", "<span class="tex-font-style-tt">tuesday</span>", "<span class="tex-font-style-tt">wednesday</span>", "<span class="tex-font-style-tt">thursday</span>", "<span class="tex-font-style-tt">friday</span>", "<span class="tex-font-style-tt">saturday</span>", "<span class="tex-font-style-tt">sunday</span>".</p></div><div class="input-specification"><p>The input consists of two lines, each of them containing the name of exactly one day of the week. It's guaranteed that each string in the input is from the set "<span class="tex-font-style-tt">monday</span>", "<span class="tex-font-style-tt">tuesday</span>", "<span class="tex-font-style-tt">wednesday</span>", "<span class="tex-font-style-tt">thursday</span>", "<span class="tex-font-style-tt">friday</span>", "<span class="tex-font-style-tt">saturday</span>", "<span class="tex-font-style-tt">sunday</span>".</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if such situation is possible during some non-leap year. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The input consists of two lines, each of them containing the name of exactly one day of the week. It's guaranteed that each string in the input is from the set "<span class="tex-font-style-tt">monday</span>", "<span class="tex-font-style-tt">tuesday</span>", "<span class="tex-font-style-tt">wednesday</span>", "<span class="tex-font-style-tt">thursday</span>", "<span class="tex-font-style-tt">friday</span>", "<span class="tex-font-style-tt">saturday</span>", "<span class="tex-font-style-tt">sunday</span>".</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if such situation is possible during some non-leap year. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
monday
tuesday

```




```input2
sunday
sunday

```




```input3
saturday
tuesday

```




```output1
NO

```




```output2
YES

```




```output3
YES

```



## Note

<p>In the second sample, one can consider February 1 and March 1 of year 2015. Both these days were Sundays.</p><p>In the third sample, one can consider July 1 and August 1 of year 2017. First of these two days is Saturday, while the second one is Tuesday.</p>
