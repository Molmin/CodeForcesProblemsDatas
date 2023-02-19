## Description

<div><p>Victor has a <a href="https://en.wikipedia.org/wiki/24-hour_clock">24-hour clock</a> that shows the time in the format "<span class="tex-font-style-tt">HH:MM</span>" (<span class="tex-font-style-tt">00</span> $\le$ <span class="tex-font-style-tt">HH</span> $\le$ <span class="tex-font-style-tt">23</span>, <span class="tex-font-style-tt">00</span> $\le$ <span class="tex-font-style-tt">MM</span> $\le$ <span class="tex-font-style-tt">59</span>). He looks at the clock every $x$ minutes, and the clock is currently showing time $s$. </p><p>How many <span class="tex-font-style-bf">different</span> palindromes will Victor see in total after looking at the clock every $x$ minutes, the first time being at time $s$?</p><p>For example, if the clock starts out as <span class="tex-font-style-tt">03:12</span> and Victor looks at the clock every $360$ minutes (i.e. every $6$ hours), then he will see the times <span class="tex-font-style-tt">03:12</span>, <span class="tex-font-style-tt">09:12</span>, <span class="tex-font-style-tt">15:12</span>, <span class="tex-font-style-tt">21:12</span>, <span class="tex-font-style-tt">03:12</span>, and the times will continue to repeat. Here the time <span class="tex-font-style-tt">21:12</span> is the only palindrome he will ever see, so the answer is $1$.</p><p>A palindrome is a string that reads the same backward as forward. For example, the times <span class="tex-font-style-tt">12:21</span>, <span class="tex-font-style-tt">05:50</span>, <span class="tex-font-style-tt">11:11</span> are palindromes but <span class="tex-font-style-tt">13:13</span>, <span class="tex-font-style-tt">22:10</span>, <span class="tex-font-style-tt">02:22</span> are not.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of each test case follows.</p><p>The only line of each test case contains a string $s$ of length $5$ with the format "<span class="tex-font-style-tt">HH:MM</span>" where "<span class="tex-font-style-tt">HH</span>" is from "<span class="tex-font-style-tt">00</span>" to "<span class="tex-font-style-tt">23</span>" and "<span class="tex-font-style-tt">MM</span>" is from "<span class="tex-font-style-tt">00</span>" to "<span class="tex-font-style-tt">59</span>" (both "<span class="tex-font-style-tt">HH</span>" and "<span class="tex-font-style-tt">MM</span>" have exactly two digits) and an integer $x$ ($1 \leq x \leq 1440$)&nbsp;— the number of minutes Victor takes to look again at the clock.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the number of different palindromes Victor will see if he looks at the clock every $x$ minutes starting from time $s$.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \leq t \leq 100$)&nbsp;— the number of test cases. The description of each test case follows.</p><p>The only line of each test case contains a string $s$ of length $5$ with the format "<span class="tex-font-style-tt">HH:MM</span>" where "<span class="tex-font-style-tt">HH</span>" is from "<span class="tex-font-style-tt">00</span>" to "<span class="tex-font-style-tt">23</span>" and "<span class="tex-font-style-tt">MM</span>" is from "<span class="tex-font-style-tt">00</span>" to "<span class="tex-font-style-tt">59</span>" (both "<span class="tex-font-style-tt">HH</span>" and "<span class="tex-font-style-tt">MM</span>" have exactly two digits) and an integer $x$ ($1 \leq x \leq 1440$)&nbsp;— the number of minutes Victor takes to look again at the clock.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the number of different palindromes Victor will see if he looks at the clock every $x$ minutes starting from time $s$.</p>





```input1
6
03:12 360
00:00 1
13:22 2
15:15 10
11:11 1440
22:30 27
```




```output1
1
16
10
0
1
1
```



## Note

<p>The first test case is explained in the statement.</p>
