## Description

<div><p>Translator's note: in Russia's most widespread grading system, there are four grades: 5, 4, 3, 2, the higher the better, roughly corresponding to A, B, C and F respectively in American grading system.</p><p>The term is coming to an end and students start thinking about their grades. Today, a professor told his students that the grades for his course would be given out automatically &nbsp;— he would calculate the simple average (arithmetic mean) of all grades given out for lab works this term and round to the nearest integer. The rounding would be done in favour of the student&nbsp;— $4.5$ would be rounded up to $5$ (as in example 3), but $4.4$ would be rounded down to $4$.</p><p>This does not bode well for Vasya who didn't think those lab works would influence anything, so he may receive a grade worse than $5$ (maybe even the dreaded $2$). However, the professor allowed him to redo some of his works of Vasya's choosing to increase his average grade. Vasya wants to redo as as few lab works as possible in order to get $5$ for the course. Of course, Vasya will get $5$ for the lab works he chooses to redo.</p><p>Help Vasya&nbsp;— calculate the minimum amount of lab works Vasya has to redo.</p></div><div class="input-specification"><p>The first line contains a single integer $n$&nbsp;— the number of Vasya's grades ($1 \leq n \leq 100$).</p><p>The second line contains $n$ integers from $2$ to $5$&nbsp;— Vasya's grades for his lab works.</p></div><div class="output-specification"><p>Output a single integer&nbsp;— the minimum amount of lab works that Vasya has to redo. It can be shown that Vasya can always redo enough lab works to get a $5$.</p></div>

## Input

<p>The first line contains a single integer $n$&nbsp;— the number of Vasya's grades ($1 \leq n \leq 100$).</p><p>The second line contains $n$ integers from $2$ to $5$&nbsp;— Vasya's grades for his lab works.</p>

## Output

<p>Output a single integer&nbsp;— the minimum amount of lab works that Vasya has to redo. It can be shown that Vasya can always redo enough lab works to get a $5$.</p>





```input1
3
4 4 4

```




```input2
4
5 4 5 5

```




```input3
4
5 3 3 5

```




```output1
2

```




```output2
0

```




```output3
1

```



## Note

<p>In the first sample, it is enough to redo two lab works to make two $4$s into $5$s.</p><p>In the second sample, Vasya's average is already $4.75$ so he doesn't have to redo anything to get a $5$.</p><p>In the second sample Vasya has to redo one lab work to get rid of one of the $3$s, that will make the average exactly $4.5$ so the final grade would be $5$.</p>
