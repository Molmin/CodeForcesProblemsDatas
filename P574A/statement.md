## Description

<div><p>Limak is a grizzly bear who desires power and adoration. He wants to win in upcoming elections and rule over the Bearland.</p><p>There are <span class="tex-span"><i>n</i></span> candidates, including Limak. We know how many citizens are going to vote for each candidate. Now <span class="tex-span"><i>i</i></span>-th candidate would get <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> votes. Limak is candidate number <span class="tex-span">1</span>. To win in elections, he must get strictly more votes than any other candidate.</p><p>Victory is more important than everything else so Limak decided to cheat. He will steal votes from his opponents by bribing some citizens. To bribe a citizen, Limak must give him or her one candy - citizens are bears and bears like candies. Limak doesn't have many candies and wonders - how many citizens does he have to bribe?</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) - number of candidates.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) - number of votes for each candidate. Limak is candidate number <span class="tex-span">1</span>.</p><p>Note that after bribing number of votes for some candidate might be zero or might be greater than <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>Print the minimum number of citizens Limak must bribe to have strictly more votes than any other candidate.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) - number of candidates.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) - number of votes for each candidate. Limak is candidate number <span class="tex-span">1</span>.</p><p>Note that after bribing number of votes for some candidate might be zero or might be greater than <span class="tex-span">1000</span>.</p>

## Output

<p>Print the minimum number of citizens Limak must bribe to have strictly more votes than any other candidate.</p>





```input1
5
5 1 11 2 8

```




```input2
4
1 8 8 8

```




```input3
2
7 6

```




```output1
4

```




```output2
6

```




```output3
0

```



## Note

<p>In the first sample Limak has <span class="tex-span">5</span> votes. One of the ways to achieve victory is to bribe <span class="tex-span">4</span> citizens who want to vote for the third candidate. Then numbers of votes would be <span class="tex-span">9, 1, 7, 2, 8</span> (Limak would have <span class="tex-span">9</span> votes). Alternatively, Limak could steal only <span class="tex-span">3</span> votes from the third candidate and <span class="tex-span">1</span> vote from the second candidate to get situation <span class="tex-span">9, 0, 8, 2, 8</span>.</p><p>In the second sample Limak will steal <span class="tex-span">2</span> votes from each candidate. Situation will be <span class="tex-span">7, 6, 6, 6</span>.</p><p>In the third sample Limak is a winner without bribing any citizen.</p>
