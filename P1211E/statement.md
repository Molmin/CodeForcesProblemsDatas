## Description

<div><p>Polycarp recently became an employee of the company "Double Permutation Inc." Now he is a fan of permutations and is looking for them everywhere!</p><p>A permutation in this problem is a sequence of integers $p_1, p_2, \dots, p_k$ such that every integer from $1$ to $k$ occurs exactly once in it. For example, the following sequences are permutations of $[3, 1, 4, 2]$, $[1]$ and $[6, 1, 2, 3, 5, 4]$. The following sequences are not permutations: $[0, 1]$, $[1, 2, 2]$, $[1, 2, 4]$ and $[2, 3]$.</p><p>In the lobby of the company's headquarter statistics on visits to the company's website for the last $n$ days are published — the sequence $a_1, a_2, \dots, a_n$. Polycarp wants to color all the elements of this sequence in one of three colors (red, green or blue) so that:</p><ul> <li> all red numbers, being written out of $a_1, a_2, \dots, a_n$ from left to right (that is, without changing their relative order), must form some permutation (let's call it $P$); </li><li> all green numbers, being written out of $a_1, a_2, \dots, a_n$ from left to right (that is, without changing their relative order), must form the same permutation $P$; </li><li> among blue numbers there should not be elements that are equal to some element of the permutation $P$. </li></ul><p>Help Polycarp to color all $n$ numbers so that the total number of red and green elements is maximum.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 2\cdot10^5$) — the length of the sequence $a$. The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2\cdot10^5$).</p></div><div class="output-specification"><p>Print a string $s$ of length $n$ such that:</p><ul> <li> $s_i$='<span class="tex-font-style-tt">R</span>', if the element $a_i$ must be colored in red; </li><li> $s_i$='<span class="tex-font-style-tt">G</span>', if the element $a_i$ must be colored in green; </li><li> $s_i$='<span class="tex-font-style-tt">B</span>', if the element $a_i$ must be colored in blue. </li></ul><p>The string $s$ should maximize the total number of red and green elements when fulfilling the requirements from the main part of the problem statement. If there are several optimal answers, print any of them.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 2\cdot10^5$) — the length of the sequence $a$. The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 2\cdot10^5$).</p>

## Output

<p>Print a string $s$ of length $n$ such that:</p><ul> <li> $s_i$='<span class="tex-font-style-tt">R</span>', if the element $a_i$ must be colored in red; </li><li> $s_i$='<span class="tex-font-style-tt">G</span>', if the element $a_i$ must be colored in green; </li><li> $s_i$='<span class="tex-font-style-tt">B</span>', if the element $a_i$ must be colored in blue. </li></ul><p>The string $s$ should maximize the total number of red and green elements when fulfilling the requirements from the main part of the problem statement. If there are several optimal answers, print any of them.</p>





```input1
5
1 2 3 2 1
```




```input2
3
1 1 1
```




```input3
10
3 3 2 2 5 4 1 5 4 1
```




```input4
10
3 9 3 1 2 1 2 4 4 4
```




```output1
RBBBG
```




```output2
BBB
```




```output3
RGRGRRRGGG
```




```output4
RBGRRGGBBB
```


