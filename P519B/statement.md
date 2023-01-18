## Description

<div><p><span class="tex-font-style-it">A and B are preparing themselves for programming contests.</span></p><p>B loves to debug his code. But before he runs the solution and starts debugging, he has to first compile the code.</p><p>Initially, the compiler displayed <span class="tex-span"><i>n</i></span> compilation errors, each of them is represented as a positive integer. After some effort, B managed to fix some mistake and then another one mistake.</p><p>However, despite the fact that B is sure that he corrected the two errors, he can not understand exactly what compilation errors disappeared — the compiler of the language which B uses shows errors in the new order every time! B is sure that unlike many other programming languages, compilation errors for his programming language do not depend on each other, that is, if you correct one error, the set of other error does not change.</p><p>Can you help B find out exactly what two errors he corrected?</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the initial number of compilation errors.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the errors the compiler displayed for the first time. </p><p>The third line contains <span class="tex-span"><i>n</i> - 1</span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span> — the errors displayed at the second compilation. It is guaranteed that the sequence in the third line contains all numbers of the second string except for exactly one. </p><p>The fourth line contains <span class="tex-span"><i>n</i> - 2</span> space-separated integers <span class="tex-span"><i>с</i><sub class="lower-index">1</sub>, <i>с</i><sub class="lower-index">2</sub>, ..., <i>с</i><sub class="lower-index"><i>n</i> - 2</sub></span> — the errors displayed at the third compilation. It is guaranteed that the sequence in the fourth line contains all numbers of the third line except for exactly one. </p></div><div class="output-specification"><p>Print two numbers on a single line: the numbers of the compilation errors that disappeared after B made the first and the second correction, respectively. </p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the initial number of compilation errors.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the errors the compiler displayed for the first time. </p><p>The third line contains <span class="tex-span"><i>n</i> - 1</span> space-separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span> — the errors displayed at the second compilation. It is guaranteed that the sequence in the third line contains all numbers of the second string except for exactly one. </p><p>The fourth line contains <span class="tex-span"><i>n</i> - 2</span> space-separated integers <span class="tex-span"><i>с</i><sub class="lower-index">1</sub>, <i>с</i><sub class="lower-index">2</sub>, ..., <i>с</i><sub class="lower-index"><i>n</i> - 2</sub></span> — the errors displayed at the third compilation. It is guaranteed that the sequence in the fourth line contains all numbers of the third line except for exactly one. </p>

## Output

<p>Print two numbers on a single line: the numbers of the compilation errors that disappeared after B made the first and the second correction, respectively. </p>





```input1
5
1 5 8 123 7
123 7 5 1
5 1 7

```




```input2
6
1 4 3 3 5 7
3 7 5 4 3
4 3 7 5

```




```output1
8
123

```




```output2
1
3

```



## Note

<p>In the first test sample B first corrects the error number 8, then the error number 123.</p><p>In the second test sample B first corrects the error number 1, then the error number 3. Note that if there are multiple errors with the same number, B can correct only one of them in one step. </p>
