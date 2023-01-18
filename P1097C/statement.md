## Description

<div><p>One day, Yuhao came across a problem about checking if some bracket sequences are correct bracket sequences.</p><p>A bracket sequence is any non-empty sequence of opening and closing parentheses. A bracket sequence is called a <span class="tex-font-style-it">correct bracket sequence</span> if it's possible to obtain a correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">1</span>" into this sequence. For example, the sequences "<span class="tex-font-style-tt">(())()</span>", "<span class="tex-font-style-tt">()</span>" and "<span class="tex-font-style-tt">(()(()))</span>" are correct, while the bracket sequences "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(()</span>" and "<span class="tex-font-style-tt">(()))(</span>" are not correct.</p><p>Yuhao found this problem too simple for him so he decided to make the problem harder. You are given many (not necessarily correct) bracket sequences. The task is to connect some of them into ordered pairs so that each bracket sequence occurs in at most one pair and the concatenation of the bracket sequences in each pair is a correct bracket sequence. The goal is to create as many pairs as possible.</p><p>This problem unfortunately turned out to be too difficult for Yuhao. Can you help him and solve it?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \leq n \leq 10^5$) — the number of bracket sequences.</p><p>Each of the following $n$ lines contains one bracket sequence — a non-empty string which consists only of characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>".</p><p>The sum of lengths of all bracket sequences in the input is at most $5 \cdot 10^5$.</p><p>Note that a bracket sequence may appear in the input multiple times. In this case, you can use each copy of the sequence separately. Also note that the order in which strings appear in the input doesn't matter.</p></div><div class="output-specification"><p>Print a single integer — the maximum number of pairs which can be made, adhering to the conditions in the statement.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \leq n \leq 10^5$) — the number of bracket sequences.</p><p>Each of the following $n$ lines contains one bracket sequence — a non-empty string which consists only of characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>".</p><p>The sum of lengths of all bracket sequences in the input is at most $5 \cdot 10^5$.</p><p>Note that a bracket sequence may appear in the input multiple times. In this case, you can use each copy of the sequence separately. Also note that the order in which strings appear in the input doesn't matter.</p>

## Output

<p>Print a single integer — the maximum number of pairs which can be made, adhering to the conditions in the statement.</p>





```input1
7
)())
)
((
((
(
)
)
```




```input2
4
(
((
(((
(())
```




```input3
2
(())
()
```




```output1
2
```




```output2
0
```




```output3
1
```



## Note

<p>In the first example, it's optimal to construct two pairs: "<span class="tex-font-style-tt">(( &nbsp;&nbsp;&nbsp; )())</span>" and "<span class="tex-font-style-tt">( &nbsp;&nbsp;&nbsp; )</span>".</p>
