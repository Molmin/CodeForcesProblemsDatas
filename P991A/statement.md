## Description

<div><p>Each student eagerly awaits the day he would pass the exams successfully. Thus, Vasya was ready to celebrate, but, alas, he didn't pass it. However, many of Vasya's fellow students from the same group were more successful and celebrated after the exam.</p><p>Some of them celebrated in the BugDonalds restaurant, some of them&nbsp;— in the BeaverKing restaurant, the most successful ones were fast enough to celebrate in both of restaurants. Students which didn't pass the exam didn't celebrate in any of those restaurants and elected to stay home to prepare for their reexamination. However, this quickly bored Vasya and he started checking celebration photos on the Kilogramm. He found out that, in total, BugDonalds was visited by $A$ students, BeaverKing&nbsp;— by $B$ students and $C$ students visited both restaurants. Vasya also knows that there are $N$ students in his group.</p><p>Based on this info, Vasya wants to determine either if his data contradicts itself or, if it doesn't, how many students in his group didn't pass the exam. Can you help him so he won't waste his valuable preparation time?</p></div><div class="input-specification"><p>The first line contains four integers&nbsp;— $A$, $B$, $C$ and $N$ ($0 \leq A, B, C, N \leq 100$).</p></div><div class="output-specification"><p>If a distribution of $N$ students exists in which $A$ students visited BugDonalds, $B$ — BeaverKing, $C$ — both of the restaurants and at least one student is left home (it is known that Vasya didn't pass the exam and stayed at home), output one integer&nbsp;— amount of students (including Vasya) who did not pass the exam. </p><p>If such a distribution does not exist and Vasya made a mistake while determining the numbers $A$, $B$, $C$ or $N$ (as in samples 2 and 3), output $-1$.</p></div>

## Input

<p>The first line contains four integers&nbsp;— $A$, $B$, $C$ and $N$ ($0 \leq A, B, C, N \leq 100$).</p>

## Output

<p>If a distribution of $N$ students exists in which $A$ students visited BugDonalds, $B$ — BeaverKing, $C$ — both of the restaurants and at least one student is left home (it is known that Vasya didn't pass the exam and stayed at home), output one integer&nbsp;— amount of students (including Vasya) who did not pass the exam. </p><p>If such a distribution does not exist and Vasya made a mistake while determining the numbers $A$, $B$, $C$ or $N$ (as in samples 2 and 3), output $-1$.</p>





```input1
10 10 5 20

```




```input2
2 2 0 4

```




```input3
2 2 2 1

```




```output1
5
```




```output2
-1
```




```output3
-1
```



## Note

<p>The first sample describes following situation: $5$ only visited BugDonalds, $5$ students only visited BeaverKing, $5$ visited both of them and $5$ students (including Vasya) didn't pass the exam.</p><p>In the second sample $2$ students only visited BugDonalds and $2$ only visited BeaverKing, but that means all $4$ students in group passed the exam which contradicts the fact that Vasya didn't pass meaning that this situation is impossible.</p><p>The third sample describes a situation where $2$ students visited BugDonalds but the group has only $1$ which makes it clearly impossible.</p>
