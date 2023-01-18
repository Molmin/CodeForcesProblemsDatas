## Description

<div><p>Buses run between the cities <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>, the first one is at 05:00 AM and the last one departs not later than at 11:59 PM. A bus from the city <span class="tex-span"><i>A</i></span> departs every <span class="tex-span"><i>a</i></span> minutes and arrives to the city <span class="tex-span"><i>B</i></span> in a <span class="tex-span"><i>t</i><sub class="lower-index"><i>a</i></sub></span> minutes, and a bus from the city <span class="tex-span"><i>B</i></span> departs every <span class="tex-span"><i>b</i></span> minutes and arrives to the city <span class="tex-span"><i>A</i></span> in a <span class="tex-span"><i>t</i><sub class="lower-index"><i>b</i></sub></span> minutes.</p><p>The driver Simion wants to make his job diverse, so he counts the buses going towards him. Simion doesn't count the buses he meet at the start and finish.</p><p>You know the time when Simion departed from the city <span class="tex-span"><i>A</i></span> to the city <span class="tex-span"><i>B</i></span>. Calculate the number of buses Simion will meet to be sure in his counting.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>a</i>, <i>t</i><sub class="lower-index"><i>a</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>t</i><sub class="lower-index"><i>a</i></sub> ≤ 120</span>) — the frequency of the buses from the city <span class="tex-span"><i>A</i></span> to the city <span class="tex-span"><i>B</i></span> and the travel time. Both values are given in minutes.</p><p>The second line contains two integers <span class="tex-span"><i>b</i>, <i>t</i><sub class="lower-index"><i>b</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i>, <i>t</i><sub class="lower-index"><i>b</i></sub> ≤ 120</span>) — the frequency of the buses from the city <span class="tex-span"><i>B</i></span> to the city <span class="tex-span"><i>A</i></span> and the travel time. Both values are given in minutes.</p><p>The last line contains the departure time of Simion from the city <span class="tex-span"><i>A</i></span> in the format <span class="tex-font-style-tt">hh:mm</span>. It is guaranteed that there are a bus from the city <span class="tex-span"><i>A</i></span> at that time. Note that the hours and the minutes are given with exactly two digits.</p></div><div class="output-specification"><p>Print the only integer <span class="tex-span"><i>z</i></span> — the number of buses Simion will meet on the way. Note that you should not count the encounters in cities <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>a</i>, <i>t</i><sub class="lower-index"><i>a</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>t</i><sub class="lower-index"><i>a</i></sub> ≤ 120</span>) — the frequency of the buses from the city <span class="tex-span"><i>A</i></span> to the city <span class="tex-span"><i>B</i></span> and the travel time. Both values are given in minutes.</p><p>The second line contains two integers <span class="tex-span"><i>b</i>, <i>t</i><sub class="lower-index"><i>b</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i>, <i>t</i><sub class="lower-index"><i>b</i></sub> ≤ 120</span>) — the frequency of the buses from the city <span class="tex-span"><i>B</i></span> to the city <span class="tex-span"><i>A</i></span> and the travel time. Both values are given in minutes.</p><p>The last line contains the departure time of Simion from the city <span class="tex-span"><i>A</i></span> in the format <span class="tex-font-style-tt">hh:mm</span>. It is guaranteed that there are a bus from the city <span class="tex-span"><i>A</i></span> at that time. Note that the hours and the minutes are given with exactly two digits.</p>

## Output

<p>Print the only integer <span class="tex-span"><i>z</i></span> — the number of buses Simion will meet on the way. Note that you should not count the encounters in cities <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span>.</p>





```input1
10 30
10 35
05:20

```




```input2
60 120
24 100
13:00

```




```output1
5

```




```output2
9

```



## Note

<p>In the first example Simion departs form the city <span class="tex-span"><i>A</i></span> at 05:20 AM and arrives to the city <span class="tex-span"><i>B</i></span> at 05:50 AM. He will meet the first <span class="tex-span">5</span> buses from the city <span class="tex-span"><i>B</i></span> that departed in the period [05:00 AM - 05:40 AM]. Also Simion will meet a bus in the city <span class="tex-span"><i>B</i></span> at 05:50 AM, but he will not count it.</p><p>Also note that the first encounter will be between 05:26 AM and 05:27 AM (if we suggest that the buses are go with the sustained speed).</p>
