## Description

<div><p>There are $n$ consecutive seat places in a railway carriage. Each place is either empty or occupied by a passenger.</p><p>The university team for the Olympiad consists of $a$ student-programmers and $b$ student-athletes. Determine the largest number of students from all $a+b$ students, which you can put in the railway carriage so that:</p><ul> <li> no student-programmer is sitting next to the student-programmer; </li><li> and no student-athlete is sitting next to the student-athlete. </li></ul><p>In the other words, there should not be two consecutive (adjacent) places where two student-athletes or two student-programmers are sitting.</p><p>Consider that initially occupied seat places are occupied by jury members (who obviously are not students at all).</p></div><div class="input-specification"><p>The first line contain three integers $n$, $a$ and $b$ ($1 \le n \le 2\cdot10^{5}$, $0 \le a, b \le 2\cdot10^{5}$, $a + b &gt; 0$) — total number of seat places in the railway carriage, the number of student-programmers and the number of student-athletes.</p><p>The second line contains a string with length $n$, consisting of characters "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">*</span>". The dot means that the corresponding place is empty. The asterisk means that the corresponding place is occupied by the jury member.</p></div><div class="output-specification"><p>Print the largest number of students, which you can put in the railway carriage so that no student-programmer is sitting next to a student-programmer and no student-athlete is sitting next to a student-athlete.</p></div>

## Input

<p>The first line contain three integers $n$, $a$ and $b$ ($1 \le n \le 2\cdot10^{5}$, $0 \le a, b \le 2\cdot10^{5}$, $a + b &gt; 0$) — total number of seat places in the railway carriage, the number of student-programmers and the number of student-athletes.</p><p>The second line contains a string with length $n$, consisting of characters "<span class="tex-font-style-tt">.</span>" and "<span class="tex-font-style-tt">*</span>". The dot means that the corresponding place is empty. The asterisk means that the corresponding place is occupied by the jury member.</p>

## Output

<p>Print the largest number of students, which you can put in the railway carriage so that no student-programmer is sitting next to a student-programmer and no student-athlete is sitting next to a student-athlete.</p>





```input1
5 1 1
*...*

```




```input2
6 2 3
*...*.

```




```input3
11 3 10
.*....**.*.

```




```input4
3 2 3
***

```




```output1
2

```




```output2
4

```




```output3
7

```




```output4
0

```



## Note

<p>In the first example you can put all student, for example, in the following way: <span class="tex-font-style-tt">*.AB*</span></p><p>In the second example you can put four students, for example, in the following way: <span class="tex-font-style-tt">*BAB*B</span></p><p>In the third example you can put seven students, for example, in the following way: <span class="tex-font-style-tt">B*ABAB**A*B</span></p><p>The letter <span class="tex-font-style-tt">A</span> means a student-programmer, and the letter <span class="tex-font-style-tt">B</span> — student-athlete.</p>
