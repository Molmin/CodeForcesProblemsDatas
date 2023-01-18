## Description

<div><p>Very soon Berland will hold a School Team Programming Olympiad. From each of the <span class="tex-span"><i>m</i></span> Berland regions a team of two people is invited to participate in the olympiad. The qualifying contest to form teams was held and it was attended by <span class="tex-span"><i>n</i></span> Berland students. There were at least two schoolboys participating from each of the <span class="tex-span"><i>m</i></span> regions of Berland. The result of each of the participants of the qualifying competition is an integer score from <span class="tex-span">0</span> to <span class="tex-span">800</span> inclusive.</p><p>The team of each region is formed from two such members of the qualifying competition of the region, that none of them can be replaced by a schoolboy of the same region, not included in the team and who received a <span class="tex-font-style-bf">greater</span> number of points. There may be a situation where a team of some region can not be formed uniquely, that is, there is more than one school team that meets the properties described above. In this case, the region needs to undertake an additional contest. The two teams in the region are considered to be different if there is at least one schoolboy who is included in one team and is not included in the other team. It is guaranteed that for each region at least two its representatives participated in the qualifying contest.</p><p>Your task is, given the results of the qualifying competition, to identify the team from each region, or to announce that in this region its formation requires additional contests.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10 000</span>, <span class="tex-span"><i>n</i> ≥ 2<i>m</i></span>)&nbsp;— the number of participants of the qualifying contest and the number of regions in Berland.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of the participants of the qualifying contest in the following format: Surname (a string of length from <span class="tex-span">1</span> to <span class="tex-span">10</span> characters and consisting of large and small English letters), region number (integer from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>) and the number of points scored by the participant (integer from <span class="tex-span">0</span> to <span class="tex-span">800</span>, inclusive).</p><p>It is guaranteed that all surnames of all the participants are distinct and at least two people participated from each of the <span class="tex-span"><i>m</i></span> regions. The surnames that only differ in letter cases, should be considered distinct.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines. On the <span class="tex-span"><i>i</i></span>-th line print the team of the <span class="tex-span"><i>i</i></span>-th region&nbsp;— the surnames of the two team members in an arbitrary order, or a single character "<span class="tex-font-style-tt">?</span>" (without the quotes) if you need to spend further qualifying contests in the region.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10 000</span>, <span class="tex-span"><i>n</i> ≥ 2<i>m</i></span>)&nbsp;— the number of participants of the qualifying contest and the number of regions in Berland.</p><p>Next <span class="tex-span"><i>n</i></span> lines contain the description of the participants of the qualifying contest in the following format: Surname (a string of length from <span class="tex-span">1</span> to <span class="tex-span">10</span> characters and consisting of large and small English letters), region number (integer from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>) and the number of points scored by the participant (integer from <span class="tex-span">0</span> to <span class="tex-span">800</span>, inclusive).</p><p>It is guaranteed that all surnames of all the participants are distinct and at least two people participated from each of the <span class="tex-span"><i>m</i></span> regions. The surnames that only differ in letter cases, should be considered distinct.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines. On the <span class="tex-span"><i>i</i></span>-th line print the team of the <span class="tex-span"><i>i</i></span>-th region&nbsp;— the surnames of the two team members in an arbitrary order, or a single character "<span class="tex-font-style-tt">?</span>" (without the quotes) if you need to spend further qualifying contests in the region.</p>





```input1
5 2
Ivanov 1 763
Andreev 2 800
Petrov 1 595
Sidorov 1 790
Semenov 2 503

```




```input2
5 2
Ivanov 1 800
Andreev 2 763
Petrov 1 800
Sidorov 1 800
Semenov 2 503

```




```output1
Sidorov Ivanov
Andreev Semenov

```




```output2
?
Andreev Semenov

```



## Note

<p>In the first sample region teams are uniquely determined.</p><p>In the second sample the team from region <span class="tex-span">2</span> is uniquely determined and the team from region <span class="tex-span">1</span> can have three teams: "<span class="tex-font-style-tt">Petrov</span>"-"<span class="tex-font-style-tt">Sidorov</span>", "<span class="tex-font-style-tt">Ivanov</span>"-"<span class="tex-font-style-tt">Sidorov</span>", "<span class="tex-font-style-tt">Ivanov</span>" -"<span class="tex-font-style-tt">Petrov</span>", so it is impossible to determine a team uniquely.</p>
