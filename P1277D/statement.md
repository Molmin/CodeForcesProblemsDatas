## Description

<div><p>Polycarp has $n$ <span class="tex-font-style-bf">different</span> binary words. A word called binary if it contains only characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'. For example, these words are binary: "<span class="tex-font-style-tt">0001</span>", "<span class="tex-font-style-tt">11</span>", "<span class="tex-font-style-tt">0</span>" and "<span class="tex-font-style-tt">0011100</span>".</p><p>Polycarp wants to offer his set of $n$ binary words to play a game "words". In this game, players name words and each next word (starting from the second) must start with the last character of the previous word. The first word can be any. For example, these sequence of words can be named during the game: "<span class="tex-font-style-tt">0101</span>", "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">10</span>", "<span class="tex-font-style-tt">00</span>", "<span class="tex-font-style-tt">00001</span>".</p><p>Word reversal is the operation of reversing the order of the characters. For example, the word "<span class="tex-font-style-tt">0111</span>" after the reversal becomes "<span class="tex-font-style-tt">1110</span>", the word "<span class="tex-font-style-tt">11010</span>" after the reversal becomes "<span class="tex-font-style-tt">01011</span>".</p><p>Probably, Polycarp has such a set of words that there is no way to put them in the order correspondent to the game rules. In this situation, he wants to reverse some words from his set so that:</p><ul> <li> the final set of $n$ words still contains <span class="tex-font-style-bf">different</span> words (i.e. all words are unique); </li><li> there is a way to put all words of the final set of words in the order so that the final sequence of $n$ words is consistent with the game rules. </li></ul><p>Polycarp wants to reverse minimal number of words. Please, help him.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>The first line of a test case contains one integer $n$ ($1 \le n \le 2\cdot10^5$) — the number of words in the Polycarp's set. Next $n$ lines contain these words. All of $n$ words aren't empty and contains only characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'. The sum of word lengths doesn't exceed $4\cdot10^6$. All words are <span class="tex-font-style-bf">different</span>.</p><p>Guaranteed, that the sum of $n$ for all test cases in the input doesn't exceed $2\cdot10^5$. Also, guaranteed that the sum of word lengths for all test cases in the input doesn't exceed $4\cdot10^6$.</p></div><div class="output-specification"><p>Print answer for all of $t$ test cases in the order they appear.</p><p>If there is no answer for the test case, print <span class="tex-font-style-tt">-1</span>. Otherwise, the first line of the output should contain $k$ ($0 \le k \le n$) — the minimal number of words in the set which should be reversed. The second line of the output should contain $k$ distinct integers — the indexes of the words in the set which should be reversed. Words are numerated from $1$ to $n$ in the order they appear. If $k=0$ you can skip this line (or you can print an empty line). If there are many answers you can print any of them.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>The first line of a test case contains one integer $n$ ($1 \le n \le 2\cdot10^5$) — the number of words in the Polycarp's set. Next $n$ lines contain these words. All of $n$ words aren't empty and contains only characters '<span class="tex-font-style-tt">0</span>' and '<span class="tex-font-style-tt">1</span>'. The sum of word lengths doesn't exceed $4\cdot10^6$. All words are <span class="tex-font-style-bf">different</span>.</p><p>Guaranteed, that the sum of $n$ for all test cases in the input doesn't exceed $2\cdot10^5$. Also, guaranteed that the sum of word lengths for all test cases in the input doesn't exceed $4\cdot10^6$.</p>

## Output

<p>Print answer for all of $t$ test cases in the order they appear.</p><p>If there is no answer for the test case, print <span class="tex-font-style-tt">-1</span>. Otherwise, the first line of the output should contain $k$ ($0 \le k \le n$) — the minimal number of words in the set which should be reversed. The second line of the output should contain $k$ distinct integers — the indexes of the words in the set which should be reversed. Words are numerated from $1$ to $n$ in the order they appear. If $k=0$ you can skip this line (or you can print an empty line). If there are many answers you can print any of them.</p>





```input1
4
4
0001
1000
0011
0111
3
010
101
0
2
00000
00001
4
01
001
0001
00001
```




```output1
1
3 
-1
0

2
1 2
```


