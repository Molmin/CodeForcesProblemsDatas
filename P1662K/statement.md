## Description

<div><p>After a long time living abroad, you have decided to move back to Italy and have to find a place to live, but things are not so easy due to the ongoing global pandemic.</p><p>Your three friends Fabio, Flavio and Francesco live at the points with coordinates $(x_1, y_1), (x_2, y_2)$ and $(x_3, y_3)$, respectively. Due to the mobility restrictions in response to the pandemic, meetings are limited to $3$ persons, so you will only be able to meet $2$ of your friends at a time. Moreover, in order to contain the spread of the infection, the authorities have imposed the following additional measure: for each meeting, the sum of the lengths travelled by each of the attendees from their residence place to the place of the meeting must not exceed $r$.</p><p>What is the minimum value of $r$ (which can be any nonnegative real number) for which there exists a place of residence that allows you to hold the three possible meetings involving you and two of your friends? Note that the chosen place of residence need not have integer coordinates.</p></div><div class="input-specification"><p>The first line contains the two integers $x_1, y_1$ ($-10^4 \le x_1, y_1 \le 10^4$) — the coordinates of the house of your friend Fabio.</p><p>The second line contains the two integers $x_2, y_2$ ($-10^4 \le x_2, y_2 \le 10^4$) — the coordinates of the house of your friend Flavio.</p><p>The third line contains the two integers $x_3, y_3$ ($-10^4 \le x_3, y_3 \le 10^4$) — the coordinates of the house of your friend Francesco.</p><p>It is guaranteed that your three friends live in different places (i.e., the three points $(x_1, y_1)$, $(x_2, y_2)$, $(x_3, y_3)$ are guaranteed to be distinct).</p></div><div class="output-specification"><p>Print the minimum value of $r$ which allows you to find a residence place satisfying the above conditions. Your answer is considered correct if its absolute or relative error does not exceed $10^{-4}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-4}$.</p></div>

## Input

<p>The first line contains the two integers $x_1, y_1$ ($-10^4 \le x_1, y_1 \le 10^4$) — the coordinates of the house of your friend Fabio.</p><p>The second line contains the two integers $x_2, y_2$ ($-10^4 \le x_2, y_2 \le 10^4$) — the coordinates of the house of your friend Flavio.</p><p>The third line contains the two integers $x_3, y_3$ ($-10^4 \le x_3, y_3 \le 10^4$) — the coordinates of the house of your friend Francesco.</p><p>It is guaranteed that your three friends live in different places (i.e., the three points $(x_1, y_1)$, $(x_2, y_2)$, $(x_3, y_3)$ are guaranteed to be distinct).</p>

## Output

<p>Print the minimum value of $r$ which allows you to find a residence place satisfying the above conditions. Your answer is considered correct if its absolute or relative error does not exceed $10^{-4}$.</p><p>Formally, let your answer be $a$, and the jury's answer be $b$. Your answer is accepted if and only if $\frac{|a - b|}{\max{(1, |b|)}} \le 10^{-4}$.</p>





```input1
0 0
5 0
3 3
```




```input2
-1 0
0 0
1 0
```




```output1
5.0686143166
```




```output2
2.0000000000
```



## Note

<p>In the <span class="tex-font-style-bf">first sample</span>, Fabio, Flavio and Francesco live at the points with coordinates $(0,0)$, $(5,0)$ and $(3,3)$ respectively. The optimal place of residence, represented by a green house in the picture below, is at the point with coordinates $(2.3842..., 0.4151...)$. </p><center> <img class="tex-graphics" src="file://qKQq0Pb4.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> For instance, it is possible for you to meet Flavio and Francesco at the point depicted below, so that the sum of the lengths travelled by the three attendees is at most (and in fact equal to) $r=5.0686...$. <center> <img class="tex-graphics" src="file://737OXflY.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the <span class="tex-font-style-bf">second sample</span>, any point on the segment $\{(x,0):\ -1 \leq x \leq 1 \}$ is an optimal place of residence.</p>
