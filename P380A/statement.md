## Description

<div><p>Sereja loves number sequences very much. That's why he decided to make himself a new one following a certain algorithm.</p><p>Sereja takes a blank piece of paper. Then he starts writing out the sequence in <span class="tex-span"><i>m</i></span> stages. Each time he either adds a new number to the end of the sequence or takes <span class="tex-span"><i>l</i></span> first elements of the current sequence and adds them <span class="tex-span"><i>c</i></span> times to the end. More formally, if we represent the current sequence as <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, then after we apply the described operation, the sequence transforms into <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub>[, <i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>l</i></sub>]</span> (the block in the square brackets must be repeated <span class="tex-span"><i>c</i></span> times). </p><p>A day has passed and Sereja has completed the sequence. He wonders what are the values of some of its elements. Help Sereja.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of stages to build a sequence. </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the description of the stages in the order they follow. The first number in the line is a type of stage (1 or 2). Type 1 means adding one number to the end of the sequence, in this case the line contains integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the number to add. Type 2 means copying a prefix of length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to the end <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> times, in this case the line further contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is the length of the prefix, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the number of copyings. It is guaranteed that the length of prefix <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is never larger than the current length of the sequence.</p><p>The next line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of elements Sereja is interested in. The next line contains the numbers of elements of the final sequence Sereja is interested in. The numbers are given in the strictly increasing order. It is guaranteed that all numbers are strictly larger than zero and do not exceed the length of the resulting sequence. Consider the elements of the final sequence numbered starting from <span class="tex-span">1</span> from the beginning to the end of the sequence.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div><div class="output-specification"><p>Print the elements that Sereja is interested in, in the order in which their numbers occur in the input. </p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of stages to build a sequence. </p><p>Next <span class="tex-span"><i>m</i></span> lines contain the description of the stages in the order they follow. The first number in the line is a type of stage (1 or 2). Type 1 means adding one number to the end of the sequence, in this case the line contains integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>)</span> — the number to add. Type 2 means copying a prefix of length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to the end <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> times, in this case the line further contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is the length of the prefix, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the number of copyings. It is guaranteed that the length of prefix <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> is never larger than the current length of the sequence.</p><p>The next line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of elements Sereja is interested in. The next line contains the numbers of elements of the final sequence Sereja is interested in. The numbers are given in the strictly increasing order. It is guaranteed that all numbers are strictly larger than zero and do not exceed the length of the resulting sequence. Consider the elements of the final sequence numbered starting from <span class="tex-span">1</span> from the beginning to the end of the sequence.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>

## Output

<p>Print the elements that Sereja is interested in, in the order in which their numbers occur in the input. </p>





```input1
6
1 1
1 2
2 2 1
1 3
2 5 2
1 4
16
1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16

```




```output1
1 2 1 2 3 1 2 1 2 3 1 2 1 2 3 4

```


