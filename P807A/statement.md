## Description

<div><p><span class="tex-font-style-underline">Is it rated?</span></p><p>Here it is. The Ultimate Question of Competitive Programming, Codeforces, and Everything. And you are here to answer it.</p><p>Another Codeforces round has been conducted. No two participants have the same number of points. For each participant, from the top to the bottom of the standings, their rating before and after the round is known.</p><p>It's known that if at least one participant's rating has changed, then the round was rated for sure.</p><p>It's also known that if the round was rated and a participant with lower rating took a better place in the standings than a participant with higher rating, then at least one round participant's rating has changed.</p><p>In this problem, you should not make any other assumptions about the rating system.</p><p>Determine if the current round is rated, unrated, or it's impossible to determine whether it is rated of not.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of round participants.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 4126</span>)&nbsp;— the rating of the <span class="tex-span"><i>i</i></span>-th participant before and after the round, respectively. The participants are listed in order from the top to the bottom of the standings.</p></div><div class="output-specification"><p>If the round is rated for sure, print "<span class="tex-font-style-tt">rated</span>". If the round is unrated for sure, print "<span class="tex-font-style-tt">unrated</span>". If it's impossible to determine whether the round is rated or not, print "<span class="tex-font-style-tt">maybe</span>".</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of round participants.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 4126</span>)&nbsp;— the rating of the <span class="tex-span"><i>i</i></span>-th participant before and after the round, respectively. The participants are listed in order from the top to the bottom of the standings.</p>

## Output

<p>If the round is rated for sure, print "<span class="tex-font-style-tt">rated</span>". If the round is unrated for sure, print "<span class="tex-font-style-tt">unrated</span>". If it's impossible to determine whether the round is rated or not, print "<span class="tex-font-style-tt">maybe</span>".</p>





```input1
6
3060 3060
2194 2194
2876 2903
2624 2624
3007 2991
2884 2884

```




```input2
4
1500 1500
1300 1300
1200 1200
1400 1400

```




```input3
5
3123 3123
2777 2777
2246 2246
2246 2246
1699 1699

```




```output1
rated

```




```output2
unrated

```




```output3
maybe

```



## Note

<p>In the first example, the ratings of the participants in the third and fifth places have changed, therefore, the round was rated.</p><p>In the second example, no one's rating has changed, but the participant in the second place has lower rating than the participant in the fourth place. Therefore, if the round was rated, someone's rating would've changed for sure.</p><p>In the third example, no one's rating has changed, and the participants took places in non-increasing order of their rating. Therefore, it's impossible to determine whether the round is rated or not.</p>
