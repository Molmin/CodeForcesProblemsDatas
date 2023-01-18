## Description

<div><p>In <span class="tex-span">2<i>N</i> - 1</span> boxes there are apples and oranges. Your task is to choose <span class="tex-span"><i>N</i></span> boxes so, that they will contain not less than half of all the apples and not less than half of all the oranges.</p></div><div class="input-specification"><p>The first input line contains one number <span class="tex-span"><i>T</i></span> — amount of tests. The description of each test starts with a natural number <span class="tex-span"><i>N</i></span> — amount of boxes. Each of the following <span class="tex-span">2<i>N</i> - 1</span> lines contains numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>o</i><sub class="lower-index"><i>i</i></sub></span> — amount of apples and oranges in the <span class="tex-span"><i>i</i></span>-th box (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>o</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The sum of <span class="tex-span"><i>N</i></span> in all the tests in the input doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. All the input numbers are integer.</p></div><div class="output-specification"><p>For each test output two lines. In the first line output <span class="tex-font-style-tt">YES</span>, if it's possible to choose <span class="tex-span"><i>N</i></span> boxes, or <span class="tex-font-style-tt">NO</span> otherwise. If the answer is positive output in the second line <span class="tex-span"><i>N</i></span> numbers — indexes of the chosen boxes. Boxes are numbered from 1 in the input order. Otherwise leave the second line empty. Separate the numbers with one space.</p></div>

## Input

<p>The first input line contains one number <span class="tex-span"><i>T</i></span> — amount of tests. The description of each test starts with a natural number <span class="tex-span"><i>N</i></span> — amount of boxes. Each of the following <span class="tex-span">2<i>N</i> - 1</span> lines contains numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>o</i><sub class="lower-index"><i>i</i></sub></span> — amount of apples and oranges in the <span class="tex-span"><i>i</i></span>-th box (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>o</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). The sum of <span class="tex-span"><i>N</i></span> in all the tests in the input doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. All the input numbers are integer.</p>

## Output

<p>For each test output two lines. In the first line output <span class="tex-font-style-tt">YES</span>, if it's possible to choose <span class="tex-span"><i>N</i></span> boxes, or <span class="tex-font-style-tt">NO</span> otherwise. If the answer is positive output in the second line <span class="tex-span"><i>N</i></span> numbers — indexes of the chosen boxes. Boxes are numbered from 1 in the input order. Otherwise leave the second line empty. Separate the numbers with one space.</p>





```input1
2
2
10 15
5 7
20 18
1
0 0

```




```output1
YES
1 3
YES
1

```


