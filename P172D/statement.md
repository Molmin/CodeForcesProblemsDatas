## Description

<div><p>Reforms have started in Berland again! At this time, the Parliament is discussing the reform of the calendar. To make the lives of citizens of Berland more varied, it was decided to change the calendar. As more and more people are complaining that "the years fly by...", it was decided that starting from the next year the number of days per year will begin to grow. So the coming year will have exactly <span class="tex-span"><i>a</i></span> days, the next after coming year will have <span class="tex-span"><i>a</i> + 1</span> days, the next one will have <span class="tex-span"><i>a</i> + 2</span> days and so on. This schedule is planned for the coming <span class="tex-span"><i>n</i></span> years (in the <span class="tex-span"><i>n</i></span>-th year the length of the year will be equal <span class="tex-span"><i>a</i> + <i>n</i> - 1</span> day).</p><p>No one has yet decided what will become of months. An MP Palevny made the following proposal. </p><ul> <li> The calendar for each month is comfortable to be printed on a square sheet of paper. We are proposed to make the number of days in each month be the square of some integer. The number of days per month should be the same for each month of any year, but may be different for different years. </li><li> The number of days in each year must be divisible by the number of days per month in this year. This rule ensures that the number of months in each year is an integer. </li><li> The number of days per month for each year must be chosen so as to save the maximum amount of paper to print the calendars. In other words, the number of days per month should be as much as possible. </li></ul><p>These rules provide an unambiguous method for choosing the number of days in each month for any given year length. For example, according to Palevny's proposition, a year that consists of 108 days will have three months, 36 days each. The year that consists of 99 days will have 11 months, 9 days each, and a year of 365 days will have 365 months, one day each.</p><p>The proposal provoked heated discussion in the community, the famous mathematician Perelmanov quickly calculated that if the proposal is supported, then in a period of <span class="tex-span"><i>n</i></span> years, beginning with the year that has <span class="tex-span"><i>a</i></span> days, the country will spend <span class="tex-span"><i>p</i></span> sheets of paper to print a set of calendars for these years. Perelmanov's calculations take into account the fact that the set will contain one calendar for each year and each month will be printed on a separate sheet.</p><p>Repeat Perelmanov's achievement and print the required number <span class="tex-span"><i>p</i></span>. You are given positive integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>n</i></span>. Perelmanov warns you that your program should not work longer than four seconds at the maximum test.</p></div><div class="input-specification"><p>The only input line contains a pair of integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>n</i> ≤ 10<sup class="upper-index">7</sup>;</span> <span class="tex-span"><i>a</i> + <i>n</i> - 1 ≤ 10<sup class="upper-index">7</sup></span>).</p></div><div class="output-specification"><p>Print the required number <span class="tex-span"><i>p</i></span>. </p><p>Please, do not use the %lld specifier to read or write 64-bit integers in C++. It is preferred to use cin, cout streams or the %I64d specifier.</p></div>

## Input

<p>The only input line contains a pair of integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>n</i> ≤ 10<sup class="upper-index">7</sup>;</span> <span class="tex-span"><i>a</i> + <i>n</i> - 1 ≤ 10<sup class="upper-index">7</sup></span>).</p>

## Output

<p>Print the required number <span class="tex-span"><i>p</i></span>. </p><p>Please, do not use the %lld specifier to read or write 64-bit integers in C++. It is preferred to use cin, cout streams or the %I64d specifier.</p>





```input1
25 3

```




```input2
50 5

```




```output1
30

```




```output2
125

```



## Note

<p>A note to the first sample test. A year of 25 days will consist of one month containing 25 days. A year of 26 days will consist of 26 months, one day each. A year of 27 days will have three months, 9 days each.</p>
