## Description

<div><p>Petr wants to make a calendar for current month. For this purpose he draws a table in which columns correspond to weeks (a week is seven consequent days from Monday to Sunday), rows correspond to weekdays, and cells contain dates. For example, a calendar for January 2017 should look like on the picture:</p><center> <img class="tex-graphics" src="file://Znah3v4b.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Petr wants to know how many columns his table should have given the month and the weekday of the first date of that month? Assume that the year is non-leap.</p></div><div class="input-specification"><p>The only line contain two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 12</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 7</span>)&nbsp;— the number of month (January is the first month, December is the twelfth) and the weekday of the first date of this month (<span class="tex-span">1</span> is Monday, <span class="tex-span">7</span> is Sunday).</p></div><div class="output-specification"><p>Print single integer: the number of columns the table should have.</p></div>

## Input

<p>The only line contain two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 12</span>, <span class="tex-span">1 ≤ <i>d</i> ≤ 7</span>)&nbsp;— the number of month (January is the first month, December is the twelfth) and the weekday of the first date of this month (<span class="tex-span">1</span> is Monday, <span class="tex-span">7</span> is Sunday).</p>

## Output

<p>Print single integer: the number of columns the table should have.</p>





```input1
1 7

```




```input2
1 1

```




```input3
11 6

```




```output1
6

```




```output2
5

```




```output3
5

```



## Note

<p>The first example corresponds to the January 2017 shown on the picture in the statements.</p><p>In the second example <span class="tex-span">1</span>-st January is Monday, so the whole month fits into <span class="tex-span">5</span> columns.</p><p>In the third example <span class="tex-span">1</span>-st November is Saturday and <span class="tex-span">5</span> columns is enough.</p>
