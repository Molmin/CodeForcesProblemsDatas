## Description

<div><p>Bob recently read about bitwise operations used in computers: <span class="tex-font-style-tt">AND</span>, <span class="tex-font-style-tt">OR</span> and <span class="tex-font-style-tt">XOR</span>. He have studied their properties and invented a new game.</p><p>Initially, Bob chooses integer <span class="tex-span"><i>m</i></span>, bit depth of the game, which means that all numbers in the game will consist of <span class="tex-span"><i>m</i></span> bits. Then he asks Peter to choose some <span class="tex-span"><i>m</i></span>-bit number. After that, Bob computes the values of <span class="tex-span"><i>n</i></span> variables. Each variable is assigned either a constant <span class="tex-span"><i>m</i></span>-bit number or result of bitwise operation. Operands of the operation may be either variables defined before, or the number, chosen by Peter. After that, Peter's score equals to the sum of all variable values.</p><p>Bob wants to know, what number Peter needs to choose to get the minimum possible score, and what number he needs to choose to get the maximum possible score. In both cases, if there are several ways to get the same score, find the minimum number, which he can choose.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, the number of variables and bit depth, respectively (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>; <span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>). </p><p>The following <span class="tex-span"><i>n</i></span> lines contain descriptions of the variables. Each line describes exactly one variable. Description has the following format: name of a new variable, space, sign "<span class="tex-font-style-tt">:=</span>", space, followed by one of:</p><ol> <li> Binary number of exactly <span class="tex-span"><i>m</i></span> bits. </li><li> The first operand, space, bitwise operation ("<span class="tex-font-style-tt">AND</span>", "<span class="tex-font-style-tt">OR</span>" or "<span class="tex-font-style-tt">XOR</span>"), space, the second operand. Each operand is either the name of variable defined before or symbol '<span class="tex-font-style-tt">?</span>', indicating the number chosen by Peter. </li></ol> <p>Variable names are strings consisting of lowercase Latin letters with length at most 10. All variable names are different.</p></div><div class="output-specification"><p>In the first line output the minimum number that should be chosen by Peter, to make the sum of all variable values minimum possible, in the second line output the minimum number that should be chosen by Peter, to make the sum of all variable values maximum possible. Both numbers should be printed as <span class="tex-span"><i>m</i></span>-bit binary numbers.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, the number of variables and bit depth, respectively (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>; <span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>). </p><p>The following <span class="tex-span"><i>n</i></span> lines contain descriptions of the variables. Each line describes exactly one variable. Description has the following format: name of a new variable, space, sign "<span class="tex-font-style-tt">:=</span>", space, followed by one of:</p><ol> <li> Binary number of exactly <span class="tex-span"><i>m</i></span> bits. </li><li> The first operand, space, bitwise operation ("<span class="tex-font-style-tt">AND</span>", "<span class="tex-font-style-tt">OR</span>" or "<span class="tex-font-style-tt">XOR</span>"), space, the second operand. Each operand is either the name of variable defined before or symbol '<span class="tex-font-style-tt">?</span>', indicating the number chosen by Peter. </li></ol> <p>Variable names are strings consisting of lowercase Latin letters with length at most 10. All variable names are different.</p>

## Output

<p>In the first line output the minimum number that should be chosen by Peter, to make the sum of all variable values minimum possible, in the second line output the minimum number that should be chosen by Peter, to make the sum of all variable values maximum possible. Both numbers should be printed as <span class="tex-span"><i>m</i></span>-bit binary numbers.</p>





```input1
3 3
a := 101
b := 011
c := ? XOR b

```




```input2
5 1
a := 1
bb := 0
cx := ? OR a
d := ? XOR ?
e := d AND bb

```




```output1
011
100

```




```output2
0
0

```



## Note

<p>In the first sample if Peter chooses a number <span class="tex-span">011<sub class="lower-index">2</sub></span>, then <span class="tex-span"><i>a</i> = 101<sub class="lower-index">2</sub>, <i>b</i> = 011<sub class="lower-index">2</sub>, <i>c</i> = 000<sub class="lower-index">2</sub></span>, the sum of their values is <span class="tex-span">8</span>. If he chooses the number <span class="tex-span">100<sub class="lower-index">2</sub></span>, then <span class="tex-span"><i>a</i> = 101<sub class="lower-index">2</sub>, <i>b</i> = 011<sub class="lower-index">2</sub>, <i>c</i> = 111<sub class="lower-index">2</sub></span>, the sum of their values is <span class="tex-span">15</span>.</p><p>For the second test, the minimum and maximum sum of variables <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>bb</i></span>, <span class="tex-span"><i>cx</i></span>, <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>e</i></span> is 2, and this sum doesn't depend on the number chosen by Peter, so the minimum Peter can choose is <span class="tex-span">0</span>.</p>
