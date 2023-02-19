## Description

<div><p>Joseph really likes the culture of Japan. Last year he learned Japanese traditional clothes and visual arts and now he is trying to find out the secret of the Japanese game called Nonogram.</p><p>In the one-dimensional version of the game, there is a row of $n$ empty cells, some of which are to be filled with a pen. There is a description of a solution called a <span class="tex-font-style-underline">profile</span>&nbsp;— a sequence of positive integers denoting the lengths of consecutive sets of filled cells. For example, the profile of $[4, 3, 1]$ means that there are sets of four, three, and one filled cell, in that order, with at least one empty cell between successive sets.</p><center> <img class="tex-graphics" src="file://5woMzRJD.png" style="max-width: 100.0%;max-height: 100.0%;"><p>A suitable solution for $n = 12$ and $p = [4, 3, 1]$. </p></center><center> <img class="tex-graphics" src="file://DZSOZrBI.png" style="max-width: 100.0%;max-height: 100.0%;"><p>A wrong solution: the first four filled cells should be consecutive. </p></center><center> <img class="tex-graphics" src="file://NmnLFtpX.png" style="max-width: 100.0%;max-height: 100.0%;"><p>A wrong solution: there should be at least one empty cell before the last filled cell. </p></center><p>Joseph found out that for some numbers $n$ and profiles $p$ there are lots of ways to fill the cells to satisfy the profile. Now he is in the process of solving a nonogram consisting of $n$ cells and a profile $p$. He has already created a <span class="tex-font-style-underline">mask</span> of $p$&nbsp;— he has filled all the cells that must be filled in every solution of the nonogram.</p><center> <img class="tex-graphics" src="file://psIewIOs.png" style="max-width: 100.0%;max-height: 100.0%;"><p>The mask for $n = 12$ and $p = [4, 3, 1]$: all the filled cells above are filled in every solution. </p></center><p>After a break, he lost the source profile $p$. He only has $n$ and the mask $m$. Help Joseph find any profile $p'$ with the mask $m$ or say that there is no such profile and Joseph has made a mistake.</p></div><div class="input-specification"><p>The only line contains a string $m$&nbsp;— the mask of the source profile $p$. The length of $m$ is $n$ ($1 \le n \le 100\,000$). The string $m$ consists of symbols <span class="tex-font-style-tt">#</span> and <span class="tex-font-style-tt">_</span>&nbsp;— denoting filled and empty cells respectively.</p></div><div class="output-specification"><p>If there is no profile with the mask $m$, output the number $-1$. Otherwise, on the first line, output an integer $k$&nbsp;— the number of integers in the profile $p'$. On the second line, output $k$ integers of the profile $p'$.</p></div>

## Input

<p>The only line contains a string $m$&nbsp;— the mask of the source profile $p$. The length of $m$ is $n$ ($1 \le n \le 100\,000$). The string $m$ consists of symbols <span class="tex-font-style-tt">#</span> and <span class="tex-font-style-tt">_</span>&nbsp;— denoting filled and empty cells respectively.</p>

## Output

<p>If there is no profile with the mask $m$, output the number $-1$. Otherwise, on the first line, output an integer $k$&nbsp;— the number of integers in the profile $p'$. On the second line, output $k$ integers of the profile $p'$.</p>





```input1
__#_____
```




```input2
_#
```




```input3
___
```




```output1
2
3 2
```




```output2
-1
```




```output3
0
```


