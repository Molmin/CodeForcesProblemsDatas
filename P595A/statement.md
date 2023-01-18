## Description

<div><p>One day Vitaly was going home late at night and wondering: how many people aren't sleeping at that moment? To estimate, Vitaly decided to look which windows are lit in the house he was passing by at that moment.</p><p>Vitaly sees a building of <span class="tex-span"><i>n</i></span> floors and <span class="tex-span">2·<i>m</i></span> windows on each floor. On each floor there are <span class="tex-span"><i>m</i></span> flats numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>, and two consecutive windows correspond to each flat. If we number the windows from <span class="tex-span">1</span> to <span class="tex-span">2·<i>m</i></span> from left to right, then the <span class="tex-span"><i>j</i></span>-th flat of the <span class="tex-span"><i>i</i></span>-th floor has windows <span class="tex-span">2·<i>j</i> - 1</span> and <span class="tex-span">2·<i>j</i></span> in the corresponding row of windows (as usual, floors are enumerated from the bottom). Vitaly thinks that people in the flat aren't sleeping at that moment if <span class="tex-font-style-bf">at least one</span> of the windows corresponding to this flat has lights on.</p><p>Given the information about the windows of the given house, your task is to calculate the number of flats where, according to Vitaly, people aren't sleeping.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>)&nbsp;— the number of floors in the house and the number of flats on each floor respectively.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the floors from top to bottom and contain <span class="tex-span">2·<i>m</i></span> characters each. If the <span class="tex-span"><i>i</i></span>-th window of the given floor has lights on, then the <span class="tex-span"><i>i</i></span>-th character of this line is '<span class="tex-font-style-tt">1</span>', otherwise it is '<span class="tex-font-style-tt">0</span>'.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of flats that have lights on in at least one window, that is, the flats where, according to Vitaly, people aren't sleeping.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>)&nbsp;— the number of floors in the house and the number of flats on each floor respectively.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the floors from top to bottom and contain <span class="tex-span">2·<i>m</i></span> characters each. If the <span class="tex-span"><i>i</i></span>-th window of the given floor has lights on, then the <span class="tex-span"><i>i</i></span>-th character of this line is '<span class="tex-font-style-tt">1</span>', otherwise it is '<span class="tex-font-style-tt">0</span>'.</p>

## Output

<p>Print a single integer&nbsp;— the number of flats that have lights on in at least one window, that is, the flats where, according to Vitaly, people aren't sleeping.</p>





```input1
2 2
0 0 0 1
1 0 1 1

```




```input2
1 3
1 1 0 1 0 0

```




```output1
3

```




```output2
2

```



## Note

<p>In the first test case the house has two floors, two flats on each floor. That is, in total there are 4 flats. The light isn't on only on the second floor in the left flat. That is, in both rooms of the flat the light is off.</p><p>In the second test case the house has one floor and the first floor has three flats. The light is on in the leftmost flat (in both windows) and in the middle flat (in one window). In the right flat the light is off.</p>
