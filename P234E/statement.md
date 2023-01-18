## Description

<div><p>In the autumn of this year, two Russian teams came into the group stage of the most prestigious football club competition in the world — the UEFA Champions League. Now, these teams have already started to play in the group stage and are fighting for advancing to the playoffs. In this problem we are interested in the draw stage, the process of sorting teams into groups.</p><p>The process of the draw goes as follows (the rules that are described in this problem, are somehow simplified compared to the real life). Suppose <span class="tex-span"><i>n</i></span> teams will take part in the group stage (<span class="tex-span"><i>n</i></span> is divisible by four). The teams should be divided into groups of four. Let's denote the number of groups as <span class="tex-span"><i>m</i></span> (<img align="middle" class="tex-formula" src="file://2AUimmQr.png" style="max-width: 100.0%;max-height: 100.0%;">). Each team has a rating — an integer characterizing the team's previous achievements. The teams are sorted by the rating's decreasing (no two teams have the same rating).</p><p>After that four "baskets" are formed, each of which will contain <span class="tex-span"><i>m</i></span> teams: the first <span class="tex-span"><i>m</i></span> teams with the highest rating go to the first basket, the following <span class="tex-span"><i>m</i></span> teams go to the second one, and so on.</p><p>Then the following procedure repeats <span class="tex-span"><i>m</i> - 1</span> times. A team is randomly taken from each basket, first from the first basket, then from the second, then from the third, and at last, from the fourth. The taken teams form another group. After that, they are <span class="tex-font-style-bf">removed</span> from their baskets.</p><p>The four teams remaining in the baskets after <span class="tex-span">(<i>m</i> - 1)</span> such procedures are performed, form the last group.</p><p>In the real draw the random selection of teams from the basket is performed by people — as a rule, the well-known players of the past. As we have none, we will use a random number generator, which is constructed as follows. Its parameters are four positive integers <span class="tex-span"><i>x</i>, <i>a</i>, <i>b</i>, <i>c</i></span>. Every time there is a call to the random number generator, it produces the following actions:</p><ul> <li> calculates <img align="middle" class="tex-formula" src="file://nmQe65Ec.png" style="max-width: 100.0%;max-height: 100.0%;">; </li><li> replaces parameter <span class="tex-span"><i>x</i></span> by value <span class="tex-span"><i>y</i></span> (assigns <img align="middle" class="tex-formula" src="file://9InBwIGa.png" style="max-width: 100.0%;max-height: 100.0%;">); </li><li> returns <span class="tex-span"><i>x</i></span> as another random number. </li></ul><p>Operation <img align="middle" class="tex-formula" src="file://gbUTQHXI.png" style="max-width: 100.0%;max-height: 100.0%;"> means taking the remainder after division: <img align="middle" class="tex-formula" src="file://acUz8x7o.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://k3DgmKqJ.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>A random number generator will be used in the draw as follows: each time we need to randomly choose a team from the basket, it will generate a random number <span class="tex-span"><i>k</i></span>. The teams that yet remain in the basket are considered numbered with consecutive integers from <span class="tex-span">0</span> to <span class="tex-span"><i>s</i> - 1</span>, in the order of decreasing rating, where <span class="tex-span"><i>s</i></span> is the current size of the basket. Then a team number <img align="middle" class="tex-formula" src="file://vXEfg3NJ.png" style="max-width: 100.0%;max-height: 100.0%;"> is taken from the basket.</p><p>Given a list of teams and the parameters of the random number generator, determine the result of the draw. </p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 64</span>, <span class="tex-span"><i>n</i></span> is divisible by four) — the number of teams that take part in the sorting. The second line contains four space-separated integers <span class="tex-span"><i>x</i>, <i>a</i>, <i>b</i>, <i>c</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>a</i>, <i>b</i>, <i>c</i> ≤ 1000</span>) — the parameters of the random number generator. Each of the following <span class="tex-span"><i>n</i></span> lines describes one team. The description consists of the name of the team and its rating, separated by a single space. The name of a team consists of uppercase and lowercase English letters and has length from 1 to 20 characters. A team's rating is an integer from 0 to 1000. All teams' names are distinct. All team's ratings are also distinct.</p></div><div class="output-specification"><p>Print the way the teams must be sorted into groups. Print the groups in the order, in which they are formed in the sorting. Number the groups by consecutive uppercase English letters, starting from letter <span class="tex-font-style-tt">'A'</span>. Inside each group print the teams' names one per line, in the order of decreasing of the teams' rating. See samples for a better understanding of the output format.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 64</span>, <span class="tex-span"><i>n</i></span> is divisible by four) — the number of teams that take part in the sorting. The second line contains four space-separated integers <span class="tex-span"><i>x</i>, <i>a</i>, <i>b</i>, <i>c</i></span> (<span class="tex-span">1 ≤ <i>x</i>, <i>a</i>, <i>b</i>, <i>c</i> ≤ 1000</span>) — the parameters of the random number generator. Each of the following <span class="tex-span"><i>n</i></span> lines describes one team. The description consists of the name of the team and its rating, separated by a single space. The name of a team consists of uppercase and lowercase English letters and has length from 1 to 20 characters. A team's rating is an integer from 0 to 1000. All teams' names are distinct. All team's ratings are also distinct.</p>

## Output

<p>Print the way the teams must be sorted into groups. Print the groups in the order, in which they are formed in the sorting. Number the groups by consecutive uppercase English letters, starting from letter <span class="tex-font-style-tt">'A'</span>. Inside each group print the teams' names one per line, in the order of decreasing of the teams' rating. See samples for a better understanding of the output format.</p>





```input1
8
1 3 1 7
Barcelona 158
Milan 90
Spartak 46
Anderlecht 48
Celtic 32
Benfica 87
Zenit 79
Malaga 16

```




```output1
Group A:
Barcelona
Benfica
Spartak
Celtic
Group B:
Milan
Zenit
Anderlecht
Malaga

```



## Note

<p>In the given sample the random number generator will be executed four times: </p><ul> <li> <img align="middle" class="tex-formula" src="file://zS41c65u.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> <img align="middle" class="tex-formula" src="file://rj5WcRly.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> <img align="middle" class="tex-formula" src="file://ZapJQoic.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> <img align="middle" class="tex-formula" src="file://AQQZI2Ut.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul>
