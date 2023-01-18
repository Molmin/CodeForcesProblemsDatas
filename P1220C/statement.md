## Description

<div><p>Mike and Ann are sitting in the classroom. The lesson is boring, so they decided to play an interesting game. Fortunately, all they need to play this game is a string $s$ and a number $k$ ($0 \le k &lt; |s|$).</p><p>At the beginning of the game, players are given a substring of $s$ with left border $l$ and right border $r$, both equal to $k$ (i.e. initially $l=r=k$). Then players start to make moves one by one, according to the following rules:</p><ul><li> A player chooses $l^{\prime}$ and $r^{\prime}$ so that $l^{\prime} \le l$, $r^{\prime} \ge r$ and $s[l^{\prime}, r^{\prime}]$ is lexicographically less than $s[l, r]$. Then the player changes $l$ and $r$ in this way: $l := l^{\prime}$, $r := r^{\prime}$.</li><li> Ann moves first.</li><li> The player, that can't make a move loses.</li></ul><p>Recall that a substring $s[l, r]$ ($l \le r$) of a string $s$ is a continuous segment of letters from s that starts at position $l$ and ends at position $r$. For example, "<span class="tex-font-style-tt">ehn</span>" is a substring ($s[3, 5]$) of "<span class="tex-font-style-tt">aaaehnsvz</span>" and "<span class="tex-font-style-tt">ahz</span>" is not.</p><p>Mike and Ann were playing so enthusiastically that they did not notice the teacher approached them. Surprisingly, the teacher didn't scold them, instead of that he said, that he can figure out the winner of the game before it starts, even if he knows only $s$ and $k$.</p><p>Unfortunately, Mike and Ann are not so keen in the game theory, so they ask you to write a program, that takes $s$ and determines the winner for all possible $k$.</p></div><div class="input-specification"><p>The first line of the input contains a single string $s$ ($1 \leq |s| \leq 5 \cdot 10^5$) consisting of lowercase English letters.</p></div><div class="output-specification"><p>Print $|s|$ lines.</p><p>In the line $i$ write the name of the winner (print <span class="tex-font-style-tt">Mike</span> or <span class="tex-font-style-tt">Ann</span>) in the game with string $s$ and $k = i$, if both play optimally</p></div>

## Input

<p>The first line of the input contains a single string $s$ ($1 \leq |s| \leq 5 \cdot 10^5$) consisting of lowercase English letters.</p>

## Output

<p>Print $|s|$ lines.</p><p>In the line $i$ write the name of the winner (print <span class="tex-font-style-tt">Mike</span> or <span class="tex-font-style-tt">Ann</span>) in the game with string $s$ and $k = i$, if both play optimally</p>





```input1
abba
```




```input2
cba
```




```output1
Mike
Ann
Ann
Mike
```




```output2
Mike
Mike
Mike
```


