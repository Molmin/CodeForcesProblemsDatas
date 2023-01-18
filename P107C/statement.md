## Description

<div><p>In the year 2500 the annual graduation ceremony in the German University in Cairo (GUC) has run smoothly for almost 500 years so far.</p><p>The most important part of the ceremony is related to the arrangement of the professors in the ceremonial hall.</p><p>Traditionally GUC has <span class="tex-span"><i>n</i></span> professors. Each professor has his seniority level. All seniorities are different. Let's enumerate the professors from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, with <span class="tex-span">1</span> being the most senior professor and <span class="tex-span"><i>n</i></span> being the most junior professor.</p><p>The ceremonial hall has <span class="tex-span"><i>n</i></span> seats, one seat for each professor. Some places in this hall are meant for more senior professors than the others. More specifically, <span class="tex-span"><i>m</i></span> pairs of seats are in "senior-junior" relation, and the tradition requires that for all <span class="tex-span"><i>m</i></span> pairs of seats <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>)</span> the professor seated in "senior" position <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> should be more senior than the professor seated in "junior" position <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>GUC is very strict about its traditions, which have been carefully observed starting from year 2001. The tradition requires that: </p><ul> <li> The seating of the professors changes every year. </li><li> Year 2001 ceremony was using lexicographically first arrangement of professors in the ceremonial hall. </li><li> Each consecutive year lexicographically next arrangement of the professors is used. </li></ul><p>The arrangement of the professors is the list of <span class="tex-span"><i>n</i></span> integers, where the first integer is the seniority of the professor seated in position number one, the second integer is the seniority of the professor seated in position number two, etc.</p><p>Given <span class="tex-span"><i>n</i></span>, the number of professors, <span class="tex-span"><i>y</i></span>, the current year and <span class="tex-span"><i>m</i></span> pairs of restrictions, output the arrangement of the professors for this year.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 16, 2001 ≤ <i>y</i> ≤ 10<sup class="upper-index">18</sup>, 0 ≤ <i>m</i> ≤ 100</span>) — the number of professors, the year for which the arrangement should be computed, and the number of pairs of seats for which the seniority relation should be kept, respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain one pair of integers each, "<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>", indicating that professor on the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th seat is more senior than professor on the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th seat (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). Some pair may be listed more than once.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span> stream (you may also use the <span class="tex-font-style-tt">%I64d</span> specificator).</p></div><div class="output-specification"><p>Print the order in which the professors should be seated in the requested year.</p><p>If by this year the GUC would have ran out of arrangements, or the given "senior-junior" relation are contradictory, print "<span class="tex-font-style-tt">The times have changed</span>" (without quotes).</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 16, 2001 ≤ <i>y</i> ≤ 10<sup class="upper-index">18</sup>, 0 ≤ <i>m</i> ≤ 100</span>) — the number of professors, the year for which the arrangement should be computed, and the number of pairs of seats for which the seniority relation should be kept, respectively.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain one pair of integers each, "<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>", indicating that professor on the <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>-th seat is more senior than professor on the <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>-th seat (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). Some pair may be listed more than once.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span> stream (you may also use the <span class="tex-font-style-tt">%I64d</span> specificator).</p>

## Output

<p>Print the order in which the professors should be seated in the requested year.</p><p>If by this year the GUC would have ran out of arrangements, or the given "senior-junior" relation are contradictory, print "<span class="tex-font-style-tt">The times have changed</span>" (without quotes).</p>





```input1
3 2001 2
1 2
2 3

```




```input2
7 2020 6
1 2
1 3
2 4
2 5
3 6
3 7

```




```input3
10 3630801 0

```




```input4
3 2001 3
1 2
2 3
3 1

```




```output1
1 2 3

```




```output2
1 2 3 7 4 6 5

```




```output3
The times have changed

```




```output4
The times have changed

```



## Note

<p>In the first example the lexicographically first order of seating is 1 2 3.</p><p>In the third example the GUC will run out of arrangements after the year 3630800.</p><p>In the fourth example there are no valid arrangements for the seating.</p><p>The lexicographical comparison of arrangements is performed by the &lt; operator in modern programming languages. The arrangement <span class="tex-span"><i>a</i></span> is lexicographically less that the arrangement <span class="tex-span"><i>b</i></span>, if there exists such <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>b</i><sub class="lower-index"><i>j</i></sub></span>.</p>
