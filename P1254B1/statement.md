## Description

<div><p><span class="tex-font-style-it">This is the easier version of the problem. In this version, $1 \le n \le 10^5$ and $0 \le a_i \le 1$. You can hack this problem only if you solve and lock both problems.</span></p><p>Christmas is coming, and our protagonist, Bob, is preparing a spectacular present for his long-time best friend Alice. This year, he decides to prepare $n$ boxes of chocolate, numbered from $1$ to $n$. Initially, the $i$-th box contains $a_i$ chocolate pieces.</p><p>Since Bob is a typical nice guy, he will not send Alice $n$ empty boxes. In other words, <span class="tex-font-style-bf">at least one of $a_1, a_2, \ldots, a_n$ is positive</span>. Since Alice dislikes coprime sets, she will be happy only if there exists some integer $k &gt; 1$ such that the number of pieces in each box is divisible by $k$. Note that Alice won't mind if there exists some empty boxes. </p><p>Charlie, Alice's boyfriend, also is Bob's second best friend, so he decides to help Bob by rearranging the chocolate pieces. In one second, Charlie can pick up a piece in box $i$ and put it into either box $i-1$ or box $i+1$ (if such boxes exist). Of course, he wants to help his friend as quickly as possible. Therefore, he asks you to calculate the minimum number of seconds he would need to make Alice happy.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of chocolate boxes.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 1$)&nbsp;— the number of chocolate pieces in the $i$-th box.</p><p>It is guaranteed that at least one of $a_1, a_2, \ldots, a_n$ is positive.</p></div><div class="output-specification"><p>If there is no way for Charlie to make Alice happy, print $-1$.</p><p>Otherwise, print a single integer $x$&nbsp;— the minimum number of seconds for Charlie to help Bob make Alice happy.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of chocolate boxes.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 1$)&nbsp;— the number of chocolate pieces in the $i$-th box.</p><p>It is guaranteed that at least one of $a_1, a_2, \ldots, a_n$ is positive.</p>

## Output

<p>If there is no way for Charlie to make Alice happy, print $-1$.</p><p>Otherwise, print a single integer $x$&nbsp;— the minimum number of seconds for Charlie to help Bob make Alice happy.</p>





```input1
3
1 0 1
```




```input2
1
1
```




```output1
2
```




```output2
-1
```


