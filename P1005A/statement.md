## Description

<div><p>Little girl Tanya climbs the stairs inside a multi-storey building. Every time Tanya climbs a stairway, she starts counting steps from $1$ to the number of steps in this stairway. She speaks every number aloud. For example, if she climbs two stairways, the first of which contains $3$ steps, and the second contains $4$ steps, she will pronounce the numbers $1, 2, 3, 1, 2, 3, 4$.</p><p>You are given all the numbers pronounced by Tanya. How many stairways did she climb? Also, output the number of steps in each stairway.</p><p>The given sequence will be a valid sequence that Tanya could have pronounced when climbing one or more stairways.</p></div><div class="input-specification"><p>The first line contains $n$ ($1 \le n \le 1000$) — the total number of numbers pronounced by Tanya.</p><p>The second line contains integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 1000$) — all the numbers Tanya pronounced while climbing the stairs, in order from the first to the last pronounced number. Passing a stairway with $x$ steps, she will pronounce the numbers $1, 2, \dots, x$ in that order.</p><p>The given sequence will be a valid sequence that Tanya could have pronounced when climbing one or more stairways.</p></div><div class="output-specification"><p>In the first line, output $t$ — the number of stairways that Tanya climbed. In the second line, output $t$ numbers — the number of steps in each stairway she climbed. Write the numbers in the correct order of passage of the stairways.</p></div>

## Input

<p>The first line contains $n$ ($1 \le n \le 1000$) — the total number of numbers pronounced by Tanya.</p><p>The second line contains integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 1000$) — all the numbers Tanya pronounced while climbing the stairs, in order from the first to the last pronounced number. Passing a stairway with $x$ steps, she will pronounce the numbers $1, 2, \dots, x$ in that order.</p><p>The given sequence will be a valid sequence that Tanya could have pronounced when climbing one or more stairways.</p>

## Output

<p>In the first line, output $t$ — the number of stairways that Tanya climbed. In the second line, output $t$ numbers — the number of steps in each stairway she climbed. Write the numbers in the correct order of passage of the stairways.</p>





```input1
7
1 2 3 1 2 3 4

```




```input2
4
1 1 1 1

```




```input3
5
1 2 3 4 5

```




```input4
5
1 2 1 2 1

```




```output1
2
3 4
```




```output2
4
1 1 1 1
```




```output3
1
5
```




```output4
3
2 2 1
```


