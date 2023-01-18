## Description

<div><p><span class="tex-span"><i>n</i></span> participants of the competition were split into <span class="tex-span"><i>m</i></span> teams in some manner so that each team has at least one participant. After the competition each pair of participants from the same team became friends.</p><p>Your task is to write a program that will find the minimum and the maximum number of pairs of friends that could have formed by the end of the competition.</p></div><div class="input-specification"><p>The only line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, separated by a single space (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of participants and the number of teams respectively. </p></div><div class="output-specification"><p>The only line of the output should contain two integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>min</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>max</i></sub></span> — the minimum possible number of pairs of friends and the maximum possible number of pairs of friends respectively.</p></div>

## Input

<p>The only line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, separated by a single space (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of participants and the number of teams respectively. </p>

## Output

<p>The only line of the output should contain two integers <span class="tex-span"><i>k</i><sub class="lower-index"><i>min</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>max</i></sub></span> — the minimum possible number of pairs of friends and the maximum possible number of pairs of friends respectively.</p>





```input1
5 1

```




```input2
3 2

```




```input3
6 3

```




```output1
10 10

```




```output2
1 1

```




```output3
3 6

```



## Note

<p>In the first sample all the participants get into one team, so there will be exactly ten pairs of friends.</p><p>In the second sample at any possible arrangement one team will always have two participants and the other team will always have one participant. Thus, the number of pairs of friends will always be equal to one.</p><p>In the third sample minimum number of newly formed friendships can be achieved if participants were split on teams consisting of <span class="tex-span">2</span> people, maximum number can be achieved if participants were split on teams of <span class="tex-span">1</span>, <span class="tex-span">1</span> and <span class="tex-span">4</span> people.</p>
