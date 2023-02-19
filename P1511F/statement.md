## Description

<div><p>A chainword is a special type of crossword. As most of the crosswords do, it has cells that you put the letters in and some sort of hints to what these letters should be.</p><p>The letter cells in a chainword are put in a single row. We will consider chainwords of length $m$ in this task.</p><p>A hint to a chainword is a sequence of segments such that the segments don't intersect with each other and cover all $m$ letter cells. Each segment contains a description of the word in the corresponding cells.</p><p>The twist is that there are actually two hints: one sequence is the row above the letter cells and the other sequence is the row below the letter cells. When the sequences are different, they provide a way to resolve the ambiguity in the answers.</p><p>You are provided with a dictionary of $n$ words, each word consists of lowercase Latin letters. All words are pairwise distinct.</p><p>An instance of a chainword is the following triple: </p><ul> <li> a string of $m$ lowercase Latin letters; </li><li> the first hint: a sequence of segments such that the letters that correspond to each segment spell a word from the dictionary; </li><li> the second hint: another sequence of segments such that the letters that correspond to each segment spell a word from the dictionary. </li></ul><p>Note that the sequences of segments don't necessarily have to be distinct.</p><p>Two instances of chainwords are considered different if they have different strings, different first hints <span class="tex-font-style-bf">or</span> different second hints.</p><p>Count the number of different instances of chainwords. Since the number might be pretty large, output it modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 8$, $1 \le m \le 10^9$)&nbsp;— the number of words in the dictionary and the number of letter cells.</p><p>Each of the next $n$ lines contains a word&nbsp;— a non-empty string of no more than $5$ lowercase Latin letters. All words are pairwise distinct. </p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of different instances of chainwords of length $m$ for the given dictionary modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 8$, $1 \le m \le 10^9$)&nbsp;— the number of words in the dictionary and the number of letter cells.</p><p>Each of the next $n$ lines contains a word&nbsp;— a non-empty string of no more than $5$ lowercase Latin letters. All words are pairwise distinct. </p>

## Output

<p>Print a single integer&nbsp;— the number of different instances of chainwords of length $m$ for the given dictionary modulo $998\,244\,353$.</p>





```input1
3 5
ababa
ab
a
```




```input2
2 4
ab
cd
```




```input3
5 100
a
aa
aaa
aaaa
aaaaa
```




```output1
11
```




```output2
4
```




```output3
142528942
```



## Note

<p>Here are all the instances of the valid chainwords for the first example: </p><center> <img class="tex-graphics" src="file://GI5kyM6P.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The red lines above the letters denote the segments of the first hint, the blue lines below the letters denote the segments of the second hint.</p><p>In the second example the possible strings are: "<span class="tex-font-style-tt">abab</span>", "<span class="tex-font-style-tt">abcd</span>", "<span class="tex-font-style-tt">cdab</span>" and "<span class="tex-font-style-tt">cdcd</span>". All the hints are segments that cover the first two letters and the last two letters.</p>
