## Description

<div><p>Vova is playing a computer game. There are in total $n$ turns in the game and Vova really wants to play all of them. The initial charge of his laptop battery (i.e. the charge before the start of the game) is $k$.</p><p>During each turn Vova can choose what to do: </p><ul> <li> If the current charge of his laptop battery is strictly greater than $a$, Vova can <span class="tex-font-style-it">just play</span>, and then the charge of his laptop battery will decrease by $a$; </li><li> if the current charge of his laptop battery is strictly greater than $b$ ($b&lt;a$), Vova can <span class="tex-font-style-it">play and charge</span> his laptop, and then the charge of his laptop battery will decrease by $b$; </li><li> if the current charge of his laptop battery is less than or equal to $a$ and $b$ at the same time then Vova cannot do anything and loses the game. </li></ul><p><span class="tex-font-style-bf">Regardless of Vova's turns the charge of the laptop battery is always decreases</span>.</p><p>Vova wants to complete the game (Vova can complete the game if after each of $n$ turns the charge of the laptop battery is <span class="tex-font-style-bf">strictly greater than $0$</span>). Vova has to play <span class="tex-font-style-bf">exactly $n$ turns</span>. Among all possible ways to complete the game, Vova wants to choose the one where the number of turns when he <span class="tex-font-style-it">just plays</span> (<span class="tex-font-style-bf">first type turn</span>) is the <span class="tex-font-style-bf">maximum</span> possible. It is possible that Vova cannot complete the game at all.</p><p>Your task is to find out the <span class="tex-font-style-bf">maximum</span> possible number of turns Vova can <span class="tex-font-style-it">just play</span> (make the <span class="tex-font-style-bf">first type turn</span>) or report that Vova cannot complete the game.</p><p>You have to answer $q$ independent queries.</p></div><div class="input-specification"><p>The first line of the input contains one integer $q$ ($1 \le q \le 10^5$) — the number of queries. Each query is presented by a single line.</p><p>The only line of the query contains four integers $k, n, a$ and $b$ ($1 \le k, n \le 10^9, 1 \le b &lt; a \le 10^9$) — the initial charge of Vova's laptop battery, the number of turns in the game and values $a$ and $b$, correspondingly.</p></div><div class="output-specification"><p>For each query print one integer: <span class="tex-font-style-tt">-1</span> if Vova cannot complete the game or the <span class="tex-font-style-bf">maximum</span> number of turns Vova can <span class="tex-font-style-it">just play</span> (make the <span class="tex-font-style-bf">first type turn</span>) otherwise.</p></div>

## Input

<p>The first line of the input contains one integer $q$ ($1 \le q \le 10^5$) — the number of queries. Each query is presented by a single line.</p><p>The only line of the query contains four integers $k, n, a$ and $b$ ($1 \le k, n \le 10^9, 1 \le b &lt; a \le 10^9$) — the initial charge of Vova's laptop battery, the number of turns in the game and values $a$ and $b$, correspondingly.</p>

## Output

<p>For each query print one integer: <span class="tex-font-style-tt">-1</span> if Vova cannot complete the game or the <span class="tex-font-style-bf">maximum</span> number of turns Vova can <span class="tex-font-style-it">just play</span> (make the <span class="tex-font-style-bf">first type turn</span>) otherwise.</p>





```input1
6
15 5 3 2
15 5 4 3
15 5 2 1
15 5 5 1
16 7 5 2
20 5 7 3
```




```output1
4
-1
5
2
0
1
```



## Note

<p>In the first example query Vova can <span class="tex-font-style-it">just play</span> $4$ turns and spend $12$ units of charge and then one turn <span class="tex-font-style-it">play and charge</span> and spend $2$ more units. So the remaining charge of the battery will be $1$.</p><p>In the second example query Vova cannot complete the game because even if he will <span class="tex-font-style-it">play and charge</span> the battery during each turn then the charge of the laptop battery will be $0$ after the last turn.</p>
