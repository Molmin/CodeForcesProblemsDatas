## Description

<div><p>Peter wrote on the board a strictly increasing sequence of positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. Then Vasil replaced some digits in the numbers of this sequence by question marks. Thus, each question mark corresponds to exactly one lost digit.</p><p>Restore the the original sequence knowing digits remaining on the board.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the sequence. Next <span class="tex-span"><i>n</i></span> lines contain one element of the sequence each. Each element consists only of digits and question marks. No element starts from digit <span class="tex-font-style-tt">0</span>. Each element has length from 1 to 8 characters, inclusive.</p></div><div class="output-specification"><p>If the answer exists, print in the first line "<span class="tex-font-style-tt">YES</span>" (without the quotes). Next <span class="tex-span"><i>n</i></span> lines must contain the sequence of positive integers — a possible variant of Peter's sequence. The found sequence must be strictly increasing, it must be transformed from the given one by replacing each question mark by a single digit. All numbers on the resulting sequence must be written without leading zeroes. If there are multiple solutions, print any of them.</p><p>If there is no answer, print a single line "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the sequence. Next <span class="tex-span"><i>n</i></span> lines contain one element of the sequence each. Each element consists only of digits and question marks. No element starts from digit <span class="tex-font-style-tt">0</span>. Each element has length from 1 to 8 characters, inclusive.</p>

## Output

<p>If the answer exists, print in the first line "<span class="tex-font-style-tt">YES</span>" (without the quotes). Next <span class="tex-span"><i>n</i></span> lines must contain the sequence of positive integers — a possible variant of Peter's sequence. The found sequence must be strictly increasing, it must be transformed from the given one by replacing each question mark by a single digit. All numbers on the resulting sequence must be written without leading zeroes. If there are multiple solutions, print any of them.</p><p>If there is no answer, print a single line "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
3
?
18
1?

```




```input2
2
??
?

```




```input3
5
12224
12??5
12226
?0000
?00000

```




```output1
YES
1
18
19

```




```output2
NO

```




```output3
YES
12224
12225
12226
20000
100000

```


