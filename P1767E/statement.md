## Description

<div><div class="epigraph"><div class="epigraph-text"> <span class="tex-font-style-it">Algebra Flash 2.2 has just been released!</span><p><span class="tex-font-style-it">Changelog:</span></p><ul> <li> New gamemode! </li></ul><p><span class="tex-font-style-it">Thank you for the continued support of the game!</span> </p></div></div><p>Huh, is that it? Slightly disappointed, you boot up the game and click on the new gamemode. It says "<span class="tex-font-style-tt">Colored platforms</span>".</p><p>There are $n$ platforms, numbered from $1$ to $n$, placed one after another. There are $m$ colors available in the game, numbered from $1$ to $m$. The $i$-th platform is colored $c_i$.</p><p>You start on the platform $1$ and want to reach platform $n$. In one move, you can jump from some platform $i$ to platforms $i + 1$ or $i + 2$.</p><p>All platforms are initially deactivated (including platforms $1$ and $n$). For each color $j$, you can pay $x_j$ coins to activate all platforms of that color.</p><p>You want to activate some platforms so that you could start on an activated platform $1$, jump through some activated platforms and reach an activated platform $n$.</p><p>What's the smallest amount of coins you can spend to achieve that?</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2 \le n \le 3 \cdot 10^5$; $1 \le m \le 40$)&nbsp;— the number of platforms and the number of colors, respectively.</p><p>The second line contains $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le m$)&nbsp;— the colors of the platforms.</p><p>The third line contains $m$ integers $x_1, x_2, \dots, x_m$ ($1 \le x_i \le 10^7$)&nbsp;— the cost of activating all platforms of each color.</p></div><div class="output-specification"><p>Print the smallest amount of coins you can spend to activate some platforms so that you could start on an activated platform $1$, jump through some activated platforms and reach an activated platform $n$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2 \le n \le 3 \cdot 10^5$; $1 \le m \le 40$)&nbsp;— the number of platforms and the number of colors, respectively.</p><p>The second line contains $n$ integers $c_1, c_2, \dots, c_n$ ($1 \le c_i \le m$)&nbsp;— the colors of the platforms.</p><p>The third line contains $m$ integers $x_1, x_2, \dots, x_m$ ($1 \le x_i \le 10^7$)&nbsp;— the cost of activating all platforms of each color.</p>

## Output

<p>Print the smallest amount of coins you can spend to activate some platforms so that you could start on an activated platform $1$, jump through some activated platforms and reach an activated platform $n$.</p>





```input1
5 3
1 3 2 3 1
1 10 100
```




```input2
5 3
1 3 2 3 1
1 200 20
```




```input3
4 2
2 2 1 1
5 5
```




```input4
10 10
3 8 6 2 10 5 2 3 7 3
9 7 4 2 1 8 2 6 2 2
```




```output1
11
```




```output2
21
```




```output3
10
```




```output4
15
```


