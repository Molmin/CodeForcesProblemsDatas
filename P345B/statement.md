## Description

<div><p>Triskaidekaphobia is a fear of number 13. Ordinary people who suffer from this phobia feel uncomfortable around numbers 13, 130, 513 etc, but you, being a programmer, take this fear one step further. For example, consider number 7. It's ok when written in decimal, but written in base 4 it becomes 13, the dreadful number!</p><p>The more you think about it, the worse it looks. Number 100 has as many as 13 notations which contain 13! And there are numbers which have 13 in infinite number of their notations! Luckily, you can do any math in binary, which is completely safe from the nasty number. But still, you want to be able to estimate the level of nastiness of any number. </p><p>Your task is: given an integer <span class="tex-span"><i>n</i></span>, find the number of different integer bases <span class="tex-span"><i>b</i></span> <span class="tex-span">(<i>b</i> ≥ 2)</span> for which <span class="tex-span"><i>n</i></span>, written in base <span class="tex-span"><i>b</i></span>, contains at least one 13. Assume that "digits" of the number in bases larger than 10 are written not as letters but as decimal numbers; thus, 30 in base 16 is not 1E but (1)(14) or simply 114. Please note, that 13 must be present as a substring of notation, not a subsequence (123 doesn't contain 13).</p></div><div class="input-specification"><p>The only line of the input contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p></div><div class="output-specification"><p>Output a single integer — the number of different integer bases <span class="tex-span"><i>b</i></span> <span class="tex-span">(<i>b</i> ≥ 2)</span> for which <span class="tex-span"><i>n</i></span>, written in base <span class="tex-span"><i>b</i></span>, contains at least one 13. If there are infinitely many such bases, output -1.</p></div>

## Input

<p>The only line of the input contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p>

## Output

<p>Output a single integer — the number of different integer bases <span class="tex-span"><i>b</i></span> <span class="tex-span">(<i>b</i> ≥ 2)</span> for which <span class="tex-span"><i>n</i></span>, written in base <span class="tex-span"><i>b</i></span>, contains at least one 13. If there are infinitely many such bases, output -1.</p>





```input1
7

```




```input2
100

```




```input3
13

```




```output1
1

```




```output2
13

```




```output3
-1

```


