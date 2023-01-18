## Description

<div><p>Vasya tries to break in a safe. He knows that a code consists of <span class="tex-span"><i>n</i></span> numbers, and every number is a 0 or a 1. Vasya has made <span class="tex-span"><i>m</i></span> attempts to enter the code. After each attempt the system told him in how many position stand the right numbers. It is not said in which positions the wrong numbers stand. Vasya has been so unlucky that he hasn’t entered the code where would be more than 5 correct numbers. Now Vasya is completely bewildered: he thinks there’s a mistake in the system and it is self-contradictory. Help Vasya — calculate how many possible code variants are left that do not contradict the previous system responses.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">6 ≤ <i>n</i> ≤ 35, 1 ≤ <i>m</i> ≤ 10</span>) which represent the number of numbers in the code and the number of attempts made by Vasya. Then follow <span class="tex-span"><i>m</i></span> lines, each containing space-separated <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> which correspondingly indicate Vasya’s attempt (a line containing <span class="tex-span"><i>n</i></span> numbers which are 0 or 1) and the system’s response (an integer from 0 to 5 inclusively).</p></div><div class="output-specification"><p>Print the single number which indicates how many possible code variants that do not contradict the <span class="tex-span"><i>m</i></span> system responses are left.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">6 ≤ <i>n</i> ≤ 35, 1 ≤ <i>m</i> ≤ 10</span>) which represent the number of numbers in the code and the number of attempts made by Vasya. Then follow <span class="tex-span"><i>m</i></span> lines, each containing space-separated <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> which correspondingly indicate Vasya’s attempt (a line containing <span class="tex-span"><i>n</i></span> numbers which are 0 or 1) and the system’s response (an integer from 0 to 5 inclusively).</p>

## Output

<p>Print the single number which indicates how many possible code variants that do not contradict the <span class="tex-span"><i>m</i></span> system responses are left.</p>





```input1
6 2
000000 2
010100 4

```




```input2
6 3
000000 2
010100 4
111100 0

```




```input3
6 3
000000 2
010100 4
111100 2

```




```output1
6

```




```output2
0

```




```output3
1

```


