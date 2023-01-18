## Description

<div><p>Petya studies positional notations. He has already learned to add and subtract numbers in the systems of notations with different radices and has moved on to a more complicated action — multiplication. To multiply large numbers one has to learn the multiplication table. Unfortunately, in the second grade students learn only the multiplication table of decimals (and some students even learn it in the first grade). Help Petya make a multiplication table for numbers in the system of notations with the radix <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ 10</span>) — the radix of the system.</p></div><div class="output-specification"><p>Output the multiplication table for the system of notations with the radix <span class="tex-span"><i>k</i></span>. The table must contain <span class="tex-span"><i>k</i> - 1</span> rows and <span class="tex-span"><i>k</i> - 1</span> columns. The element on the crossing of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column is equal to the product of <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> in the system of notations with the radix <span class="tex-span"><i>k</i></span>. Each line may have any number of spaces between the numbers (the extra spaces in the samples are put for clarity).</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ 10</span>) — the radix of the system.</p>

## Output

<p>Output the multiplication table for the system of notations with the radix <span class="tex-span"><i>k</i></span>. The table must contain <span class="tex-span"><i>k</i> - 1</span> rows and <span class="tex-span"><i>k</i> - 1</span> columns. The element on the crossing of the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column is equal to the product of <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> in the system of notations with the radix <span class="tex-span"><i>k</i></span>. Each line may have any number of spaces between the numbers (the extra spaces in the samples are put for clarity).</p>





```input1
10

```




```input2
3

```




```output1
1  2  3  4  5  6  7  8  9
2  4  6  8 10 12 14 16 18
3  6  9 12 15 18 21 24 27
4  8 12 16 20 24 28 32 36
5 10 15 20 25 30 35 40 45
6 12 18 24 30 36 42 48 54
7 14 21 28 35 42 49 56 63
8 16 24 32 40 48 56 64 72
9 18 27 36 45 54 63 72 81

```




```output2
1  2
2 11
```


