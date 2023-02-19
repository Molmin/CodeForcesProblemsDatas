## Description

<div><p>Monocarp has a dictionary of $n$ words, consisting of $12$ first letters of the Latin alphabet. The words are numbered from $1$ to $n$. In every pair of adjacent characters in each word, the characters are different. For every word $i$, Monocarp also has an integer $c_i$ denoting how often he uses this word.</p><p>Monocarp wants to design a keyboard that would allow him to type some of the words easily. A keyboard can be denoted as a sequence of $12$ first letters of the Latin alphabet, where each letter from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">l</span> appears exactly once.</p><p>A word can be typed with the keyboard easily if, for every pair of adjacent characters in the word, these characters are adjacent in the keyboard as well. The <span class="tex-font-style-it">optimality</span> of the keyboard is the sum of $c_i$ over all words $i$ that can be typed easily with it.</p><p>Help Monocarp to design a keyboard with the maximum possible optimality.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 1000$)&nbsp;— the number of words.</p><p>Then, $n$ lines follow. The $i$-th of them contains an integer $c_i$ ($1 \le c_i \le 10^5$) and a string $s_i$ ($2 \le |s_i| \le 2000$) denoting the $i$-th word. Each character of $s_i$ is one of $12$ first letters of Latin alphabet, in lowercase. For every $j \in [1, |s_i| - 1]$, the $j$-th character of $s_i$ is different from the $(j+1)$-th one.</p><p>Additional constraint on the input: $\sum \limits_{i=1}^{n} |s_i| \le 2000$.</p></div><div class="output-specification"><p>Print a sequence of $12$ first letters of the Latin alphabet, where each letter from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">l</span> appears exactly once, denoting the optimal keyboard. If there are multiple answers, you may print any of them.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 1000$)&nbsp;— the number of words.</p><p>Then, $n$ lines follow. The $i$-th of them contains an integer $c_i$ ($1 \le c_i \le 10^5$) and a string $s_i$ ($2 \le |s_i| \le 2000$) denoting the $i$-th word. Each character of $s_i$ is one of $12$ first letters of Latin alphabet, in lowercase. For every $j \in [1, |s_i| - 1]$, the $j$-th character of $s_i$ is different from the $(j+1)$-th one.</p><p>Additional constraint on the input: $\sum \limits_{i=1}^{n} |s_i| \le 2000$.</p>

## Output

<p>Print a sequence of $12$ first letters of the Latin alphabet, where each letter from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">l</span> appears exactly once, denoting the optimal keyboard. If there are multiple answers, you may print any of them.</p>





```input1
3
7 abacaba
10 cba
4 db
```




```input2
1
100 abca
```




```output1
hjkildbacefg
```




```output2
abcdefghijkl
```


