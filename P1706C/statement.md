## Description

<div><p><span class="tex-font-style-it">Qpwoeirut has taken up architecture and ambitiously decided to remodel his city.</span></p><p>Qpwoeirut's city can be described as a row of $n$ buildings, the $i$-th ($1 \le i \le n$) of which is $h_i$ floors high. You can assume that the height of every floor in this problem is equal. Therefore, building $i$ is taller than the building $j$ if and only if the number of floors $h_i$ in building $i$ is larger than the number of floors $h_j$ in building $j$.</p><p>Building $i$ is <span class="tex-font-style-it">cool</span> if it is taller than both building $i-1$ and building $i+1$ (and both of them exist). Note that neither the $1$-st nor the $n$-th building can be cool.</p><p>To remodel the city, Qpwoeirut needs to maximize the number of cool buildings. To do this, Qpwoeirut can build additional floors on top of any of the buildings to make them taller. Note that he cannot remove already existing floors.</p><p>Since building new floors is expensive, Qpwoeirut wants to minimize the number of floors he builds. Find the minimum number of floors Qpwoeirut needs to build in order to maximize the number of cool buildings.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($3 \le n \le 10^5$)&nbsp;— the number of buildings in Qpwoeirut's city.</p><p>The second line of each test case contains $n$ integers $h_1, h_2, \ldots, h_n$ ($1 \le h_i \le 10^9$)&nbsp;— the number of floors in each of the buildings of the city.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;— the minimum number of additional floors Qpwoeirut needs to build in order to maximize the number of cool buildings.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains the single integer $n$ ($3 \le n \le 10^5$)&nbsp;— the number of buildings in Qpwoeirut's city.</p><p>The second line of each test case contains $n$ integers $h_1, h_2, \ldots, h_n$ ($1 \le h_i \le 10^9$)&nbsp;— the number of floors in each of the buildings of the city.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;— the minimum number of additional floors Qpwoeirut needs to build in order to maximize the number of cool buildings.</p>





```input1|2,3,6,7,10,11
6
3
2 1 2
5
1 2 1 4 3
6
3 1 4 5 5 2
8
4 2 1 3 5 3 6 1
6
1 10 1 1 10 1
8
1 10 11 1 10 11 10 1
```




```output1
2
0
3
3
0
4
```



## Note

<p>In the first test case, it is optimal for Qpwoeirut to make the second building cool by building $2$ additional floors on top of it, making it taller than both of its adjacent buildings. The final heights of buildings will be $[2, \underline{3}, 2]$.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://zf8CQVp3.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://MpfMwNDj.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td><img class="tex-graphics" src="file://WPKic3S2.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> </center><p>In the second test case, the number of cool buildings is already maximized, so Qpwoeirut does not need to do anything.</p><p>In the third test case, it is optimal for Qpwoeirut to make the third and fifth buildings cool by building $2$ additional floors onto the third building and $1$ additional floor onto the fifth building. The final heights of buildings will be $[3, 1, \underline{6}, 5, \underline{6}, 2]$.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://1dJ69B9V.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://RR7mt45l.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td><img class="tex-graphics" src="file://CXTCAC6w.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> </center><p>It can be shown that it is impossible to make more than $2$ of the buildings cool, or to make $2$ buildings cool using fewer than $3$ additional floors.</p><p>In the fourth test case, Qpwoeirut can either make the second building cool, or he can make the third building cool. Either way, he will be building $3$ additional floors and maximizing the number of cool buildings. The final heights of buildings will be $[4, 2, \underline{4}, 3, 5, 3, 6, 1]$ or $[4, \underline{5}, 1, 3, 5, 3, 6, 1]$.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://AO3Ltzel.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td class="tex-tabular-text-align-center"><img class="tex-graphics" src="file://uhSVYQSt.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td><img class="tex-graphics" src="file://PD6YAq0k.png" style="max-width: 100.0%;max-height: 100.0%;"></td><td><img class="tex-graphics" src="file://a0VQvnrG.png" style="max-width: 100.0%;max-height: 100.0%;"></td></tr></tbody></table> </center>
