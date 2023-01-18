## Description

<div><p>Today is Wednesday, the third day of the week. What's more interesting is that tomorrow is the last day of the year 2015.</p><p>Limak is a little polar bear. He enjoyed this year a lot. Now, he is so eager to the coming year 2016.</p><p>Limak wants to prove how responsible a bear he is. He is going to regularly save candies for the entire year 2016! He considers various saving plans. He can save one candy either on some fixed day of the week or on some fixed day of the month.</p><p>Limak chose one particular plan. He isn't sure how many candies he will save in the 2016 with his plan. Please, calculate it and tell him.</p></div><div class="input-specification"><p>The only line of the input is in one of the following two formats: </p><ul> <li> "<span class="tex-font-style-tt"><span class="tex-span"><i>x</i></span> of week</span>" where <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 7</span>) denotes the day of the week. The 1-st day is Monday and the 7-th one is Sunday. </li><li> "<span class="tex-font-style-tt"><span class="tex-span"><i>x</i></span> of month</span>" where <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 31</span>) denotes the day of the month. </li></ul></div><div class="output-specification"><p>Print one integer&nbsp;— the number of candies Limak will save in the year 2016.</p></div>

## Input

<p>The only line of the input is in one of the following two formats: </p><ul> <li> "<span class="tex-font-style-tt"><span class="tex-span"><i>x</i></span> of week</span>" where <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 7</span>) denotes the day of the week. The 1-st day is Monday and the 7-th one is Sunday. </li><li> "<span class="tex-font-style-tt"><span class="tex-span"><i>x</i></span> of month</span>" where <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 31</span>) denotes the day of the month. </li></ul>

## Output

<p>Print one integer&nbsp;— the number of candies Limak will save in the year 2016.</p>





```input1
4 of week

```




```input2
30 of month

```




```output1
52

```




```output2
11

```



## Note

<p>Polar bears use the Gregorian calendar. It is the most common calendar and you likely use it too. You can read about it on Wikipedia if you want to – <a href="https://en.wikipedia.org/wiki/Gregorian_calendar">https://en.wikipedia.org/wiki/Gregorian_calendar</a>. The week starts with Monday.</p><p>In the first sample Limak wants to save one candy on each Thursday (the 4-th day of the week). There are <span class="tex-span">52</span> Thursdays in the 2016. Thus, he will save <span class="tex-span">52</span> candies in total.</p><p>In the second sample Limak wants to save one candy on the 30-th day of each month. There is the 30-th day in exactly <span class="tex-span">11</span> months in the 2016&nbsp;— all months but February. It means that Limak will save <span class="tex-span">11</span> candies in total.</p>
