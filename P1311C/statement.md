## Description

<div><p>You want to perform the combo on your opponent in one popular fighting game. The combo is the string $s$ consisting of $n$ lowercase Latin letters. To perform the combo, you have to press all buttons in the order they appear in $s$. I.e. if $s=$"<span class="tex-font-style-tt">abca</span>" then you have to press '<span class="tex-font-style-tt">a</span>', then '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>' and '<span class="tex-font-style-tt">a</span>' again.</p><p>You know that you will spend $m$ wrong tries to perform the combo and during the $i$-th try you will make a mistake right after $p_i$-th button ($1 \le p_i &lt; n$) (i.e. you will press first $p_i$ buttons right and start performing the combo from the beginning). It is guaranteed that during the $m+1$-th try you press all buttons right and finally perform the combo.</p><p>I.e. if $s=$"<span class="tex-font-style-tt">abca</span>", $m=2$ and $p = [1, 3]$ then the sequence of pressed buttons will be '<span class="tex-font-style-tt">a</span>' (<span class="tex-font-style-bf">here</span> you're making a mistake and start performing the combo from the beginning), '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>', (<span class="tex-font-style-bf">here</span> you're making a mistake and start performing the combo from the beginning), '<span class="tex-font-style-tt">a</span>' (<span class="tex-font-style-bf">note that at this point you will not perform the combo because of the mistake</span>), '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>', '<span class="tex-font-style-tt">a</span>'.</p><p>Your task is to calculate for each button (letter) the number of times you'll press it.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m \le 2 \cdot 10^5$) — the length of $s$ and the number of tries correspondingly.</p><p>The second line of each test case contains the string $s$ consisting of $n$ lowercase Latin letters.</p><p>The third line of each test case contains $m$ integers $p_1, p_2, \dots, p_m$ ($1 \le p_i &lt; n$) — the number of characters pressed right during the $i$-th try.</p><p>It is guaranteed that the sum of $n$ and the sum of $m$ both does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$, $\sum m \le 2 \cdot 10^5$).</p><p>It is guaranteed that the answer for each letter does not exceed $2 \cdot 10^9$.</p></div><div class="output-specification"><p>For each test case, print the answer — $26$ integers: the number of times you press the button '<span class="tex-font-style-tt">a</span>', the number of times you press the button '<span class="tex-font-style-tt">b</span>', $\dots$, the number of times you press the button '<span class="tex-font-style-tt">z</span>'.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \le n \le 2 \cdot 10^5$, $1 \le m \le 2 \cdot 10^5$) — the length of $s$ and the number of tries correspondingly.</p><p>The second line of each test case contains the string $s$ consisting of $n$ lowercase Latin letters.</p><p>The third line of each test case contains $m$ integers $p_1, p_2, \dots, p_m$ ($1 \le p_i &lt; n$) — the number of characters pressed right during the $i$-th try.</p><p>It is guaranteed that the sum of $n$ and the sum of $m$ both does not exceed $2 \cdot 10^5$ ($\sum n \le 2 \cdot 10^5$, $\sum m \le 2 \cdot 10^5$).</p><p>It is guaranteed that the answer for each letter does not exceed $2 \cdot 10^9$.</p>

## Output

<p>For each test case, print the answer — $26$ integers: the number of times you press the button '<span class="tex-font-style-tt">a</span>', the number of times you press the button '<span class="tex-font-style-tt">b</span>', $\dots$, the number of times you press the button '<span class="tex-font-style-tt">z</span>'.</p>





```input1
3
4 2
abca
1 3
10 5
codeforces
2 8 3 2 9
26 10
qwertyuioplkjhgfdsazxcvbnm
20 10 1 2 3 5 10 5 9 4
```




```output1
4 2 2 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 
0 0 9 4 5 3 0 0 0 0 0 0 0 0 9 0 0 3 1 0 0 0 0 0 0 0 
2 1 1 2 9 2 2 2 5 2 2 2 1 1 5 4 11 8 2 7 5 1 10 1 5 2
```



## Note

<p>The first test case is described in the problem statement. Wrong tries are "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">abc</span>" and the final try is "<span class="tex-font-style-tt">abca</span>". The number of times you press '<span class="tex-font-style-tt">a</span>' is $4$, '<span class="tex-font-style-tt">b</span>' is $2$ and '<span class="tex-font-style-tt">c</span>' is $2$.</p><p>In the second test case, there are five wrong tries: "<span class="tex-font-style-tt">co</span>", "<span class="tex-font-style-tt">codeforc</span>", "<span class="tex-font-style-tt">cod</span>", "<span class="tex-font-style-tt">co</span>", "<span class="tex-font-style-tt">codeforce</span>" and the final try is "<span class="tex-font-style-tt">codeforces</span>". The number of times you press '<span class="tex-font-style-tt">c</span>' is $9$, '<span class="tex-font-style-tt">d</span>' is $4$, '<span class="tex-font-style-tt">e</span>' is $5$, '<span class="tex-font-style-tt">f</span>' is $3$, '<span class="tex-font-style-tt">o</span>' is $9$, '<span class="tex-font-style-tt">r</span>' is $3$ and '<span class="tex-font-style-tt">s</span>' is $1$.</p>
