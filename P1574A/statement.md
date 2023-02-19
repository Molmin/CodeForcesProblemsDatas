## Description

<div><p>A bracket sequence is a string containing only characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>". A regular bracket sequence is a bracket sequence that can be transformed into a correct arithmetic expression by inserting characters "<span class="tex-font-style-tt">1</span>" and "<span class="tex-font-style-tt">+</span>" between the original characters of the sequence. For example, bracket sequences "<span class="tex-font-style-tt">()()</span>" and "<span class="tex-font-style-tt">(())</span>" are regular (the resulting expressions are: "<span class="tex-font-style-tt">(1)+(1)</span>" and "<span class="tex-font-style-tt">((1+1)+1)</span>"), and "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" are not.</p><p>You are given an integer $n$. Your goal is to construct and print <span class="tex-font-style-bf">exactly $n$</span> different regular bracket sequences of length $2n$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 50$) — the number of test cases.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n \le 50$).</p></div><div class="output-specification"><p>For each test case, print $n$ lines, each containing a regular bracket sequence of length <span class="tex-font-style-bf">exactly $2n$</span>. All bracket sequences you output for a testcase should be different (though they may repeat in different test cases). If there are multiple answers, print any of them. It can be shown that it's always possible.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 50$) — the number of test cases.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n \le 50$).</p>

## Output

<p>For each test case, print $n$ lines, each containing a regular bracket sequence of length <span class="tex-font-style-bf">exactly $2n$</span>. All bracket sequences you output for a testcase should be different (though they may repeat in different test cases). If there are multiple answers, print any of them. It can be shown that it's always possible.</p>





```input1
3
3
1
3
```




```output1
()()()
((()))
(()())
()
((()))
(())()
()(())
```


