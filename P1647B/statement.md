## Description

<div><p>Madoka's father just reached $1$ million subscribers on Mathub! So the website decided to send him a personalized award&nbsp;— The Mathhub's Bit Button! </p><p>The Bit Button is a rectangular table with $n$ rows and $m$ columns with $0$ or $1$ in each cell. After exploring the table Madoka found out that:</p><ul><li> A subrectangle $A$ is contained in a subrectangle $B$ if there's no cell contained in $A$ but not contained in $B$.</li><li> Two subrectangles intersect if there is a cell contained in both of them.</li><li> A subrectangle is called <span class="tex-font-style-bf">black</span> if there's no cell with value $0$ inside it.</li><li> A subrectangle is called <span class="tex-font-style-bf">nice</span> if it's <span class="tex-font-style-bf">black</span> and it's not contained in another <span class="tex-font-style-bf">black</span> subrectangle.</li><li> The table is called <span class="tex-font-style-bf">elegant</span> if there are no two <span class="tex-font-style-bf">nice</span> intersecting subrectangles.</li></ul><p>For example, in the first illustration the red subrectangle is nice, but in the second one it's not, because it's contained in the purple subrectangle.</p><center> <img class="tex-graphics" height="215px" src="file://FJJJM2Or.png" style="max-width: 100.0%;max-height: 100.0%;" width="567px"> </center><p>Help Madoka to determine whether the table is elegant.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 200$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two positive integers $n, m$ ($1 \le n, m \le 100$).</p><p>The next $n$ lines contain strings of length $m$ consisting of zeros and ones&nbsp;— the description of the table.</p><p>It is guaranteed that the sum of the values of $n$ and the sum of the values of $m$ for all test cases do not exceed $777$.</p></div><div class="output-specification"><p>For each test case print "<span class="tex-font-style-tt">YES</span>" if its table is elegant or print "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may print each letter in any case (for example, "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">Yes</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">yEs</span>" will all be recognized as positive answer).</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 200$)&nbsp;— the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains two positive integers $n, m$ ($1 \le n, m \le 100$).</p><p>The next $n$ lines contain strings of length $m$ consisting of zeros and ones&nbsp;— the description of the table.</p><p>It is guaranteed that the sum of the values of $n$ and the sum of the values of $m$ for all test cases do not exceed $777$.</p>

## Output

<p>For each test case print "<span class="tex-font-style-tt">YES</span>" if its table is elegant or print "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You may print each letter in any case (for example, "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">Yes</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">yEs</span>" will all be recognized as positive answer).</p>





```input1
5
3 3
100
011
011
3 3
110
111
110
1 5
01111
4 5
11111
01010
01000
01000
3 2
11
00
11
```




```output1
YES
NO
YES
NO
YES
```



## Note

<p>In the second test case the table is not elegant, because the red and the purple subrectangles are nice and intersect. </p><center> <img class="tex-graphics" height="215px" src="file://57Ch4952.png" style="max-width: 100.0%;max-height: 100.0%;" width="215px"> </center><p>In the fourth test case the table is not elegant, because the red and the purple subrectangles are nice and intersect. </p><center> <img class="tex-graphics" height="215px" src="file://uvhezvSY.png" style="max-width: 100.0%;max-height: 100.0%;" width="265px"> </center>
