## Description

<div><p>You are given a pair of integers $(a, b)$ and an integer $x$.</p><p>You can change the pair in two different ways: </p><ul> <li> set (assign) $a := |a - b|$; </li><li> set (assign) $b := |a - b|$, </li></ul> where $|a - b|$ is the absolute difference between $a$ and $b$.<p>The pair $(a, b)$ is called $x$-magic if $x$ is obtainable either as $a$ or as $b$ using only the given operations (i.e. the pair $(a, b)$ is $x$-magic if $a = x$ or $b = x$ after some number of operations applied). You can apply the operations any number of times (even zero).</p><p>Your task is to find out if the pair $(a, b)$ is $x$-magic or not.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. The next $t$ lines describe test cases.</p><p>The only line of the test case contains three integers $a$, $b$ and $x$ ($1 \le a, b, x \le 10^{18}$).</p></div><div class="output-specification"><p>For the $i$-th test case, print <span class="tex-font-style-tt">YES</span> if the corresponding pair $(a, b)$ is $x$-magic and <span class="tex-font-style-tt">NO</span> otherwise.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) — the number of test cases. The next $t$ lines describe test cases.</p><p>The only line of the test case contains three integers $a$, $b$ and $x$ ($1 \le a, b, x \le 10^{18}$).</p>

## Output

<p>For the $i$-th test case, print <span class="tex-font-style-tt">YES</span> if the corresponding pair $(a, b)$ is $x$-magic and <span class="tex-font-style-tt">NO</span> otherwise.</p>





```input1
8
6 9 3
15 38 7
18 8 8
30 30 30
40 50 90
24 28 20
365 216 52
537037812705867558 338887693834423551 3199921013340
```




```output1
YES
YES
YES
YES
NO
YES
YES
YES
```


