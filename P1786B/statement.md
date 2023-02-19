## Description

<div><p>A cake assembly line in a bakery was once again optimized, and now $n$ cakes are made at a time! In the last step, each of the $n$ cakes should be covered with chocolate.</p><p>Consider a side view on the conveyor belt, let it be a number line. The $i$-th cake occupies the segment $[a_i - w, a_i + w]$ on this line, each pair of these segments does not have common points. Above the conveyor, there are $n$ dispensers, and when a common button is pressed, chocolate from the $i$-th dispenser will cover the conveyor segment $[b_i - h, b_i + h]$. Each pair of these segments also does not have common points.</p><center> <img class="tex-graphics" src="file://tYeUo0sg.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> <span class="tex-font-size-small">Cakes and dispensers corresponding to the first example.</span> </center><p>The calibration of this conveyor belt part has not yet been performed, so you are to make it. Determine if it's possible to shift the conveyor so that each cake has some chocolate on it, and there is no chocolate outside the cakes. You can assume that the conveyour is long enough, so the cakes never fall. Also note that the button can only be pressed once.</p><center> <img class="tex-graphics" src="file://PDY5kjya.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> <span class="tex-font-size-small">In the first example we can shift the cakes as shown in the picture.</span> </center></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $w$, and $h$ ($1 \le n \le 10^5$; $1 \le w, h \le 10^5$; $h \le w$)&nbsp;— the number of cakes and dispensers, as well as the halfwidths of cakes and segments on which the chocolate is dispensed.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the positions of the cakes centers. It is guaranteed that $a_i + w &lt; a_{i + 1} - w$ for all $i$.</p><p>The third line contains $n$ integers $b_1$, $b_2$, ..., $b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the positions of the dispensers. It is guaranteed that $b_i + h &lt; b_{i + 1} - h$ for all $i$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case output "<span class="tex-font-style-tt">YES</span>", if it's possible to shift the conveyor in such a way that each cake ends up with some chocolate, and no chocolate is outside the cakes, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^5$). The description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $w$, and $h$ ($1 \le n \le 10^5$; $1 \le w, h \le 10^5$; $h \le w$)&nbsp;— the number of cakes and dispensers, as well as the halfwidths of cakes and segments on which the chocolate is dispensed.</p><p>The second line contains $n$ integers $a_1$, $a_2$, ..., $a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the positions of the cakes centers. It is guaranteed that $a_i + w &lt; a_{i + 1} - w$ for all $i$.</p><p>The third line contains $n$ integers $b_1$, $b_2$, ..., $b_n$ ($1 \le b_i \le 10^9$)&nbsp;— the positions of the dispensers. It is guaranteed that $b_i + h &lt; b_{i + 1} - h$ for all $i$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case output "<span class="tex-font-style-tt">YES</span>", if it's possible to shift the conveyor in such a way that each cake ends up with some chocolate, and no chocolate is outside the cakes, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as positive responses.</p>





```input1|2,3,4,8,9,10
4
3 10 5
65 95 165
40 65 145
5 2 1
1 6 11 16 21
4 9 14 19 24
3 3 2
13 22 29
5 16 25
4 4 1
27 36 127 136
35 50 141 144
```




```output1
YES
YES
NO
YES
```



## Note

<p>The first example is shown in the figures in the statement.</p><p>In the second example, we can move the conveyor, for example, so that the centers of the cakes are at $4, 9, 14, 19, 24$.</p><p>In the third example, we can't move the conveyor accordingly.</p>
