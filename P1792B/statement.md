## Description

<div><p>Eve is a beginner stand-up comedian. Her first show gathered a grand total of two spectators: Alice and Bob.</p><p>Eve prepared $a_1 + a_2 + a_3 + a_4$ jokes to tell, grouped by their type: </p><ul> <li> type 1: both Alice and Bob like them; </li><li> type 2: Alice likes them, but Bob doesn't; </li><li> type 3: Bob likes them, but Alice doesn't; </li><li> type 4: neither Alice nor Bob likes them. </li></ul><p>Initially, both spectators have their mood equal to $0$. When a spectator hears a joke he/she likes, his/her mood increases by $1$. When a spectator hears a joke he/she doesn't like, his/her mood decreases by $1$. If the mood of a spectator becomes negative (strictly below zero), he/she leaves.</p><p>When someone leaves, Eve gets sad and ends the show. If no one leaves, and Eve is out of jokes, she also ends the show.</p><p>Thus, Eve wants to arrange her jokes in such a way that the show lasts as long as possible. Help her to calculate the maximum number of jokes she can tell before the show ends.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains four integers $a_1, a_2, a_3, a_4$ ($0 \le a_1, a_2, a_3, a_4 \le 10^8$; $a_1 + a_2 + a_3 + a_4 \ge 1$)&nbsp;— the number of jokes of each type Eve prepared.</p></div><div class="output-specification"><p>For each testcase, print a single integer&nbsp;— the maximum number of jokes Eve can tell before at least one of the spectators leaves or before she runs out of jokes.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>The only line of each testcase contains four integers $a_1, a_2, a_3, a_4$ ($0 \le a_1, a_2, a_3, a_4 \le 10^8$; $a_1 + a_2 + a_3 + a_4 \ge 1$)&nbsp;— the number of jokes of each type Eve prepared.</p>

## Output

<p>For each testcase, print a single integer&nbsp;— the maximum number of jokes Eve can tell before at least one of the spectators leaves or before she runs out of jokes.</p>





```input1|2,4
4
5 0 0 0
0 0 0 5
2 5 10 6
3 0 0 7
```




```output1
5
1
15
7
```



## Note

<p>In the first testcase, Eve only has jokes of the first type. Thus, there's no order to choose. She tells all her jokes, both Alice and Bob like them. Their mood becomes $5$. The show ends after Eve runs out of jokes.</p><p>In the second testcase, Eve only has jokes of the fourth type. Thus, once again no order to choose. She tells a joke, and neither Alice, nor Bob likes it. Their mood decrease by one, becoming $-1$. They both have negative mood, thus, both leave, and the show ends.</p><p>In the third testcase, first, Eve tells both jokes of the first type. Both Alice and Bob has mood $2$. Then she can tell $2$ jokes of the third type. Alice's mood becomes $0$. Bob's mood becomes $4$. Then $4$ jokes of the second type. Alice's mood becomes $4$. Bob's mood becomes $0$. Then another $4$ jokes of the third type. Alice's mood becomes $0$. Bob's mood becomes $4$. Then the remaining joke of the second type. Alice's mood becomes $1$. Bob's mood becomes $3$. Then one more joke of the third type, and a joke of the fourth type, for example. Alice's mood becomes $-1$, she leaves, and the show ends. </p><p>In the fourth testcase, Eve should first tell the jokes both spectators like, then the jokes they don't. She can tell $4$ jokes of the fourth type until the spectators leave.</p>
