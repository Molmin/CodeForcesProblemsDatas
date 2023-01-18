## Description

<div><p><span class="tex-font-style-it">This problem differs from the previous one only in the absence of the constraint on the equal length of all numbers $a_1, a_2, \dots, a_n$.</span></p><p>A team of SIS students is going to make a trip on a submarine. Their target is an ancient treasure in a sunken ship lying on the bottom of the Great Rybinsk sea. Unfortunately, the students don't know the coordinates of the ship, so they asked Meshanya (who is a hereditary mage) to help them. He agreed to help them, but only if they solve his problem.</p><p>Let's denote a function that alternates digits of two numbers $f(a_1 a_2 \dots a_{p - 1} a_p, b_1 b_2 \dots b_{q - 1} b_q)$, where $a_1 \dots a_p$ and $b_1 \dots b_q$ are digits of two integers written in the decimal notation without leading zeros.</p><p>In other words, the function $f(x, y)$ alternately shuffles the digits of the numbers $x$ and $y$ by writing them from the lowest digits to the older ones, starting with the number $y$. The result of the function is also built from right to left (that is, from the lower digits to the older ones). If the digits of one of the arguments have ended, then the remaining digits of the other argument are written out. Familiarize with examples and formal definitions of the function below.</p><p>For example: $$f(1111, 2222) = 12121212$$ $$f(7777, 888) = 7787878$$ $$f(33, 44444) = 4443434$$ $$f(555, 6) = 5556$$ $$f(111, 2222) = 2121212$$</p><p>Formally,</p><ul> <li> if $p \ge q$ then $f(a_1 \dots a_p, b_1 \dots b_q) = a_1 a_2 \dots a_{p - q + 1} b_1 a_{p - q + 2} b_2 \dots a_{p - 1} b_{q - 1} a_p b_q$; </li><li> if $p &lt; q$ then $f(a_1 \dots a_p, b_1 \dots b_q) = b_1 b_2 \dots b_{q - p} a_1 b_{q - p + 1} a_2 \dots a_{p - 1} b_{q - 1} a_p b_q$. </li></ul><p>Mishanya gives you an array consisting of $n$ integers $a_i$, your task is to help students to calculate $\sum_{i = 1}^{n}\sum_{j = 1}^{n} f(a_i, a_j)$ modulo $998\,244\,353$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $n$ ($1 \le n \le 100\,000$) — the number of elements in the array. The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) — the elements of the array.</p></div><div class="output-specification"><p>Print the answer modulo $998\,244\,353$.</p></div>

## Input

<p>The first line of the input contains a single integer $n$ ($1 \le n \le 100\,000$) — the number of elements in the array. The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$) — the elements of the array.</p>

## Output

<p>Print the answer modulo $998\,244\,353$.</p>





```input1
3
12 3 45
```




```input2
2
123 456
```




```output1
12330
```




```output2
1115598
```


