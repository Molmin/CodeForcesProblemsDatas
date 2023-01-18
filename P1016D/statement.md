## Description

<div><p>Now Vasya is taking an exam in mathematics. In order to get a good mark, Vasya needs to guess the matrix that the teacher has constructed!</p><p>Vasya knows that the matrix consists of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns. For each row, he knows the xor (bitwise excluding or) of the elements in this row. The sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> denotes the xor of elements in rows with indices <span class="tex-span">1</span>, <span class="tex-span">2</span>, ..., <span class="tex-span"><i>n</i></span>, respectively. Similarly, for each column, he knows the xor of the elements in this column. The sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> denotes the xor of elements in columns with indices <span class="tex-span">1</span>, <span class="tex-span">2</span>, ..., <span class="tex-span"><i>m</i></span>, respectively.</p><p>Help Vasya! Find a matrix satisfying the given constraints or tell him that there is no suitable matrix.</p></div><div class="input-specification"><p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i>&nbsp;(2 ≤ <i>n</i>, <i>m</i> ≤ 100)</span> — the dimensions of the matrix.</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>&nbsp;(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the xor of all elements in row <span class="tex-span"><i>i</i></span>.</p><p>The third line contains <span class="tex-span"><i>m</i></span> numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub>&nbsp;(0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the xor of all elements in column <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>If there is no matrix satisfying the given constraints in the first line, output "NO".</p><p>Otherwise, on the first line output "YES", and then <span class="tex-span"><i>n</i></span> rows of <span class="tex-span"><i>m</i></span> numbers in each <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>1</sub>, <i>c</i><sub class="lower-index"><i>i</i>2</sub>, ... , <i>c</i><sub class="lower-index"><i>im</i></sub>&nbsp;(0 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 2·10<sup class="upper-index">9</sup>)</span> — the description of the matrix.</p><p>If there are several suitable matrices, it is allowed to print any of them.</p></div>

## Input

<p>The first line contains two numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i>&nbsp;(2 ≤ <i>n</i>, <i>m</i> ≤ 100)</span> — the dimensions of the matrix.</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>&nbsp;(0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the xor of all elements in row <span class="tex-span"><i>i</i></span>.</p><p>The third line contains <span class="tex-span"><i>m</i></span> numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub>&nbsp;(0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the xor of all elements in column <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>If there is no matrix satisfying the given constraints in the first line, output "NO".</p><p>Otherwise, on the first line output "YES", and then <span class="tex-span"><i>n</i></span> rows of <span class="tex-span"><i>m</i></span> numbers in each <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>1</sub>, <i>c</i><sub class="lower-index"><i>i</i>2</sub>, ... , <i>c</i><sub class="lower-index"><i>im</i></sub>&nbsp;(0 ≤ <i>c</i><sub class="lower-index"><i>ij</i></sub> ≤ 2·10<sup class="upper-index">9</sup>)</span> — the description of the matrix.</p><p>If there are several suitable matrices, it is allowed to print any of them.</p>





```input1
2 3
2 9
5 3 13

```




```input2
3 3
1 7 6
2 15 12

```




```output1
YES
3 4 5
6 7 8

```




```output2
NO

```


