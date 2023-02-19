## Description

<div><p>Bertown is a city with $n$ buildings in a straight line.</p><p>The city's security service discovered that some buildings were mined. A map was compiled, which is a string of length $n$, where the $i$-th character is "<span class="tex-font-style-tt">1</span>" if there is a mine under the building number $i$ and "<span class="tex-font-style-tt">0</span>" otherwise.</p><p>Bertown's best sapper knows how to activate mines so that the buildings above them are not damaged. When a mine under the building numbered $x$ is activated, it explodes and activates two adjacent mines under the buildings numbered $x-1$ and $x+1$ (if there were no mines under the building, then nothing happens). Thus, it is enough to activate any one mine on a continuous segment of mines to activate all the mines of this segment. For manual activation of one mine, the sapper takes $a$ coins. He can repeat this operation as many times as you want.</p><p>Also, a sapper can place a mine under a building if it wasn't there. For such an operation, he takes $b$ coins. He can also repeat this operation as many times as you want.</p><p>The sapper can carry out operations in any order.</p><p>You want to blow up all the mines in the city to make it safe. Find the minimum number of coins that the sapper will have to pay so that after his actions there are no mines left in the city.</p></div><div class="input-specification"><p>The first line contains one positive integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case begins with a line containing two integers $a$ and $b$ ($1 \le a, b \le 1000$)&nbsp;— the cost of activating and placing one mine, respectively.</p><p>The next line contains a map of mines in the city&nbsp;— a string consisting of zeros and ones.</p><p>The sum of the string lengths for all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, output one integer&nbsp;— the minimum number of coins that the sapper will have to pay.</p></div>

## Input

<p>The first line contains one positive integer $t$ ($1 \le t \le 10^5$)&nbsp;— the number of test cases. Then $t$ test cases follow.</p><p>Each test case begins with a line containing two integers $a$ and $b$ ($1 \le a, b \le 1000$)&nbsp;— the cost of activating and placing one mine, respectively.</p><p>The next line contains a map of mines in the city&nbsp;— a string consisting of zeros and ones.</p><p>The sum of the string lengths for all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, output one integer&nbsp;— the minimum number of coins that the sapper will have to pay.</p>





```input1
2
1 1
01000010
5 1
01101110
```




```output1
2
6
```



## Note

<p>In the second test case, if we place a mine under the fourth building and then activate it, then all mines on the field are activated. The cost of such operations is six, $b=1$ coin for placing a mine and $a=5$ coins for activating.</p>
