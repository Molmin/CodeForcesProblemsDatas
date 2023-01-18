## Description

<div><p>A string is called <span class="tex-font-style-it">bracket sequence</span> if it does not contain any characters other than "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>". A bracket sequence is called <span class="tex-font-style-it">regular</span> if it it is possible to obtain correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">+</span>" and "<span class="tex-font-style-tt">1</span>" into this sequence. For example, "", "<span class="tex-font-style-tt">(())</span>" and "<span class="tex-font-style-tt">()()</span>" are regular bracket sequences; "<span class="tex-font-style-tt">))</span>" and "<span class="tex-font-style-tt">)((</span>" are bracket sequences (but not regular ones), and "<span class="tex-font-style-tt">(a)</span>" and "<span class="tex-font-style-tt">(1)+(1)</span>" are not bracket sequences at all.</p><p>You have a number of strings; each string is a bracket sequence of length $2$. So, overall you have $cnt_1$ strings "<span class="tex-font-style-tt">((</span>", $cnt_2$ strings "<span class="tex-font-style-tt">()</span>", $cnt_3$ strings "<span class="tex-font-style-tt">)(</span>" and $cnt_4$ strings "<span class="tex-font-style-tt">))</span>". You want to write all these strings in some order, one after another; after that, you will get a long bracket sequence of length $2(cnt_1 + cnt_2 + cnt_3 + cnt_4)$. You wonder: is it possible to choose some order of the strings you have such that you will get a regular bracket sequence? <span class="tex-font-style-bf">Note that you may not remove any characters or strings, and you may not add anything either</span>.</p></div><div class="input-specification"><p>The input consists of four lines, $i$-th of them contains one integer $cnt_i$ ($0 \le cnt_i \le 10^9$).</p></div><div class="output-specification"><p>Print one integer: $1$ if it is possible to form a regular bracket sequence by choosing the correct order of the given strings, $0$ otherwise.</p></div>

## Input

<p>The input consists of four lines, $i$-th of them contains one integer $cnt_i$ ($0 \le cnt_i \le 10^9$).</p>

## Output

<p>Print one integer: $1$ if it is possible to form a regular bracket sequence by choosing the correct order of the given strings, $0$ otherwise.</p>





```input1
3
1
4
3
```




```input2
0
0
0
0
```




```input3
1
2
3
4
```




```output1
1
```




```output2
1
```




```output3
0
```



## Note

<p>In the first example it is possible to construct a string "<span class="tex-font-style-tt">(())()(()((()()()())))</span>", which is a regular bracket sequence.</p><p>In the second example it is possible to construct a string "", which is a regular bracket sequence.</p>
