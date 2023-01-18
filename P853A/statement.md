## Description

<div><p>Helen works in Metropolis airport. She is responsible for creating a departure schedule. There are <span class="tex-span"><i>n</i></span> flights that must depart today, the <span class="tex-span"><i>i</i></span>-th of them is planned to depart at the <span class="tex-span"><i>i</i></span>-th minute of the day.</p><p>Metropolis airport is the main transport hub of Metropolia, so it is difficult to keep the schedule intact. This is exactly the case today: because of technical issues, no flights were able to depart during the first <span class="tex-span"><i>k</i></span> minutes of the day, so now the new departure schedule must be created.</p><p>All <span class="tex-span"><i>n</i></span> scheduled flights must now depart at different minutes between <span class="tex-span">(<i>k</i> + 1)</span>-th and <span class="tex-span">(<i>k</i> + <i>n</i>)</span>-th, inclusive. However, it's not mandatory for the flights to depart in the same order they were initially scheduled to do so&nbsp;— their order in the new schedule can be different. There is only one restriction: no flight is allowed to depart earlier than it was supposed to depart in the initial schedule.</p><p>Helen knows that each minute of delay of the <span class="tex-span"><i>i</i></span>-th flight costs airport <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> burles. Help her find the order for flights to depart in the new schedule that minimizes the total cost for the airport.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 300 000</span>), here <span class="tex-span"><i>n</i></span> is the number of flights, and <span class="tex-span"><i>k</i></span> is the number of minutes in the beginning of the day that the flights did not depart.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>), here <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the cost of delaying the <span class="tex-span"><i>i</i></span>-th flight for one minute.</p></div><div class="output-specification"><p>The first line must contain the minimum possible total cost of delaying the flights.</p><p>The second line must contain <span class="tex-span"><i>n</i></span> different integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>k</i> + 1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i> + <i>n</i></span>), here <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the minute when the <span class="tex-span"><i>i</i></span>-th flight must depart. If there are several optimal schedules, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 300 000</span>), here <span class="tex-span"><i>n</i></span> is the number of flights, and <span class="tex-span"><i>k</i></span> is the number of minutes in the beginning of the day that the flights did not depart.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>), here <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the cost of delaying the <span class="tex-span"><i>i</i></span>-th flight for one minute.</p>

## Output

<p>The first line must contain the minimum possible total cost of delaying the flights.</p><p>The second line must contain <span class="tex-span"><i>n</i></span> different integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"><i>k</i> + 1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i> + <i>n</i></span>), here <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the minute when the <span class="tex-span"><i>i</i></span>-th flight must depart. If there are several optimal schedules, print any of them.</p>





```input1
5 2
4 2 1 10 2

```




```output1
20
3 6 7 4 5 

```



## Note

<p>Let us consider sample test. If Helen just moves all flights <span class="tex-span">2</span> minutes later preserving the order, the total cost of delaying the flights would be <span class="tex-span">(3 - 1)·4 + (4 - 2)·2 + (5 - 3)·1 + (6 - 4)·10 + (7 - 5)·2 = 38</span> burles. </p><p>However, the better schedule is shown in the sample answer, its cost is <span class="tex-span">(3 - 1)·4 + (6 - 2)·2 + (7 - 3)·1 + (4 - 4)·10 + (5 - 5)·2 = 20</span> burles.</p>
