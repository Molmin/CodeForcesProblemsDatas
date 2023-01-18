## Description

<div><p>Balph is learning to play a game called Buma. In this game, he is given a row of colored balls. He has to choose the color of one new ball and the place to insert it (between two balls, or to the left of all the balls, or to the right of all the balls).</p><p>When the ball is inserted the following happens repeatedly: if some segment of balls of the same color became longer as a result of a previous action and its length became at least $3$, then all the balls of this segment are eliminated. </p><p>Consider, for example, a row of balls '<span class="tex-font-style-tt">AAABBBWWBB</span>'. Suppose Balph chooses a ball of color '<span class="tex-font-style-tt">W</span>' and the place to insert it after the sixth ball, i.&nbsp;e. to the left of the two '<span class="tex-font-style-tt">W</span>'s. After Balph inserts this ball, the balls of color '<span class="tex-font-style-tt">W</span>' are eliminated, since this segment was made longer and has length $3$ now, so the row becomes '<span class="tex-font-style-tt">AAABBBBB</span>'. The balls of color '<span class="tex-font-style-tt">B</span>' are eliminated now, because the segment of balls of color '<span class="tex-font-style-tt">B</span>' became longer and has length $5$ now. Thus, the row becomes '<span class="tex-font-style-tt">AAA</span>'. However, none of the balls are eliminated now, because there is no elongated segment.</p><p>Help Balph count the number of possible ways to choose a color of a new ball and a place to insert it that leads to the elimination of all the balls.</p></div><div class="input-specification"><p>The only line contains a non-empty string of uppercase English letters of length at most $3 \cdot 10^5$. Each letter represents a ball with the corresponding color.</p></div><div class="output-specification"><p>Output the number of ways to choose a color and a position of a new ball in order to eliminate all the balls.</p></div>

## Input

<p>The only line contains a non-empty string of uppercase English letters of length at most $3 \cdot 10^5$. Each letter represents a ball with the corresponding color.</p>

## Output

<p>Output the number of ways to choose a color and a position of a new ball in order to eliminate all the balls.</p>





```input1
BBWWBB
```




```input2
BWWB
```




```input3
BBWBB
```




```input4
OOOWWW
```




```input5
WWWOOOOOOWWW
```




```output1
3
```




```output2
0
```




```output3
0
```




```output4
0
```




```output5
7
```


