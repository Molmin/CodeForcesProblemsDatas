## Description

<div><p>Polycarp came up with a new programming language. There are only two types of statements in it: </p><ul> <li> "<span class="tex-font-style-tt">x := s</span>": assign the variable named <span class="tex-font-style-tt">x</span> the value <span class="tex-font-style-tt">s</span> (where <span class="tex-font-style-tt">s</span> is a string). For example, the statement <span class="tex-font-style-tt">var := hello</span> assigns the variable named <span class="tex-font-style-tt">var</span> the value <span class="tex-font-style-tt">hello</span>. Note that <span class="tex-font-style-tt">s</span> is the value of a string, not the name of a variable. Between the variable name, the <span class="tex-font-style-tt">:=</span> operator and the string contains exactly one space each.</li><li> "<span class="tex-font-style-tt">x = a + b</span>": assign the variable named <span class="tex-font-style-tt">x</span> the concatenation of values of two variables <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">b</span>. For example, if the program consists of three statements <span class="tex-font-style-tt">a := hello</span>, <span class="tex-font-style-tt">b := world</span>, <span class="tex-font-style-tt">c = a + b</span>, then the variable <span class="tex-font-style-tt">c</span> will contain the string <span class="tex-font-style-tt">helloworld</span>. It is guaranteed that the program is correct and the variables <span class="tex-font-style-tt">a</span> and <span class="tex-font-style-tt">b</span> were previously defined. There is exactly one space between the variable names and the <span class="tex-font-style-tt">=</span> and <span class="tex-font-style-tt">+</span> operators. </li></ul><p>All variable names and strings only consist of lowercase letters of the English alphabet and do not exceed $5$ characters.</p><p>The result of the program is the number of occurrences of string <span class="tex-font-style-tt">haha</span> in the string that was written to the variable in the last statement.</p><p>Polycarp was very tired while inventing that language. He asks you to implement it. Your task is&nbsp;— for given program statements calculate the number of occurrences of string <span class="tex-font-style-tt">haha</span> in the last assigned variable.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^3$). Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 50$)&nbsp;— the number of statements in the program. All variable names and strings are guaranteed to consist only of lowercase letters of the English alphabet and do not exceed $5$ characters.</p><p>This is followed by $n$ lines describing the statements in the format described above. It is guaranteed that the program is correct.</p></div><div class="output-specification"><p>For each set of input data, output the number of occurrences of the <span class="tex-font-style-tt">haha</span> substring in the string that was written to the variable in the last statement.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^3$). Then $t$ test cases follow.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 50$)&nbsp;— the number of statements in the program. All variable names and strings are guaranteed to consist only of lowercase letters of the English alphabet and do not exceed $5$ characters.</p><p>This is followed by $n$ lines describing the statements in the format described above. It is guaranteed that the program is correct.</p>

## Output

<p>For each set of input data, output the number of occurrences of the <span class="tex-font-style-tt">haha</span> substring in the string that was written to the variable in the last statement.</p>





```input1
4
6
a := h
b := aha
c = a + b
c = c + c
e = c + c
d = a + c
15
x := haha
x = x + x
x = x + x
x = x + x
x = x + x
x = x + x
x = x + x
x = x + x
x = x + x
x = x + x
x = x + x
x = x + x
x = x + x
x = x + x
x = x + x
1
haha := hah
5
haahh := aaaha
ahhhh = haahh + haahh
haahh = haahh + haahh
ahhhh = ahhhh + haahh
ahhaa = haahh + ahhhh
```




```output1
3
32767
0
0
```



## Note

<p>In the first test case the resulting value of <span class="tex-font-style-tt">d</span> is <span class="tex-font-style-tt">hhahahaha</span>.</p>
