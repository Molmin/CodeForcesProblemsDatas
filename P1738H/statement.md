## Description

<div><p>Your task is to maintain a <a href="https://en.wikipedia.org/wiki/Queue_(abstract_data_type)">queue</a> consisting of lowercase English letters as follows: </p><ul> <li> "<span class="tex-font-style-tt">push</span> $c$": insert a letter $c$ at the back of the queue; </li><li> "<span class="tex-font-style-tt">pop</span>": delete a letter from the front of the queue. </li></ul><p>Initially, the queue is empty. </p><p>After each operation, you are asked to count the number of <span class="tex-font-style-bf">distinct</span> palindromic substrings in the string that are obtained by concatenating the letters from the front to the back of the queue.</p><p>Especially, the number of distinct palindromic substrings of the empty string is $0$. </p><p>A string $s[1..n]$ of length $n$ is palindromic if $s[i] = s[n-i+1]$ for every $1 \leq i \leq n$. </p><p>The string $s[l..r]$ is a substring of string $s[1..n]$ for every $1 \leq l \leq r \leq n$. </p><p>Two strings $s[1..n]$ and $t[1..m]$ are distinct, if at least one of the following holds. </p><ul> <li> $n \neq m$; </li><li> $s[i] \neq t[i]$ for some $1 \leq i \leq \min\{n,m\}$. </li></ul></div><div class="input-specification"><p>The first line is an integer $q$ ($1 \leq q \leq 10^6$), indicating the number of operations.</p><p>Then $q$ lines follow. Each of the following lines contains one of the operations as follows. </p><ul> <li> "<span class="tex-font-style-tt">push</span> $c$": insert a letter $c$ at the back of the queue, where $c$ is a lowercase English letter; </li><li> "<span class="tex-font-style-tt">pop</span>": delete a letter from the front of the queue. </li></ul><p>It is guaranteed that no "<span class="tex-font-style-tt">pop</span>" operation will be performed when the queue is empty.</p></div><div class="output-specification"><p>After each operation, print the number of distinct palindromic substrings in the string presented in the queue. </p></div>

## Input

<p>The first line is an integer $q$ ($1 \leq q \leq 10^6$), indicating the number of operations.</p><p>Then $q$ lines follow. Each of the following lines contains one of the operations as follows. </p><ul> <li> "<span class="tex-font-style-tt">push</span> $c$": insert a letter $c$ at the back of the queue, where $c$ is a lowercase English letter; </li><li> "<span class="tex-font-style-tt">pop</span>": delete a letter from the front of the queue. </li></ul><p>It is guaranteed that no "<span class="tex-font-style-tt">pop</span>" operation will be performed when the queue is empty.</p>

## Output

<p>After each operation, print the number of distinct palindromic substrings in the string presented in the queue. </p>





```input1
12
push a
pop
push a
push a
push b
push b
push a
push a
pop
pop
pop
push b
```




```output1
1
0
1
2
3
4
5
6
5
4
3
4
```



## Note

<p>Let $s_k$ be the string presented in the queue after the $k$-th operation, and let $c_k$ be the number of distinct palindromic substrings of $s_k$. The following table shows the details of the example.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$k$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$s_k$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$c_k$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$a$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$\textsf{empty}$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$0$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$a$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$4$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$aa$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$5$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$aab$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$6$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$aabb$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$4$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$7$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$aabba$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$5$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$8$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$aabbaa$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$6$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$9$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$abbaa$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$5$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$10$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$bbaa$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$4$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$11$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$baa$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$12$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$baab$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$4$</td></tr></tbody></table> </center><p>It is worth pointing out that </p><ul> <li> After the $2$-nd operation, the string is empty and thus has no substrings. So the answer is $0$; </li><li> After the $8$-th operation, the string is "$aabbaa$". The $6$ distinct palindromic substrings are "$a$", "$aa$", "$aabbaa$", "$abba$", "$b$", and "$bb$". </li></ul>
