## Description

<div><p>Scientists are researching an impact of football match results on the mood of football fans. They have a hypothesis that there is a correlation between the number of draws and fans' desire to watch football matches in the future.</p><p>In football, two teams play a match. The teams score goals throughout a match. A score "$x$<span class="tex-font-style-tt">:</span>$y$" means that the team we observe scored $x$ goals and conceded $y$ goals. If $x = y$, then the match ends in a draw. If $x &gt; y$, then the observed team wins, and if $x &lt; y$, then it loses.</p><p>To find out if there is a correlation, the scientists gathered information about the results of teams in lower leagues. The information they found is the number of matches played by the team ($n$), the number of goals scored in these matches ($a$), and the number of goals conceded in these matches ($b$). </p><p>You are given this information for a single team. You are asked to calculate the minimum number of draws that could have happened during the team's matches and provide a list of match scores with the minimum number of draws.</p></div><div class="input-specification"><p>The first line contains an integer $n$&nbsp;— the number of matches played by the team ($1 \le n \le 100$). The second line contains an integer $a$&nbsp;— the total number of goals scored by the team in all $n$ matches ($0 \le a \le 1000$). The third line contains an integer $b$&nbsp;— the total number of goals conceded by the team in all $n$ matches ($0 \le b \le 1000$).</p></div><div class="output-specification"><p>In the first line, print a single integer $d$&nbsp;— the minimum number of draws.</p><p>In the following $n$ lines, print a list of match scores, each line in the format "$x$<span class="tex-font-style-tt">:</span>$y$", where $x$ is the number of goals scored in the match, and $y$&nbsp;– the number of goals conceded, so that exactly $d$ of these matches have ended in a draw. In case multiple such lists of match scores exist, print any of them.</p></div>

## Input

<p>The first line contains an integer $n$&nbsp;— the number of matches played by the team ($1 \le n \le 100$). The second line contains an integer $a$&nbsp;— the total number of goals scored by the team in all $n$ matches ($0 \le a \le 1000$). The third line contains an integer $b$&nbsp;— the total number of goals conceded by the team in all $n$ matches ($0 \le b \le 1000$).</p>

## Output

<p>In the first line, print a single integer $d$&nbsp;— the minimum number of draws.</p><p>In the following $n$ lines, print a list of match scores, each line in the format "$x$<span class="tex-font-style-tt">:</span>$y$", where $x$ is the number of goals scored in the match, and $y$&nbsp;– the number of goals conceded, so that exactly $d$ of these matches have ended in a draw. In case multiple such lists of match scores exist, print any of them.</p>





```input1
3
2
4
```




```input2
1
2
2
```




```input3
4
0
7
```




```input4
6
3
1
```




```output1
0
1:0
1:2
0:2
```




```output2
1
2:2
```




```output3
0
0:1
0:2
0:1
0:3
```




```output4
2
0:0
1:0
0:0
0:1
1:0
1:0
```


