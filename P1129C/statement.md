## Description

<div><p>In Morse code, an letter of English alphabet is represented as a string of some length from $1$ to $4$. Moreover, each Morse code representation of an English letter contains only dots and dashes. In this task, we will represent a dot with a "<span class="tex-font-style-tt">0</span>" and a dash with a "<span class="tex-font-style-tt">1</span>".</p><p>Because there are $2^1+2^2+2^3+2^4 = 30$ strings with length $1$ to $4$ containing only "<span class="tex-font-style-tt">0</span>" and/or "<span class="tex-font-style-tt">1</span>", not all of them correspond to one of the $26$ English letters. In particular, each string of "<span class="tex-font-style-tt">0</span>" and/or "<span class="tex-font-style-tt">1</span>" of length <span class="tex-font-style-bf">at most</span> $4$ translates into a distinct English letter, except the following four strings that do not correspond to any English alphabet: "<span class="tex-font-style-tt">0011</span>", "<span class="tex-font-style-tt">0101</span>", "<span class="tex-font-style-tt">1110</span>", and "<span class="tex-font-style-tt">1111</span>".</p><p>You will work with a string $S$, which is initially empty. For $m$ times, either a dot or a dash will be appended to $S$, one at a time. Your task is to find and report, after each of these modifications to string $S$, the number of non-empty sequences of English letters that are represented with some substring of $S$ in Morse code.</p><p>Since the answers can be incredibly tremendous, print them modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The first line contains an integer $m$ ($1 \leq m \leq 3\,000$)&nbsp;— the number of modifications to $S$. </p><p>Each of the next $m$ lines contains either a "<span class="tex-font-style-tt">0</span>" (representing a dot) or a "<span class="tex-font-style-tt">1</span>" (representing a dash), specifying which character should be appended to $S$.</p></div><div class="output-specification"><p>Print $m$ lines, the $i$-th of which being the answer after the $i$-th modification to $S$.</p></div>

## Input

<p>The first line contains an integer $m$ ($1 \leq m \leq 3\,000$)&nbsp;— the number of modifications to $S$. </p><p>Each of the next $m$ lines contains either a "<span class="tex-font-style-tt">0</span>" (representing a dot) or a "<span class="tex-font-style-tt">1</span>" (representing a dash), specifying which character should be appended to $S$.</p>

## Output

<p>Print $m$ lines, the $i$-th of which being the answer after the $i$-th modification to $S$.</p>





```input1
3
1
1
1

```




```input2
5
1
0
1
0
1

```




```input3
9
1
1
0
0
0
1
1
0
1

```




```output1
1
3
7

```




```output2
1
4
10
22
43

```




```output3
1
3
10
24
51
109
213
421
833

```



## Note

<p>Let us consider the first sample after all characters have been appended to $S$, so S is "<span class="tex-font-style-tt">111</span>".</p><p>As you can see, "<span class="tex-font-style-tt">1</span>", "<span class="tex-font-style-tt">11</span>", and "<span class="tex-font-style-tt">111</span>" all correspond to some distinct English letter. In fact, they are translated into a '<span class="tex-font-style-tt">T</span>', an '<span class="tex-font-style-tt">M</span>', and an '<span class="tex-font-style-tt">O</span>', respectively. All non-empty sequences of English letters that are represented with some substring of $S$ in Morse code, therefore, are as follows.</p><ol> <li> "<span class="tex-font-style-tt">T</span>" (translates into "<span class="tex-font-style-tt">1</span>") </li><li> "<span class="tex-font-style-tt">M</span>" (translates into "<span class="tex-font-style-tt">11</span>") </li><li> "<span class="tex-font-style-tt">O</span>" (translates into "<span class="tex-font-style-tt">111</span>") </li><li> "<span class="tex-font-style-tt">TT</span>" (translates into "<span class="tex-font-style-tt">11</span>") </li><li> "<span class="tex-font-style-tt">TM</span>" (translates into "<span class="tex-font-style-tt">111</span>") </li><li> "<span class="tex-font-style-tt">MT</span>" (translates into "<span class="tex-font-style-tt">111</span>") </li><li> "<span class="tex-font-style-tt">TTT</span>" (translates into "<span class="tex-font-style-tt">111</span>") </li></ol><p>Although unnecessary for this task, a conversion table from English alphabets into Morse code can be found <a href="https://en.wikipedia.org/wiki/Morse_code">here</a>.</p>
