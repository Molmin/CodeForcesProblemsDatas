## Description

<div><p>Madoka is going to enroll in "<span class="tex-font-style-tt">TSUNS PTU</span>". But she stumbled upon a difficult task during the entrance computer science exam:</p><ul> <li> A number is called <span class="tex-font-style-it">good</span> if it is a multiple of $d$. </li><li> A number is called <span class="tex-font-style-it">beatiful</span> if it is <span class="tex-font-style-bf">good</span> and it <span class="tex-font-style-bf">cannot</span> be represented as a product of two good numbers. </li></ul><p>Notice that a beautiful number must be good.</p><p>Given a good number $x$, determine whether it can be represented in at least two different ways as a product of several (possibly, one) <span class="tex-font-style-bf">beautiful</span> numbers. Two ways are different if the sets of numbers used are different.</p><p>Solve this problem for Madoka and help her to enroll in the best school in Russia!</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— number of test cases. Below comes their description.</p><p>Each test case consists of two integers $x$ and $d$, separated by a space ($2 \leq x, d \leq 10^9$). It is guaranteed that $x$ is a multiple of $d$.</p></div><div class="output-specification"><p>For each set of input data, output "<span class="tex-font-style-tt">NO</span>" if the number <span class="tex-font-style-bf">cannot be</span> represented in at least two ways. Otherwise, output "<span class="tex-font-style-tt">YES</span>".</p><p>You can output each letter in any case (for example, "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">Yes</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yEs</span>" will be recognized as a positive answer).</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \leq t \leq 100$)&nbsp;— number of test cases. Below comes their description.</p><p>Each test case consists of two integers $x$ and $d$, separated by a space ($2 \leq x, d \leq 10^9$). It is guaranteed that $x$ is a multiple of $d$.</p>

## Output

<p>For each set of input data, output "<span class="tex-font-style-tt">NO</span>" if the number <span class="tex-font-style-bf">cannot be</span> represented in at least two ways. Otherwise, output "<span class="tex-font-style-tt">YES</span>".</p><p>You can output each letter in any case (for example, "<span class="tex-font-style-tt">YES</span>", "<span class="tex-font-style-tt">Yes</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yEs</span>" will be recognized as a positive answer).</p>





```input1
8
6 2
12 2
36 2
8 2
1000 10
2376 6
128 4
16384 4
```




```output1
NO
NO
YES
NO
YES
YES
NO
YES
```



## Note

<p>In the first example, $6$ can be represented as $6$, $1 \cdot 6$, $2 \cdot 3$. But $3$ and $1$ are not a good numbers because they are not divisible by $2$, so there is only one way.</p><p>In the second example, $12$ can be represented as $6 \cdot 2$, $12$, $3 \cdot 4$, or $3 \cdot 2 \cdot 2$. The first option is suitable. The second is— no, because $12$ is not beautiful number ($12 = 6 \cdot 2$). The third and fourth are also not suitable, because $3$ is not good number.</p><p>In the third example, $36$ can be represented as $18 \cdot 2$ and $6 \cdot 6$. Therefore it can be decomposed in at least two ways.</p>
