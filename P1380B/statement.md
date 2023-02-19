## Description

<div><p>Recently, you found a bot to play "Rock paper scissors" with. Unfortunately, the bot uses quite a simple algorithm to play: he has a string $s = s_1 s_2 \dots s_{n}$ of length $n$ where each letter is either <span class="tex-font-style-tt">R</span>, <span class="tex-font-style-tt">S</span> or <span class="tex-font-style-tt">P</span>.</p><p>While initializing, the bot is choosing a starting index $pos$ ($1 \le pos \le n$), and then it can play any number of rounds. In the first round, he chooses "Rock", "Scissors" or "Paper" based on the value of $s_{pos}$: </p><ul> <li> if $s_{pos}$ is equal to <span class="tex-font-style-tt">R</span> the bot chooses "Rock"; </li><li> if $s_{pos}$ is equal to <span class="tex-font-style-tt">S</span> the bot chooses "Scissors"; </li><li> if $s_{pos}$ is equal to <span class="tex-font-style-tt">P</span> the bot chooses "Paper"; </li></ul><p>In the second round, the bot's choice is based on the value of $s_{pos + 1}$. In the third round&nbsp;— on $s_{pos + 2}$ and so on. After $s_n$ the bot returns to $s_1$ and continues his game.</p><p>You plan to play $n$ rounds and you've already figured out the string $s$ but still don't know what is the starting index $pos$. But since the bot's tactic is so boring, you've decided to find $n$ choices to each round to maximize the average number of wins.</p><p>In other words, let's suggest your choices are $c_1 c_2 \dots c_n$ and if the bot starts from index $pos$ then you'll win in $win(pos)$ rounds. Find $c_1 c_2 \dots c_n$ such that $\frac{win(1) + win(2) + \dots + win(n)}{n}$ is maximum possible.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Next $t$ lines contain test cases&nbsp;— one per line. The first and only line of each test case contains string $s = s_1 s_2 \dots s_{n}$ ($1 \le n \le 2 \cdot 10^5$; $s_i \in \{\text{R}, \text{S}, \text{P}\}$)&nbsp;— the string of the bot.</p><p>It's guaranteed that the total length of all strings in one test doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print $n$ choices $c_1 c_2 \dots c_n$ to maximize the average number of wins. Print them in the same manner as the string $s$.</p><p>If there are multiple optimal answers, print any of them.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>Next $t$ lines contain test cases&nbsp;— one per line. The first and only line of each test case contains string $s = s_1 s_2 \dots s_{n}$ ($1 \le n \le 2 \cdot 10^5$; $s_i \in \{\text{R}, \text{S}, \text{P}\}$)&nbsp;— the string of the bot.</p><p>It's guaranteed that the total length of all strings in one test doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print $n$ choices $c_1 c_2 \dots c_n$ to maximize the average number of wins. Print them in the same manner as the string $s$.</p><p>If there are multiple optimal answers, print any of them.</p>





```input1
3
RRRR
RSP
S
```




```output1
PPPP
RSP
R
```



## Note

<p>In the first test case, the bot (wherever it starts) will always choose "Rock", so we can always choose "Paper". So, in any case, we will win all $n = 4$ rounds, so the average is also equal to $4$.</p><p>In the second test case: </p><ul> <li> if bot will start from $pos = 1$, then $(s_1, c_1)$ is draw, $(s_2, c_2)$ is draw and $(s_3, c_3)$ is draw, so $win(1) = 0$; </li><li> if bot will start from $pos = 2$, then $(s_2, c_1)$ is win, $(s_3, c_2)$ is win and $(s_1, c_3)$ is win, so $win(2) = 3$; </li><li> if bot will start from $pos = 3$, then $(s_3, c_1)$ is lose, $(s_1, c_2)$ is lose and $(s_2, c_3)$ is lose, so $win(3) = 0$; </li></ul> The average is equal to $\frac{0 + 3 + 0}{3} = 1$ and it can be proven that it's the maximum possible average.<p>A picture from Wikipedia explaining "Rock paper scissors" game: </p><center> <img class="tex-graphics" src="file://Bg43nx8M.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
