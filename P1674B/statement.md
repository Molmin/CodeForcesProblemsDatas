## Description

<div><p>The Berland language consists of words having <span class="tex-font-style-bf">exactly two letters</span>. Moreover, <span class="tex-font-style-bf">the first letter of a word is different from the second letter</span>. Any combination of two different Berland letters (which, by the way, are the same as the lowercase letters of Latin alphabet) is a correct word in Berland language.</p><p>The Berland dictionary contains all words of this language. The words are listed in a way they are usually ordered in dictionaries. Formally, word $a$ comes earlier than word $b$ in the dictionary if one of the following conditions hold:</p><ul> <li> the first letter of $a$ is less than the first letter of $b$; </li><li> the first letters of $a$ and $b$ are the same, and the second letter of $a$ is less than the second letter of $b$. </li></ul><p>So, the dictionary looks like that:</p><ul> <li> Word $1$: <span class="tex-font-style-tt">ab</span> </li><li> Word $2$: <span class="tex-font-style-tt">ac</span> </li><li> ... </li><li> Word $25$: <span class="tex-font-style-tt">az</span> </li><li> Word $26$: <span class="tex-font-style-tt">ba</span> </li><li> Word $27$: <span class="tex-font-style-tt">bc</span> </li><li> ... </li><li> Word $649$: <span class="tex-font-style-tt">zx</span> </li><li> Word $650$: <span class="tex-font-style-tt">zy</span> </li></ul><p>You are given a word $s$ from the Berland language. Your task is to find its index in the dictionary.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 650$)&nbsp;— the number of test cases.</p><p>Each test case consists of one line containing $s$&nbsp;— a string consisting of <span class="tex-font-style-bf">exactly two different lowercase Latin letters</span> (i. e. a correct word of the Berland language).</p></div><div class="output-specification"><p>For each test case, print one integer&nbsp;— the index of the word $s$ in the dictionary.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 650$)&nbsp;— the number of test cases.</p><p>Each test case consists of one line containing $s$&nbsp;— a string consisting of <span class="tex-font-style-bf">exactly two different lowercase Latin letters</span> (i. e. a correct word of the Berland language).</p>

## Output

<p>For each test case, print one integer&nbsp;— the index of the word $s$ in the dictionary.</p>





```input1
7
ab
ac
az
ba
bc
zx
zy
```




```output1
1
2
25
26
27
649
650
```


