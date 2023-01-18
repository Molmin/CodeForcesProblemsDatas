## Description

<div><p>Devu is a renowned classical singer. He is invited to many big functions/festivals. Recently he was invited to "All World Classical Singing Festival". Other than Devu, comedian Churu was also invited.</p><p>Devu has provided organizers a list of the songs and required time for singing them. He will sing <span class="tex-span"><i>n</i></span> songs, <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> song will take <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> minutes exactly. </p><p>The Comedian, Churu will crack jokes. All his jokes are of 5 minutes exactly.</p><p>People have mainly come to listen Devu. But you know that he needs rest of 10 minutes after each song. On the other hand, Churu being a very active person, doesn't need any rest.</p><p>You as one of the organizers should make an optimal sсhedule for the event. For some reasons you must follow the conditions:</p><ul> <li> The duration of the event must be no more than <span class="tex-span"><i>d</i></span> minutes; </li><li> Devu must complete all his songs; </li><li> With satisfying the two previous conditions the number of jokes cracked by Churu should be as many as possible. </li></ul><p>If it is not possible to find a way to conduct all the songs of the Devu, output -1. Otherwise find out maximum number of jokes that Churu can crack in the grand event.</p></div><div class="input-specification"><p>The first line contains two space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100;&nbsp;1 ≤ <i>d</i> ≤ 10000)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p></div><div class="output-specification"><p>If there is no way to conduct all the songs of Devu, output -1. Otherwise output the maximum number of jokes that Churu can crack in the grand event.</p></div>

## Input

<p>The first line contains two space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100;&nbsp;1 ≤ <i>d</i> ≤ 10000)</span>. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>.</p>

## Output

<p>If there is no way to conduct all the songs of Devu, output -1. Otherwise output the maximum number of jokes that Churu can crack in the grand event.</p>





```input1
3 30
2 2 1

```




```input2
3 20
2 1 1

```




```output1
5

```




```output2
-1

```



## Note

<p>Consider the first example. The duration of the event is <span class="tex-span">30</span> minutes. There could be maximum <span class="tex-span">5</span> jokes in the following way:</p><ul> <li> First Churu cracks a joke in <span class="tex-span">5</span> minutes. </li><li> Then Devu performs the first song for <span class="tex-span">2</span> minutes. </li><li> Then Churu cracks <span class="tex-span">2</span> jokes in <span class="tex-span">10</span> minutes. </li><li> Now Devu performs second song for <span class="tex-span">2</span> minutes. </li><li> Then Churu cracks <span class="tex-span">2</span> jokes in <span class="tex-span">10</span> minutes. </li><li> Now finally Devu will perform his last song in <span class="tex-span">1</span> minutes. </li></ul> <p>Total time spent is <span class="tex-span">5 + 2 + 10 + 2 + 10 + 1 = 30</span> minutes.</p><p>Consider the second example. There is no way of organizing Devu's all songs. Hence the answer is -1. </p>
