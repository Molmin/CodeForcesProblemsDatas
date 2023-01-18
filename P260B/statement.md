## Description

<div><p>A recently found Ancient Prophesy is believed to contain the exact Apocalypse date. The prophesy is a string that only consists of digits and characters "<span class="tex-font-style-tt">-</span>".</p><p>We'll say that some date is mentioned in the Prophesy if there is a substring in the Prophesy that is the date's record in the format "<span class="tex-font-style-tt">dd-mm-yyyy</span>". We'll say that the number of the date's occurrences is the number of such substrings in the Prophesy. For example, the Prophesy "<span class="tex-font-style-tt">0012-10-2012-10-2012</span>" mentions date <span class="tex-font-style-tt">12-10-2012</span> twice (first time as "<span class="tex-font-style-tt">00<span class="tex-font-style-bf">12-10-2012</span>-10-2012</span>", second time as "<span class="tex-font-style-tt">0012-10-20<span class="tex-font-style-bf">12-10-2012</span></span>").</p><p>The date of the Apocalypse is such correct date that the number of times it is mentioned in the Prophesy is strictly larger than that of any other correct date.</p><p>A date is correct if the year lies in the range from <span class="tex-span">2013</span> to <span class="tex-span">2015</span>, the month is from <span class="tex-span">1</span> to <span class="tex-span">12</span>, and the number of the day is strictly more than a zero and doesn't exceed the number of days in the current month. Note that a date is written in the format "<span class="tex-font-style-tt">dd-mm-yyyy</span>", that means that leading zeroes may be added to the numbers of the months or days if needed. In other words, date "<span class="tex-font-style-tt">1-1-2013</span>" isn't recorded in the format "<span class="tex-font-style-tt">dd-mm-yyyy</span>", and date "<span class="tex-font-style-tt">01-01-2013</span>" is recorded in it.</p><p>Notice, that any year between 2013 and 2015 is not a leap year.</p></div><div class="input-specification"><p>The first line contains the Prophesy: a non-empty string that only consists of digits and characters "<span class="tex-font-style-tt">-</span>". The length of the Prophesy doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p></div><div class="output-specification"><p>In a single line print the date of the Apocalypse. It is guaranteed that such date exists and is unique.</p></div>

## Input

<p>The first line contains the Prophesy: a non-empty string that only consists of digits and characters "<span class="tex-font-style-tt">-</span>". The length of the Prophesy doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> characters.</p>

## Output

<p>In a single line print the date of the Apocalypse. It is guaranteed that such date exists and is unique.</p>





```input1
777-444---21-12-2013-12-2013-12-2013---444-777

```




```output1
13-12-2013
```


