## Description

<div><p>You have $c_1$ letters '<span class="tex-font-style-tt">a</span>', $c_2$ letters '<span class="tex-font-style-tt">b</span>', ..., $c_{26}$ letters '<span class="tex-font-style-tt">z</span>'. You want to build a <span class="tex-font-style-it">beautiful</span> string of length $n$ from them (obviously, you cannot use the $i$-th letter more than $c_i$ times). <span class="tex-font-style-bf">Each $c_i$ is greater than $\frac{n}{3}$</span>.</p><p>A string is called <span class="tex-font-style-it">beautiful</span> if there are no palindromic contiguous substrings of odd length greater than $1$ in it. For example, the string "<span class="tex-font-style-tt">abacaba</span>" is not beautiful, it has several palindromic substrings of odd length greater than $1$ (for example, "<span class="tex-font-style-tt">aca</span>"). Another example: the string "<span class="tex-font-style-tt">abcaa</span>" is <span class="tex-font-style-it">beautiful</span>.</p><p>Calculate the number of different strings you can build, and print the answer modulo $998244353$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($3 \le n \le 400$).</p><p>The second line contains $26$ integers $c_1$, $c_2$, ..., $c_{26}$ ($\frac{n}{3} &lt; c_i \le n$).</p></div><div class="output-specification"><p>Print one integer — the number of strings you can build, taken modulo $998244353$.</p></div>

## Input

<p>The first line contains one integer $n$ ($3 \le n \le 400$).</p><p>The second line contains $26$ integers $c_1$, $c_2$, ..., $c_{26}$ ($\frac{n}{3} &lt; c_i \le n$).</p>

## Output

<p>Print one integer — the number of strings you can build, taken modulo $998244353$.</p>





```input1
4
2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2 2
```




```input2
3
2 2 2 2 2 2 3 3 3 2 2 2 2 2 2 3 3 3 2 2 3 2 2 3 2 2
```




```input3
400
348 322 247 158 209 134 151 267 268 176 214 379 372 291 388 135 147 304 169 149 193 351 380 368 181 340
```




```output1
422500
```




```output2
16900
```




```output3
287489790
```


