## Description

<div><p>Let's introduce a number system which is based on a roman digits. There are digits <span class="tex-font-style-tt">I</span>, <span class="tex-font-style-tt">V</span>, <span class="tex-font-style-tt">X</span>, <span class="tex-font-style-tt">L</span> which correspond to the numbers $1$, $5$, $10$ and $50$ respectively. The use of other roman digits is not allowed.</p><p>Numbers in this system are written as a sequence of one or more digits. We define the value of the sequence simply as the sum of digits in it.</p><p>For example, the number <span class="tex-font-style-tt">XXXV</span> evaluates to $35$ and the number <span class="tex-font-style-tt">IXI</span>&nbsp;— to $12$.</p><p>Pay attention to the difference to the traditional roman system&nbsp;— in our system any sequence of digits is valid, moreover the order of digits doesn't matter, for example <span class="tex-font-style-tt">IX</span> means $11$, not $9$.</p><p>One can notice that this system is ambiguous, and some numbers can be written in many different ways. Your goal is to determine how many distinct integers can be represented by <span class="tex-font-style-bf">exactly</span> $n$ roman digits <span class="tex-font-style-tt">I</span>, <span class="tex-font-style-tt">V</span>, <span class="tex-font-style-tt">X</span>, <span class="tex-font-style-tt">L</span>.</p></div><div class="input-specification"><p>The only line of the input file contains a single integer $n$ ($1 \le n \le 10^9$)&nbsp;— the number of roman digits to use.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the number of distinct integers which can be represented using $n$ roman digits <span class="tex-font-style-tt">exactly</span>.</p></div>

## Input

<p>The only line of the input file contains a single integer $n$ ($1 \le n \le 10^9$)&nbsp;— the number of roman digits to use.</p>

## Output

<p>Output a single integer&nbsp;— the number of distinct integers which can be represented using $n$ roman digits <span class="tex-font-style-tt">exactly</span>.</p>





```input1
1

```




```input2
2

```




```input3
10

```




```output1
4

```




```output2
10

```




```output3
244

```



## Note

<p>In the first sample there are exactly $4$ integers which can be represented&nbsp;— <span class="tex-font-style-tt">I</span>, <span class="tex-font-style-tt">V</span>, <span class="tex-font-style-tt">X</span> and <span class="tex-font-style-tt">L</span>.</p><p>In the second sample it is possible to represent integers $2$ (<span class="tex-font-style-tt">II</span>), $6$ (<span class="tex-font-style-tt">VI</span>), $10$ (<span class="tex-font-style-tt">VV</span>), $11$ (<span class="tex-font-style-tt">XI</span>), $15$ (<span class="tex-font-style-tt">XV</span>), $20$ (<span class="tex-font-style-tt">XX</span>), $51$ (<span class="tex-font-style-tt">IL</span>), $55$ (<span class="tex-font-style-tt">VL</span>), $60$ (<span class="tex-font-style-tt">XL</span>) and $100$ (<span class="tex-font-style-tt">LL</span>).</p>
