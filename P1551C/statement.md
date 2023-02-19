## Description

<div><p>Stephen Queen wants to write a story. He is a very unusual writer, he uses only letters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>', '<span class="tex-font-style-tt">d</span>' and '<span class="tex-font-style-tt">e</span>'!</p><p>To compose a story, Stephen wrote out $n$ words consisting of the first $5$ lowercase letters of the Latin alphabet. He wants to select the <span class="tex-font-style-bf">maximum</span> number of <span class="tex-font-style-bf">words</span> to make an <span class="tex-font-style-bf">interesting</span> story.</p><p>Let a story be a sequence of words that are not necessarily different. A story is called <span class="tex-font-style-it">interesting</span> if there exists a letter which occurs among all words of the story more times than all other letters together.</p><p>For example, the story consisting of three words "<span class="tex-font-style-tt">bac</span>", "<span class="tex-font-style-tt">aaada</span>", "<span class="tex-font-style-tt">e</span>" is interesting (the letter '<span class="tex-font-style-tt">a</span>' occurs $5$ times, all other letters occur $4$ times in total). But the story consisting of two words "<span class="tex-font-style-tt">aba</span>", "<span class="tex-font-style-tt">abcde</span>" is not (no such letter that it occurs more than all other letters in total).</p><p>You are given a sequence of $n$ words consisting of letters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>', '<span class="tex-font-style-tt">d</span>' and '<span class="tex-font-style-tt">e</span>'. Your task is to choose the maximum number of them to make an interesting story. If there's no way to make a non-empty story, output $0$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 5000$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of the words in the sequence. Then $n$ lines follow, each of them contains a word — a non-empty string consisting of lowercase letters of the Latin alphabet. The words in the sequence may be non-distinct (i. e. duplicates are allowed). Only the letters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>', '<span class="tex-font-style-tt">d</span>' and '<span class="tex-font-style-tt">e</span>' may occur in the words.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$; the sum of the lengths of all words over all test cases doesn't exceed $4 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output the maximum number of words that compose an interesting story. Print <span class="tex-font-style-tt">0</span> if there's no way to make a non-empty interesting story.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 5000$) — the number of test cases. Then $t$ test cases follow.</p><p>The first line of each test case contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$) — the number of the words in the sequence. Then $n$ lines follow, each of them contains a word — a non-empty string consisting of lowercase letters of the Latin alphabet. The words in the sequence may be non-distinct (i. e. duplicates are allowed). Only the letters '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">b</span>', '<span class="tex-font-style-tt">c</span>', '<span class="tex-font-style-tt">d</span>' and '<span class="tex-font-style-tt">e</span>' may occur in the words.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$; the sum of the lengths of all words over all test cases doesn't exceed $4 \cdot 10^5$.</p>

## Output

<p>For each test case, output the maximum number of words that compose an interesting story. Print <span class="tex-font-style-tt">0</span> if there's no way to make a non-empty interesting story.</p>





```input1
6
3
bac
aaada
e
3
aba
abcde
aba
2
baba
baba
4
ab
ab
c
bc
5
cbdca
d
a
d
e
3
b
c
ca
```




```output1
3
2
0
2
3
2
```



## Note

<p>In the first test case of the example, all $3$ words can be used to make an interesting story. The interesting story is "<span class="tex-font-style-tt">bac aaada e</span>".</p><p>In the second test case of the example, the $1$-st and the $3$-rd words can be used to make an interesting story. The interesting story is "<span class="tex-font-style-tt">aba aba</span>". Stephen can't use all three words at the same time.</p><p>In the third test case of the example, Stephen can't make a non-empty interesting story. So the answer is $0$.</p><p>In the fourth test case of the example, Stephen can use the $3$-rd and the $4$-th words to make an interesting story. The interesting story is "<span class="tex-font-style-tt">c bc</span>".</p>
