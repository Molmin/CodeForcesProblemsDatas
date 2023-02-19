## Description

<div><p>There is a pyramid which consists of $n$ floors. The floors are numbered from top to bottom in increasing order. In the pyramid, the $i$-th floor consists of $i$ rooms.</p><p>Denote the $j$-th room on the $i$-th floor as $(i,j)$. For all positive integers $i$ and $j$ such that $1 \le j \le i &lt; n$, there are $2$ <span class="tex-font-style-bf">one-way</span> staircases which lead from $(i,j)$ to $(i+1,j)$ and from $(i,j)$ to $(i+1,j+1)$ respectively.</p><p>In each room you can either put a torch or leave it empty. Define the <span class="tex-font-style-it">brightness</span> of a room $(i, j)$ to be the number of rooms with a torch from which you can reach the room $(i, j)$ through a non-negative number of staircases.</p><p>For example, when $n=5$ and torches are placed in the rooms $(1,1)$, $(2,1)$, $(3,2)$, $(4,1)$, $(4,3)$, and $(5,3)$, the pyramid can be illustrated as follows:</p><center> <img class="tex-graphics" src="file://YM70Lnke.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center><p>In the above picture, rooms with torches are colored in yellow, and empty rooms are white. The blue numbers in the bottom-right corner indicate the brightness of the rooms.</p><p>The room $(4,2)$ (the room with a star) has brightness $3$. In the picture below, the rooms from where you can reach $(4,2)$ have red border. The brightness is $3$ since there are three torches among these rooms.</p><center> <img class="tex-graphics" src="file://FuANOCS9.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center><p>The pyramid is called <span class="tex-font-style-it">nice</span> if and only if for all floors, all rooms in the floor have the same brightness.</p><p>Define the <span class="tex-font-style-it">brilliance</span> of a nice pyramid to be the sum of brightness over the rooms $(1,1)$, $(2,1)$, $(3,1)$, ..., $(n,1)$.</p><p>Find an arrangement of torches in the pyramid, such that the resulting pyramid is nice and its brilliance is maximized.</p><p>We can show that an answer always exists. If there are multiple answers, output any one of them.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single positive integer $n$ ($1 \le n \le 500$)&nbsp;— the number of floors in the pyramid.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $500$.</p></div><div class="output-specification"><p>For each test case, output $n$ lines, the arrangement of torches in the pyramid.</p><p>The $i$-th line should contain $i$ integers, each separated with a space. The $j$-th integer on the $i$-th line should be $1$ if room $(i,j)$ has a torch, and $0$ otherwise.</p><p>We can show that an answer always exists. If there are multiple answers, output any one of them.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single positive integer $n$ ($1 \le n \le 500$)&nbsp;— the number of floors in the pyramid.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $500$.</p>

## Output

<p>For each test case, output $n$ lines, the arrangement of torches in the pyramid.</p><p>The $i$-th line should contain $i$ integers, each separated with a space. The $j$-th integer on the $i$-th line should be $1$ if room $(i,j)$ has a torch, and $0$ otherwise.</p><p>We can show that an answer always exists. If there are multiple answers, output any one of them.</p>





```input1|2,4
3
1
2
3
```




```output1
1 
1 
1 1 
1 
1 1 
1 0 1
```



## Note

<p>In the third test case, torches are placed in $(1,1)$, $(2,1)$, $(2,2)$, $(3,1)$, and $(3,3)$.</p><center> <img class="tex-graphics" src="file://GBWwumYM.png" style="max-width: 100.0%;max-height: 100.0%;" width="302px"> </center><p>The pyramid is nice as rooms on each floor have the same brightness. For example, all rooms on the third floor have brightness $3$.</p><p>The brilliance of the pyramid is $1+2+3 = 6$. It can be shown that no arrangements with $n=3$ will have a greater brilliance.</p>
