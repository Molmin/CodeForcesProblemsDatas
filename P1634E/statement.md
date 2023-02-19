## Description

<div><div class="epigraph"><div class="epigraph-text">Even a cat has things it can do that AI cannot.</div><div class="epigraph-source">— Fei-Fei Li</div></div><p>You are given $m$ arrays of positive integers. Each array is of even length.</p><p>You need to split all these integers into two <span class="tex-font-style-bf">equal</span> multisets $L$ and $R$, that is, each element of each array should go into one of two multisets (but not both). Additionally, for each of the $m$ arrays, <span class="tex-font-style-bf">exactly half</span> of its elements should go into $L$, and the rest should go into $R$.</p><p>Give an example of such a division or determine that no such division exists.</p></div><div class="input-specification"><p>The first line contains an integer $m$ ($1 \le m \le 10 ^ 5$)&nbsp;— the number of arrays.</p><p>The next $2 \cdot m$ lines contain descriptions of the arrays.</p><p>For each array, the first line contains an even integer $n$ ($2 \le n \le 2 \cdot 10 ^ 5$)&nbsp;— the length of the array. The second line consists of $n$ space-separated integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10 ^ 9$)&nbsp;— array elements.</p><p>It is guaranteed that the sum of $n$ over all arrays does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>If the answer exists, print "YES", and then print $m$ lines.</p><p>On each line, for each element, print the letter "L" or "R" (capitalized, without spaces), depending on which multiset the element should go into.</p><p>If there is no answer, print "NO" on the only line.</p></div>

## Input

<p>The first line contains an integer $m$ ($1 \le m \le 10 ^ 5$)&nbsp;— the number of arrays.</p><p>The next $2 \cdot m$ lines contain descriptions of the arrays.</p><p>For each array, the first line contains an even integer $n$ ($2 \le n \le 2 \cdot 10 ^ 5$)&nbsp;— the length of the array. The second line consists of $n$ space-separated integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10 ^ 9$)&nbsp;— array elements.</p><p>It is guaranteed that the sum of $n$ over all arrays does not exceed $2 \cdot 10^5$.</p>

## Output

<p>If the answer exists, print "YES", and then print $m$ lines.</p><p>On each line, for each element, print the letter "L" or "R" (capitalized, without spaces), depending on which multiset the element should go into.</p><p>If there is no answer, print "NO" on the only line.</p>





```input1
3
2
1 2
4
1 2 3 3
6
1 1 2 2 3 3
```




```output1
YES
RL
LRLR
RLLRRL
```



## Note

<p>In the first array, we add the first element to $R$ and the second to $L$. Now $L = \{2\}$, and $R = \{1\}$.</p><p>In the second array, we add the first and third elements to $L$ and the rest to $R$. Now $L = \{1, 2, 3\}$ and $R = \{1, 2, 3\}$.</p><p>In the third array, we add elements 2, 3, and 6 to $L$, and others&nbsp;— to $R$. As a result, $L = R = \{1, 1, 2, 2, 3, 3\}$.</p>
