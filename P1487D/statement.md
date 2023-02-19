## Description

<div><p>A Pythagorean triple is a triple of integer numbers $(a, b, c)$ such that it is possible to form a right triangle with the lengths of the first cathetus, the second cathetus and the hypotenuse equal to $a$, $b$ and $c$, respectively. An example of the Pythagorean triple is $(3, 4, 5)$.</p><p>Vasya studies the properties of right triangles, and he uses a formula that determines if some triple of integers is Pythagorean. Unfortunately, he has forgotten the exact formula; he remembers only that the formula was some equation with squares. So, he came up with the following formula: $c = a^2 - b$.</p><p>Obviously, this is not the right formula to check if a triple of numbers is Pythagorean. But, to Vasya's surprise, it actually worked on the triple $(3, 4, 5)$: $5 = 3^2 - 4$, so, according to Vasya's formula, it is a Pythagorean triple.</p><p>When Vasya found the right formula (and understood that his formula is wrong), he wondered: how many are there triples of integers $(a, b, c)$ with $1 \le a \le b \le c \le n$ such that they are Pythagorean both according to his formula and the real definition? He asked you to count these triples.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print one integer — the number of triples of integers $(a, b, c)$ with $1 \le a \le b \le c \le n$ such that they are Pythagorean according both to the real definition and to the formula Vasya came up with.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases.</p><p>Each test case consists of one line containing one integer $n$ ($1 \le n \le 10^9$).</p>

## Output

<p>For each test case, print one integer — the number of triples of integers $(a, b, c)$ with $1 \le a \le b \le c \le n$ such that they are Pythagorean according both to the real definition and to the formula Vasya came up with.</p>





```input1
3
3
6
9
```




```output1
0
1
1
```



## Note

<p>The only Pythagorean triple satisfying $c = a^2 - b$ with $1 \le a \le b \le c \le 9$ is $(3, 4, 5)$; that's why the answer for $n = 3$ is $0$, and the answer for $n = 6$ (and for $n = 9$) is $1$.</p>
