## Description

<div><div class="epigraph"><div class="epigraph-text">Your program fails again. This time it gets "<span class="tex-font-style-tt">Wrong answer on test 233</span>"</div></div>.<p><span class="tex-font-style-it">This is the easier version of the problem. In this version $1 \le n \le 2000$. You can hack this problem only if you solve and lock both problems.</span></p><p>The problem is about a test containing $n$ one-choice-questions. Each of the questions contains $k$ options, and only one of them is correct. The answer to the $i$-th question is $h_{i}$, and if your answer of the question $i$ is $h_{i}$, you earn $1$ point, otherwise, you earn $0$ points for this question. The values $h_1, h_2, \dots, h_n$ are known to you in this problem.</p><p>However, you have a mistake in your program. It moves the answer clockwise! Consider all the $n$ answers are written in a circle. Due to the mistake in your program, they are shifted by one cyclically.</p><p>Formally, the mistake moves the answer for the question $i$ to the question $i \bmod n + 1$. So it moves the answer for the question $1$ to question $2$, the answer for the question $2$ to the question $3$, ..., the answer for the question $n$ to the question $1$.</p><p>We call all the $n$ answers together an <span class="tex-font-style-it">answer suit</span>. There are $k^n$ possible answer suits in total.</p><p>You're wondering, how many answer suits satisfy the following condition: <span class="tex-font-style-it">after moving clockwise by $1$, the total number of points of the new answer suit is strictly larger than the number of points of the old one</span>. You need to find the answer modulo $998\,244\,353$.</p><p>For example, if $n = 5$, and your answer suit is $a=[1,2,3,4,5]$, it will submitted as $a'=[5,1,2,3,4]$ because of a mistake. If the correct answer suit is $h=[5,2,2,3,4]$, the answer suit $a$ earns $1$ point and the answer suite $a'$ earns $4$ points. Since $4 &gt; 1$, the answer suit $a=[1,2,3,4,5]$ should be counted.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $k$ ($1 \le n \le 2000$, $1 \le k \le 10^9$)&nbsp;— the number of questions and the number of possible answers to each question.</p><p>The following line contains $n$ integers $h_1, h_2, \dots, h_n$, ($1 \le h_{i} \le k)$&nbsp;— answers to the questions.</p></div><div class="output-specification"><p>Output one integer: the number of answers suits satisfying the given condition, modulo $998\,244\,353$.</p></div>

## Input

<p>The first line contains two integers $n$, $k$ ($1 \le n \le 2000$, $1 \le k \le 10^9$)&nbsp;— the number of questions and the number of possible answers to each question.</p><p>The following line contains $n$ integers $h_1, h_2, \dots, h_n$, ($1 \le h_{i} \le k)$&nbsp;— answers to the questions.</p>

## Output

<p>Output one integer: the number of answers suits satisfying the given condition, modulo $998\,244\,353$.</p>





```input1
3 3
1 3 1
```




```input2
5 5
1 1 4 2 2
```




```output1
9
```




```output2
1000
```



## Note

<p>For the first example, valid answer suits are $[2,1,1], [2,1,2], [2,1,3], [3,1,1], [3,1,2], [3,1,3], [3,2,1], [3,2,2], [3,2,3]$.</p>
