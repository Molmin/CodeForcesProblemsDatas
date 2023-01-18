## Description

<div><p>Vector Willman and Array Bolt are the two most famous athletes of Byteforces. They are going to compete in a race with a distance of <span class="tex-span"><i>L</i></span> meters today.</p><center> <img class="tex-graphics" src="file://vEgYZw5Y.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Willman and Bolt have exactly the same speed, so when they compete the result is always a tie. That is a problem for the organizers because they want a winner. </p><p>While watching previous races the organizers have noticed that Willman can perform <span class="tex-font-style-bf">only</span> steps of length equal to <span class="tex-span"><i>w</i></span> meters, and Bolt can perform <span class="tex-font-style-bf">only</span> steps of length equal to <span class="tex-span"><i>b</i></span> meters. Organizers decided to slightly change the rules of the race. Now, at the end of the racetrack there will be an abyss, and the winner will be declared the athlete, who manages to run farther from the starting point of the the racetrack (which is not the subject to change by any of the athletes). </p><p>Note that none of the athletes can run infinitely far, as they both will at some moment of time face the point, such that only one step further will cause them to fall in the abyss. In other words, the athlete <span class="tex-font-style-bf">will not</span> fall into the abyss if the total length of all his steps will be less or equal to the chosen distance <span class="tex-span"><i>L</i></span>.</p><p>Since the organizers are very fair, the are going to set the length of the racetrack as an integer chosen randomly and uniformly in range from 1 to <span class="tex-span"><i>t</i></span> (both are included). What is the probability that Willman and Bolt tie again today?</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>t</i>, <i>w</i>, <i>b</i> ≤ 5·10<sup class="upper-index">18</sup></span>) — the maximum possible length of the racetrack, the length of Willman's steps and the length of Bolt's steps respectively.</p></div><div class="output-specification"><p>Print the answer to the problem as an irreducible fraction <img align="middle" class="tex-formula" src="file://52Jj6St9.png" style="max-width: 100.0%;max-height: 100.0%;">. Follow the format of the samples output.</p><p>The fraction <img align="middle" class="tex-formula" src="file://kdea6Vdc.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> are integers, and both <span class="tex-span"><i>p</i> ≥ 0</span> and <span class="tex-span"><i>q</i> &gt; 0</span> holds) is called irreducible, if there is no such integer <span class="tex-span"><i>d</i> &gt; 1</span>, that both <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> are divisible by <span class="tex-span"><i>d</i></span>.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>w</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>t</i>, <i>w</i>, <i>b</i> ≤ 5·10<sup class="upper-index">18</sup></span>) — the maximum possible length of the racetrack, the length of Willman's steps and the length of Bolt's steps respectively.</p>

## Output

<p>Print the answer to the problem as an irreducible fraction <img align="middle" class="tex-formula" src="file://52Jj6St9.png" style="max-width: 100.0%;max-height: 100.0%;">. Follow the format of the samples output.</p><p>The fraction <img align="middle" class="tex-formula" src="file://kdea6Vdc.png" style="max-width: 100.0%;max-height: 100.0%;"> (<span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> are integers, and both <span class="tex-span"><i>p</i> ≥ 0</span> and <span class="tex-span"><i>q</i> &gt; 0</span> holds) is called irreducible, if there is no such integer <span class="tex-span"><i>d</i> &gt; 1</span>, that both <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> are divisible by <span class="tex-span"><i>d</i></span>.</p>





```input1
10 3 2

```




```input2
7 1 2

```




```output1
3/10

```




```output2
3/7

```



## Note

<p>In the first sample Willman and Bolt will tie in case <span class="tex-span">1</span>, <span class="tex-span">6</span> or <span class="tex-span">7</span> are chosen as the length of the racetrack.</p>
