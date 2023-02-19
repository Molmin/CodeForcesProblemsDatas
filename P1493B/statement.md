## Description

<div><p>The time on the planet Lapituletti goes the same way it goes on Earth but a day lasts $h$ hours and each hour lasts $m$ minutes. The inhabitants of that planet use digital clocks similar to earth ones. Clocks display time in a format <span class="tex-font-style-tt">HH:MM</span> (the number of hours in decimal is displayed first, then (after the colon) follows the number of minutes in decimal; the number of minutes and hours is written with leading zeros if needed to form a two-digit number). Hours are numbered from $0$ to $h-1$ and minutes are numbered from $0$ to $m-1$. </p><center> <img class="tex-graphics" src="file://C22BGD5P.png" style="max-width: 100.0%;max-height: 100.0%;"><p>That's how the digits are displayed on the clock. Please note that digit $1$ is placed in the <span class="tex-font-style-bf">middle</span> of its position. </p></center><p>A standard mirror is in use on the planet Lapituletti. Inhabitants often look at the reflection of the digital clocks in the mirror and feel happy when what you see on the reflected clocks is a valid time (that means that you see valid digits in the reflection and this time can be seen on the normal clocks at some moment of a day).</p><p>The image of the clocks in the mirror is reflected against a vertical axis. </p><center> <img class="tex-graphics" src="file://1WFKE2rG.png" style="max-width: 100.0%;max-height: 100.0%;"><p>The reflection is not a valid time.</p><p><img class="tex-graphics" src="file://CmS9hoQt.png" style="max-width: 100.0%;max-height: 100.0%;"></p><p>The reflection is a valid time with $h=24$, $m = 60$. However, for example, if $h=10$, $m=60$, then the reflection is not a valid time. </p></center><p>An inhabitant of the planet Lapituletti begins to look at a mirrored image of the clocks at some time moment $s$ and wants to know the nearest future time moment (which can possibly happen on the next day), when the reflected clock time is valid.</p><p>It can be shown that with any $h$, $m$, $s$ such a moment exists. If the reflected time is correct at the moment the inhabitant began to look at the clock, that moment is considered the nearest.</p><p>You are asked to solve the problem for several test cases.</p></div><div class="input-specification"><p>The first line contains a single integer $T$ ($1 \le T \le 100$) — the number of test cases.</p><p>The next $2 \cdot T$ lines contain the description of test cases. The description of each test case consists of two lines.</p><p>The first line of a test case contains two integers $h$, $m$ ($1 \le h, m \le 100$).</p><p>The second line contains the start time $s$ in the described format <span class="tex-font-style-tt">HH:MM</span>.</p></div><div class="output-specification"><p>For each test case output in a separate line the nearest moment in format <span class="tex-font-style-tt">HH:MM</span> when the reflected time is correct.</p></div>

## Input

<p>The first line contains a single integer $T$ ($1 \le T \le 100$) — the number of test cases.</p><p>The next $2 \cdot T$ lines contain the description of test cases. The description of each test case consists of two lines.</p><p>The first line of a test case contains two integers $h$, $m$ ($1 \le h, m \le 100$).</p><p>The second line contains the start time $s$ in the described format <span class="tex-font-style-tt">HH:MM</span>.</p>

## Output

<p>For each test case output in a separate line the nearest moment in format <span class="tex-font-style-tt">HH:MM</span> when the reflected time is correct.</p>





```input1
5
24 60
12:21
24 60
23:59
90 80
52:26
1 100
00:01
10 10
04:04
```




```output1
12:21
00:00
52:28
00:00
00:00
```



## Note

<p>In the second test case it is not hard to show that the reflection of <span class="tex-font-style-tt">23:59</span> is incorrect, while the reflection of the moment <span class="tex-font-style-tt">00:00</span> on the next day is correct. </p><center> <img class="tex-graphics" src="file://M1cIb5hZ.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
