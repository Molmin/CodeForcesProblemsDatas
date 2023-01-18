## Description

<div><p>On the 228-th international Uzhlyandian Wars strategic game tournament teams from each country are called. The teams should consist of <span class="tex-span">5</span> participants.</p><p>The team of Uzhlyandia will consist of soldiers, because there are no gamers.</p><p>Masha is a new minister of defense and gaming. The prime duty of the minister is to calculate the efficiency of the Uzhlandian army. The army consists of <span class="tex-span"><i>n</i></span> soldiers standing in a row, enumerated from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. For each soldier we know his <span class="tex-font-style-it">skill</span> in Uzhlyandian Wars: the <span class="tex-span"><i>i</i></span>-th soldier's skill is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>It was decided that the team will consist of three players and two assistants. The skills of players should be same, and the assistants' skills should not be greater than the players' skill. Moreover, it is important for Masha that one of the assistants should stand in the row to the left of the players, and the other one should stand in the row to the right of the players. Formally, a team is five soldiers with indexes <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>p</i></span>, such that <span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> &lt; <i>k</i> &lt; <i>l</i> &lt; <i>p</i> ≤ <i>n</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> = <i>a</i><sub class="lower-index"><i>k</i></sub> = <i>a</i><sub class="lower-index"><i>l</i></sub> ≥ <i>a</i><sub class="lower-index"><i>p</i></sub></span>. </p><p>The efficiency of the army is the number of different teams Masha can choose. Two teams are considered different if there is such <span class="tex-span"><i>i</i></span> such that the <span class="tex-span"><i>i</i></span>-th soldier is a member of one team, but not a member of the other team.</p><p>Initially, all players are able to be players. For some reasons, sometimes some soldiers become unable to be players. Sometimes some soldiers, that were unable to be players, become able to be players. At any time any soldier is able to be an assistant. Masha wants to control the efficiency of the army, so she asked you to tell her the number of different possible teams modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>) after each change. </p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of soldiers in Uzhlyandia.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the soldiers' skills.</p><p>The third line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of changes.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the changes, each change is described with two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 2</span>, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>) on a separate line. If <span class="tex-span"><i>t</i> = 1</span>, then the <span class="tex-span"><i>x</i></span>-th soldier is unable to be a player after this change. If <span class="tex-span"><i>t</i> = 2</span>, then the <span class="tex-span"><i>x</i></span>-th soldier is able to be a player after this change. </p><p>It is guaranteed that before each query of the first type the soldier is able to be a player, and before each query of the second type the soldier is unable to be a player.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> integers&nbsp;— the number of distinct teams after each change.</p><p>Print the answers modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). </p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of soldiers in Uzhlyandia.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the soldiers' skills.</p><p>The third line contains single integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of changes.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the changes, each change is described with two integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 2</span>, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>) on a separate line. If <span class="tex-span"><i>t</i> = 1</span>, then the <span class="tex-span"><i>x</i></span>-th soldier is unable to be a player after this change. If <span class="tex-span"><i>t</i> = 2</span>, then the <span class="tex-span"><i>x</i></span>-th soldier is able to be a player after this change. </p><p>It is guaranteed that before each query of the first type the soldier is able to be a player, and before each query of the second type the soldier is unable to be a player.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> integers&nbsp;— the number of distinct teams after each change.</p><p>Print the answers modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>). </p>





```input1
6
1 1 1 1 1 1
2
1 3
2 3

```




```input2
8
3 4 4 2 4 5 4 1
3
1 5
2 5
1 2

```




```output1
1
6

```




```output2
1
6
2

```



## Note

<p>In the first example, after the first change the only team consists of soldiers <span class="tex-span">[1, 2, 4, 5, 6]</span>. After the second change any five soldiers can form a team.</p><p>In the first example after the first change the only team is soldiers <span class="tex-span">[1, 2, 3, 7, 8]</span>. After the second change the possible teams are: <span class="tex-span">[1, 2, 3, 5, 7]</span>, <span class="tex-span">[1, 2, 3, 5, 8]</span>, <span class="tex-span">[1, 2, 3, 7, 8]</span>, <span class="tex-span">[1, 2, 5, 7, 8]</span>, <span class="tex-span">[1, 3, 5, 7, 8]</span>, <span class="tex-span">[2, 3, 5, 7, 8]</span>. After the third change the possible teams are: <span class="tex-span">[1, 3, 5, 7, 8]</span>, <span class="tex-span">[2, 3, 5, 7, 8]</span>.</p>
