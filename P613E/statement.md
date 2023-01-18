## Description

<div><p>Oleg Petrov loves crossword puzzles and every Thursday he buys his favorite magazine with crosswords and other word puzzles. In the last magazine Oleg found a curious puzzle, and the magazine promised a valuable prize for it's solution. We give a formal description of the problem below.</p><p>The puzzle field consists of two rows, each row contains <span class="tex-span"><i>n</i></span> cells. Each cell contains exactly one small English letter. You also are given a word <span class="tex-span"><i>w</i></span>, which consists of <span class="tex-span"><i>k</i></span> small English letters. A <span class="tex-font-style-it">solution</span> of the puzzle is a sequence of field cells <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span>, such that:</p><ul><li> For all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span> the letter written in the cell <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> matches the letter <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>;</li><li> All the cells in the sequence are pairwise distinct;</li><li> For all <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i> - 1</span> cells <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i> + 1</sub></span> have a common side.</li></ul><p>Oleg Petrov quickly found a solution for the puzzle. Now he wonders, how many distinct solutions are there for this puzzle. Oleg Petrov doesn't like too large numbers, so calculate the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Two solutions <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i>'<sub class="lower-index"><i>i</i></sub></span> are considered distinct if the sequences of cells do not match in at least one position, that is there is such <span class="tex-span"><i>j</i></span> in range from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>, such that <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub> ≠ <i>c</i>'<sub class="lower-index"><i>j</i></sub></span>.</p></div><div class="input-specification"><p>The first two lines contain the state of the field for the puzzle. Each of these non-empty lines contains exactly <span class="tex-span"><i>n</i></span> small English letters.</p><p>The next line is left empty.</p><p>The next line is non-empty and contains word <span class="tex-span"><i>w</i></span>, consisting of small English letters.</p><p>The length of each line doesn't exceed <span class="tex-span">2 000</span>.</p></div><div class="output-specification"><p>Print a single integer — the number of distinct solutions for the puzzle modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first two lines contain the state of the field for the puzzle. Each of these non-empty lines contains exactly <span class="tex-span"><i>n</i></span> small English letters.</p><p>The next line is left empty.</p><p>The next line is non-empty and contains word <span class="tex-span"><i>w</i></span>, consisting of small English letters.</p><p>The length of each line doesn't exceed <span class="tex-span">2 000</span>.</p>

## Output

<p>Print a single integer — the number of distinct solutions for the puzzle modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
code
edoc

code

```




```input2
aaa
aaa

aa

```




```output1
4

```




```output2
14

```


