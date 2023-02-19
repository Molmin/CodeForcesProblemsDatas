## Description

<div><p>Anna is a girl so brave that she is loved by everyone in the city and citizens love her cookies. She is planning to hold a party with cookies. Now she has $a$ vanilla cookies and $b$ chocolate cookies for the party.</p><p>She invited $n$ guests of the first type and $m$ guests of the second type to the party. They will come to the party in some order. After coming to the party, each guest will choose the type of cookie (vanilla or chocolate) to eat. There is a difference in the way how they choose that type:</p><p>If there are $v$ vanilla cookies and $c$ chocolate cookies at the moment, when the guest comes, then</p><ul> <li> if the guest of the first type: if $v&gt;c$ the guest selects a <span class="tex-font-style-bf">vanilla</span> cookie. Otherwise, the guest selects a <span class="tex-font-style-bf">chocolate</span> cookie. </li><li> if the guest of the second type: if $v&gt;c$ the guest selects a <span class="tex-font-style-bf">chocolate</span> cookie. Otherwise, the guest selects a <span class="tex-font-style-bf">vanilla</span> cookie. </li></ul><p>After that:</p><ul> <li> If there is at least one cookie of the selected type, the guest eats one. </li><li> Otherwise (there are no cookies of the selected type), the guest gets angry and returns to home. </li></ul><p>Anna wants to know if there exists some order of guests, such that <span class="tex-font-style-bf">no one guest gets angry</span>. Your task is to answer her question.</p></div><div class="input-specification"><p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Next $t$ lines contain descriptions of test cases.</p><p>For each test case, the only line contains four integers $a$, $b$, $n$, $m$ ($0 \le a,b,n,m \le 10^{18}, n+m \neq 0$).</p></div><div class="output-specification"><p>For each test case, print the answer in one line. If there exists at least one valid order, print "<span class="tex-font-style-tt">Yes</span>". Otherwise, print "<span class="tex-font-style-tt">No</span>".</p><p>You can print each letter in any case (upper or lower).</p></div>

## Input

<p>The input consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases. Next $t$ lines contain descriptions of test cases.</p><p>For each test case, the only line contains four integers $a$, $b$, $n$, $m$ ($0 \le a,b,n,m \le 10^{18}, n+m \neq 0$).</p>

## Output

<p>For each test case, print the answer in one line. If there exists at least one valid order, print "<span class="tex-font-style-tt">Yes</span>". Otherwise, print "<span class="tex-font-style-tt">No</span>".</p><p>You can print each letter in any case (upper or lower).</p>





```input1
6
2 2 1 2
0 100 0 1
12 13 25 1
27 83 14 25
0 0 1 0
1000000000000000000 1000000000000000000 1000000000000000000 1000000000000000000
```




```output1
Yes
No
No
Yes
No
Yes
```



## Note

<p>In the first test case, let's consider the order $\{1, 2, 2\}$ of types of guests. Then:</p><ul> <li> The first guest eats a chocolate cookie. After that, there are $2$ vanilla cookies and $1$ chocolate cookie. </li><li> The second guest eats a chocolate cookie. After that, there are $2$ vanilla cookies and $0$ chocolate cookies. </li><li> The last guest selects a chocolate cookie, but there are no chocolate cookies. So, the guest gets angry. </li></ul><p>So, this order can't be chosen by Anna.</p><p>Let's consider the order $\{2, 2, 1\}$ of types of guests. Then:</p><ul> <li> The first guest eats a vanilla cookie. After that, there is $1$ vanilla cookie and $2$ chocolate cookies. </li><li> The second guest eats a vanilla cookie. After that, there are $0$ vanilla cookies and $2$ chocolate cookies. </li><li> The last guest eats a chocolate cookie. After that, there are $0$ vanilla cookies and $1$ chocolate cookie. </li></ul><p>So, the answer to this test case is "<span class="tex-font-style-tt">Yes</span>".</p><p>In the fifth test case, it is illustrated, that the number of cookies ($a + b$) can be equal to zero, but the number of guests ($n + m$) can't be equal to zero.</p><p>In the sixth test case, be careful about the overflow of $32$-bit integer type.</p>
