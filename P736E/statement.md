## Description

<div><p>Ostap is preparing to play chess again and this time he is about to prepare. Thus, he was closely monitoring one recent chess tournament. There were <span class="tex-span"><i>m</i></span> players participating and each pair of players played exactly one game. The victory gives <span class="tex-span">2</span> points, draw&nbsp;— <span class="tex-span">1</span> points, lose&nbsp;— <span class="tex-span">0</span> points.</p><p>Ostap is lazy, so he never tries to remember the outcome of each game. Instead, he computes the total number of points earned by each of the players (the sum of his points in all games which he took part in), sort these value in non-ascending order and then remembers first <span class="tex-span"><i>n</i></span> integers in this list.</p><p>Now the Great Strategist Ostap wonders whether he remembers everything correct. He considers that he is correct if there exists at least one tournament results table such that it will produce the given integers. That means, if we count the sum of points for each player, sort them and take first <span class="tex-span"><i>n</i></span> elements, the result will coincide with what Ostap remembers. Can you check if such table exists?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>m</i> ≤ 3000</span>)&nbsp;— the number of participants of the tournament and the number of top results Ostap remembers.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, provided in non-ascending order&nbsp;— the number of points earned by top participants as Ostap remembers them. It's guaranteed that this integers are non-negative and do not exceed <span class="tex-span">2·<i>m</i></span>.</p></div><div class="output-specification"><p>If there is no tournament such that Ostap can obtain the given set of integers using the procedure described in the statement, then print "<span class="tex-font-style-tt">no</span>" in the only line of the output. Otherwise, the first line of the output should contain the word "<span class="tex-font-style-tt">yes</span>". Next <span class="tex-span"><i>m</i></span> lines should provide the description of any valid tournament. Each of these lines must contain <span class="tex-span"><i>m</i></span> characters '<span class="tex-font-style-tt">X</span>', '<span class="tex-font-style-tt">W</span>', '<span class="tex-font-style-tt">D</span>' and '<span class="tex-font-style-tt">L</span>'. Character '<span class="tex-font-style-tt">X</span>' should always be located on the main diagonal (and only there), that is on the <span class="tex-span"><i>i</i></span>-th position of the <span class="tex-span"><i>i</i></span>-th string. Character '<span class="tex-font-style-tt">W</span>' on the <span class="tex-span"><i>j</i></span>-th position of the <span class="tex-span"><i>i</i></span>-th string means that the <span class="tex-span"><i>i</i></span>-th player won the game against the <span class="tex-span"><i>j</i></span>-th. In the same way character '<span class="tex-font-style-tt">L</span>' means loose and '<span class="tex-font-style-tt">D</span>' means draw.</p><p>The table you print must be consistent and the points earned by best <span class="tex-span"><i>n</i></span> participants should match the memory of Ostap. If there are many possible answers, print any of them.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>m</i> ≤ 3000</span>)&nbsp;— the number of participants of the tournament and the number of top results Ostap remembers.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, provided in non-ascending order&nbsp;— the number of points earned by top participants as Ostap remembers them. It's guaranteed that this integers are non-negative and do not exceed <span class="tex-span">2·<i>m</i></span>.</p>

## Output

<p>If there is no tournament such that Ostap can obtain the given set of integers using the procedure described in the statement, then print "<span class="tex-font-style-tt">no</span>" in the only line of the output. Otherwise, the first line of the output should contain the word "<span class="tex-font-style-tt">yes</span>". Next <span class="tex-span"><i>m</i></span> lines should provide the description of any valid tournament. Each of these lines must contain <span class="tex-span"><i>m</i></span> characters '<span class="tex-font-style-tt">X</span>', '<span class="tex-font-style-tt">W</span>', '<span class="tex-font-style-tt">D</span>' and '<span class="tex-font-style-tt">L</span>'. Character '<span class="tex-font-style-tt">X</span>' should always be located on the main diagonal (and only there), that is on the <span class="tex-span"><i>i</i></span>-th position of the <span class="tex-span"><i>i</i></span>-th string. Character '<span class="tex-font-style-tt">W</span>' on the <span class="tex-span"><i>j</i></span>-th position of the <span class="tex-span"><i>i</i></span>-th string means that the <span class="tex-span"><i>i</i></span>-th player won the game against the <span class="tex-span"><i>j</i></span>-th. In the same way character '<span class="tex-font-style-tt">L</span>' means loose and '<span class="tex-font-style-tt">D</span>' means draw.</p><p>The table you print must be consistent and the points earned by best <span class="tex-span"><i>n</i></span> participants should match the memory of Ostap. If there are many possible answers, print any of them.</p>





```input1
5 5
8 6 4 2 0

```




```input2
5 1
9

```




```output1
yes
XWWWW
LXWWW
LLXWW
LLLXW
LLLLX

```




```output2
no

```


