## Description

<div><p>«Bersoft» company is working on a new version of its most popular text editor — Bord 2010. Bord, like many other text editors, should be able to print out multipage documents. A user keys a sequence of the document page numbers that he wants to print out (separates them with a comma, without spaces).</p><p>Your task is to write a part of the program, responsible for «standardization» of this sequence. Your program gets the sequence, keyed by the user, as input. The program should output this sequence in format <span class="tex-span"><i>l</i><sub class="lower-index">1</sub></span>-<span class="tex-span"><i>r</i><sub class="lower-index">1</sub></span>,<span class="tex-span"><i>l</i><sub class="lower-index">2</sub></span>-<span class="tex-span"><i>r</i><sub class="lower-index">2</sub></span>,...,<span class="tex-span"><i>l</i><sub class="lower-index"><i>k</i></sub></span>-<span class="tex-span"><i>r</i><sub class="lower-index"><i>k</i></sub></span>, where <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub> + 1 &lt; <i>l</i><sub class="lower-index"><i>i</i> + 1</sub></span> for all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i> - 1</span>, and <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub></span>. The new sequence should contain all the page numbers, keyed by the user, and nothing else. If some page number appears in the input sequence several times, its appearances, starting from the second one, should be ignored. If for some element <span class="tex-span"><i>i</i></span> from the new sequence <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> = <i>r</i><sub class="lower-index"><i>i</i></sub></span>, this element should be output as <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, and not as «<span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub> - <i>l</i><sub class="lower-index"><i>i</i></sub></span>».</p><p>For example, sequence <span class="tex-font-style-tt">1,2,3,1,1,2,6,6,2</span> should be output as <span class="tex-font-style-tt">1-3,6</span>.</p></div><div class="input-specification"><p>The only line contains the sequence, keyed by the user. The sequence contains at least one and at most 100 positive integer numbers. It's guaranteed, that this sequence consists of positive integer numbers, not exceeding 1000, separated with a comma, doesn't contain any other characters, apart from digits and commas, can't end with a comma, and the numbers don't contain leading zeroes. Also it doesn't start with a comma or contain more than one comma in a row.</p></div><div class="output-specification"><p>Output the sequence in the required format.</p></div>

## Input

<p>The only line contains the sequence, keyed by the user. The sequence contains at least one and at most 100 positive integer numbers. It's guaranteed, that this sequence consists of positive integer numbers, not exceeding 1000, separated with a comma, doesn't contain any other characters, apart from digits and commas, can't end with a comma, and the numbers don't contain leading zeroes. Also it doesn't start with a comma or contain more than one comma in a row.</p>

## Output

<p>Output the sequence in the required format.</p>





```input1
1,2,3,1,1,2,6,6,2

```




```input2
3,2,1

```




```input3
30,20,10

```




```output1
1-3,6

```




```output2
1-3

```




```output3
10,20,30

```


