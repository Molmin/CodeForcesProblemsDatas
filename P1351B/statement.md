## Description

<div><p>Vasya claims that he had a paper square. He cut it into two rectangular parts using one vertical or horizontal cut. Then Vasya informed you the dimensions of these two rectangular parts. You need to check whether Vasya originally had a square. In other words, check if it is possible to make a square using two given rectangles.</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case is given in two lines.</p><p>The first line contains two integers $a_1$ and $b_1$ ($1 \le a_1, b_1 \le 100$) — the dimensions of the first one obtained after cutting rectangle. The sizes are given in random order (that is, it is not known which of the numbers is the width, and which of the numbers is the length).</p><p>The second line contains two integers $a_2$ and $b_2$ ($1 \le a_2, b_2 \le 100$) — the dimensions of the second obtained after cutting rectangle. The sizes are given in random order (that is, it is not known which of the numbers is the width, and which of the numbers is the length).</p></div><div class="output-specification"><p>Print $t$ answers, each of which is a string "<span class="tex-font-style-tt">YES</span>" (in the case of a positive answer) or "<span class="tex-font-style-tt">NO</span>" (in the case of a negative answer). The letters in words can be printed in any case (upper or lower).</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 10^4$) — the number of test cases in the input. Then $t$ test cases follow.</p><p>Each test case is given in two lines.</p><p>The first line contains two integers $a_1$ and $b_1$ ($1 \le a_1, b_1 \le 100$) — the dimensions of the first one obtained after cutting rectangle. The sizes are given in random order (that is, it is not known which of the numbers is the width, and which of the numbers is the length).</p><p>The second line contains two integers $a_2$ and $b_2$ ($1 \le a_2, b_2 \le 100$) — the dimensions of the second obtained after cutting rectangle. The sizes are given in random order (that is, it is not known which of the numbers is the width, and which of the numbers is the length).</p>

## Output

<p>Print $t$ answers, each of which is a string "<span class="tex-font-style-tt">YES</span>" (in the case of a positive answer) or "<span class="tex-font-style-tt">NO</span>" (in the case of a negative answer). The letters in words can be printed in any case (upper or lower).</p>





```input1
3
2 3
3 1
3 2
1 3
3 3
1 3
```




```output1
Yes
Yes
No
```


