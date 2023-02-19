## Description

<div><p>Polycarp bought a new expensive painting and decided to show it to his $n$ friends. He hung it in his room. $n$ of his friends entered and exited there one by one. At one moment there was no more than one person in the room. In other words, the first friend entered and left first, then the second, and so on.</p><p>It is known that at the beginning (before visiting friends) a picture hung in the room. At the end (after the $n$-th friend) it turned out that it disappeared. At what exact moment it disappeared&nbsp;— there is no information.</p><p>Polycarp asked his friends one by one. He asked each one if there was a picture when he entered the room. Each friend answered one of three:</p><ul> <li> <span class="tex-font-style-it">no</span> (response encoded with <span class="tex-font-style-tt">0</span>); </li><li> <span class="tex-font-style-it">yes</span> (response encoded as <span class="tex-font-style-tt">1</span>); </li><li> <span class="tex-font-style-it">can't remember</span> (response is encoded with <span class="tex-font-style-tt">?</span>). </li></ul><p>Everyone except the thief either doesn't remember or told the <span class="tex-font-style-bf">truth</span>. The thief can say anything (any of the three options).</p><p>Polycarp cannot understand who the thief is. He asks you to find out the number of those who can be considered a thief according to the answers.</p></div><div class="input-specification"><p>The first number $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the test.</p><p>The following is a description of test cases.</p><p>The first line of each test case contains one string $s$ (length does not exceed $2 \cdot 10^5$)&nbsp;— a description of the friends' answers, where $s_i$ indicates the answer of the $i$-th friend. Each character in the string is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span> or <span class="tex-font-style-tt">?</span>.</p><p>The given regularity is described in the actual situation. In particular, on the basis of answers, at least one friend can be suspected of stealing a painting.</p><p>It is guaranteed that the sum of string lengths over the entire input data set does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>Output one positive (strictly more zero) number&nbsp;– the number of people who could steal the picture based on the data shown.</p></div>

## Input

<p>The first number $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases in the test.</p><p>The following is a description of test cases.</p><p>The first line of each test case contains one string $s$ (length does not exceed $2 \cdot 10^5$)&nbsp;— a description of the friends' answers, where $s_i$ indicates the answer of the $i$-th friend. Each character in the string is either <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span> or <span class="tex-font-style-tt">?</span>.</p><p>The given regularity is described in the actual situation. In particular, on the basis of answers, at least one friend can be suspected of stealing a painting.</p><p>It is guaranteed that the sum of string lengths over the entire input data set does not exceed $2 \cdot 10^5$.</p>

## Output

<p>Output one positive (strictly more zero) number&nbsp;– the number of people who could steal the picture based on the data shown.</p>





```input1
8
0
1
1110000
?????
1?1??0?0
0?0???
??11
??0??
```




```output1
1
1
2
5
4
1
1
3
```



## Note

<p>In the first case, the answer is $1$ since we had exactly $1$ friend.</p><p>The second case is similar to the first.</p><p>In the third case, the suspects are the third and fourth friends (we count from one). It can be shown that no one else could be the thief.</p><p>In the fourth case, we know absolutely nothing, so we suspect everyone.</p>
