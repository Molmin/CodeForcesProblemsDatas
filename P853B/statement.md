## Description

<div><p>Country of Metropolia is holding Olympiad of Metrpolises soon. It mean that all jury members of the olympiad should meet together in Metropolis (the capital of the country) for the problem preparation process.</p><p>There are <span class="tex-span"><i>n</i> + 1</span> cities consecutively numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i></span>. City <span class="tex-span">0</span> is Metropolis that is the meeting point for all jury members. For each city from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> there is exactly one jury member living there. Olympiad preparation is a long and demanding process that requires <span class="tex-span"><i>k</i></span> days of work. For all of these <span class="tex-span"><i>k</i></span> days each of the <span class="tex-span"><i>n</i></span> jury members should be present in Metropolis to be able to work on problems.</p><p>You know the flight schedule in the country (jury members consider themselves important enough to only use flights for transportation). All flights in Metropolia are either going to Metropolis or out of Metropolis. There are no night flights in Metropolia, or in the other words, plane always takes off at the same day it arrives. On his arrival day and departure day jury member is not able to discuss the olympiad. All flights in Megapolia depart and arrive at the same day.</p><p>Gather everybody for <span class="tex-span"><i>k</i></span> days in the capital is a hard objective, doing that while spending the minimum possible money is even harder. Nevertheless, your task is to arrange the cheapest way to bring all of the jury members to Metrpolis, so that they can work together for <span class="tex-span"><i>k</i></span> days and then send them back to their home cities. Cost of the arrangement is defined as a total cost of tickets for all used flights. It is allowed for jury member to stay in Metropolis for more than <span class="tex-span"><i>k</i></span> days.</p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>). </p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>m</i></span> lines contains the description of the <span class="tex-span"><i>i</i></span>-th flight defined by four integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, exactly one of <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals zero), the day of departure (and arrival), the departure city, the arrival city and the ticket cost.</p></div><div class="output-specification"><p>Output the only integer that is the minimum cost of gathering all jury members in city <span class="tex-span">0</span> for <span class="tex-span"><i>k</i></span> days and then sending them back to their home cities.</p><p>If it is impossible to gather everybody in Metropolis for <span class="tex-span"><i>k</i></span> days and then send them back to their home cities, output "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>). </p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>m</i></span> lines contains the description of the <span class="tex-span"><i>i</i></span>-th flight defined by four integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">0 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>, exactly one of <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> equals zero), the day of departure (and arrival), the departure city, the arrival city and the ticket cost.</p>

## Output

<p>Output the only integer that is the minimum cost of gathering all jury members in city <span class="tex-span">0</span> for <span class="tex-span"><i>k</i></span> days and then sending them back to their home cities.</p><p>If it is impossible to gather everybody in Metropolis for <span class="tex-span"><i>k</i></span> days and then send them back to their home cities, output "<span class="tex-font-style-tt">-1</span>" (without the quotes).</p>





```input1
2 6 5
1 1 0 5000
3 2 0 5500
2 2 0 6000
15 0 2 9000
9 0 1 7000
8 0 2 6500

```




```input2
2 4 5
1 2 0 5000
2 1 0 4500
2 1 0 3000
8 0 1 6000

```




```output1
24500

```




```output2
-1

```



## Note

<p>The optimal way to gather everybody in Metropolis in the first sample test is to use flights that take place on days <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">8</span> and <span class="tex-span">9</span>. The only alternative option is to send jury member from second city back home on day <span class="tex-span">15</span>, that would cost 2500 more.</p><p>In the second sample it is impossible to send jury member from city <span class="tex-span">2</span> back home from Metropolis.</p>
