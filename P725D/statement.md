## Description

<div><p>One tradition of ACM-ICPC contests is that a team gets a balloon for every solved problem. We assume that the submission time doesn't matter and teams are sorted only by the number of balloons they have. It means that one's place is equal to the number of teams with more balloons, increased by <span class="tex-span">1</span>. For example, if there are seven teams with more balloons, you get the eight place. Ties are allowed.</p><p>You should know that it's important to eat before a contest. If the number of balloons of a team is greater than the weight of this team, the team starts to float in the air together with their workstation. They eventually touch the ceiling, what is strictly forbidden by the rules. The team is then disqualified and isn't considered in the standings.</p><p>A contest has just finished. There are <span class="tex-span"><i>n</i></span> teams, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th team has <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> balloons and weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>. It's guaranteed that <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> doesn't exceed <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> so nobody floats initially.</p><p>Limak is a member of the first team. He doesn't like cheating and he would never steal balloons from other teams. Instead, he can give his balloons away to other teams, possibly making them float. Limak can give away zero or more balloons of his team. Obviously, he can't give away more balloons than his team initially has.</p><p>What is the best place Limak can get?</p></div><div class="input-specification"><p>The first line of the standard input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 300 000</span>)&nbsp;— the number of teams.</p><p>The <span class="tex-span"><i>i</i></span>-th of <span class="tex-span"><i>n</i></span> following lines contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— respectively the number of balloons and the weight of the <span class="tex-span"><i>i</i></span>-th team. Limak is a member of the first team.</p></div><div class="output-specification"><p>Print one integer denoting the best place Limak can get.</p></div>

## Input

<p>The first line of the standard input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 300 000</span>)&nbsp;— the number of teams.</p><p>The <span class="tex-span"><i>i</i></span>-th of <span class="tex-span"><i>n</i></span> following lines contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— respectively the number of balloons and the weight of the <span class="tex-span"><i>i</i></span>-th team. Limak is a member of the first team.</p>

## Output

<p>Print one integer denoting the best place Limak can get.</p>





```input1
8
20 1000
32 37
40 1000
45 50
16 16
16 16
14 1000
2 1000

```




```input2
7
4 4
4 4
4 4
4 4
4 4
4 4
5 5

```




```input3
7
14000000003 1000000000000000000
81000000000 88000000000
5000000000 7000000000
15000000000 39000000000
46000000000 51000000000
0 1000000000
0 0

```




```output1
3

```




```output2
2

```




```output3
2

```



## Note

<p>In the first sample, Limak has <span class="tex-span">20</span> balloons initially. There are three teams with more balloons (<span class="tex-span">32</span>, <span class="tex-span">40</span> and <span class="tex-span">45</span> balloons), so Limak has the fourth place initially. One optimal strategy is:</p><ol><li> Limak gives <span class="tex-span">6</span> balloons away to a team with <span class="tex-span">32</span> balloons and weight <span class="tex-span">37</span>, which is just enough to make them fly. Unfortunately, Limak has only <span class="tex-span">14</span> balloons now and he would get the fifth place.</li><li> Limak gives <span class="tex-span">6</span> balloons away to a team with <span class="tex-span">45</span> balloons. Now they have <span class="tex-span">51</span> balloons and weight <span class="tex-span">50</span> so they fly and get disqualified.</li><li> Limak gives <span class="tex-span">1</span> balloon to each of two teams with <span class="tex-span">16</span> balloons initially.</li><li> Limak has <span class="tex-span">20 - 6 - 6 - 1 - 1 = 6</span> balloons.</li><li> There are three other teams left and their numbers of balloons are <span class="tex-span">40</span>, <span class="tex-span">14</span> and <span class="tex-span">2</span>.</li><li> Limak gets the third place because there are two teams with more balloons. </li></ol><p>In the second sample, Limak has the second place and he can't improve it.</p><p>In the third sample, Limak has just enough balloons to get rid of teams <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">5</span> (the teams with <span class="tex-span">81 000 000 000</span>, <span class="tex-span">5 000 000 000</span> and <span class="tex-span">46 000 000 000</span> balloons respectively). With zero balloons left, he will get the second place (ex-aequo with team <span class="tex-span">6</span> and team <span class="tex-span">7</span>).</p>
