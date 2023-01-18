## Description

<div><p>One not particularly beautiful evening Valera got very bored. To amuse himself a little bit, he found the following game.</p><p>He took a checkered white square piece of paper, consisting of <span class="tex-span"><i>n</i> × <i>n</i></span> cells. After that, he started to paint the white cells black one after the other. In total he painted <span class="tex-span"><i>m</i></span> different cells on the piece of paper. Since Valera was keen on everything square, he wondered, how many moves (i.e. times the boy paints a square black) he should make till a black square with side <span class="tex-span">3</span> can be found on the piece of paper. But Valera does not know the answer to this question, so he asks you to help him.</p><p>Your task is to find the minimum number of moves, till the checkered piece of paper has at least one black square with side of <span class="tex-span">3</span>. Otherwise determine that such move does not exist.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>min</i>(<i>n</i>·<i>n</i>, 10<sup class="upper-index">5</sup>))</span> — the size of the squared piece of paper and the number of moves, correspondingly. </p><p>Then, <span class="tex-span"><i>m</i></span> lines contain the description of the moves. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the number of row and column of the square that gets painted on the <span class="tex-span"><i>i</i></span>-th move. </p><p>All numbers on the lines are separated by single spaces. It is guaranteed that all moves are different. The moves are numbered starting from <span class="tex-span">1</span> in the order, in which they are given in the input. The columns of the squared piece of paper are numbered starting from <span class="tex-span">1</span>, from the left to the right. The rows of the squared piece of paper are numbered starting from <span class="tex-span">1</span>, from top to bottom.</p></div><div class="output-specification"><p>On a single line print the answer to the problem — the minimum number of the move after which the piece of paper has a black square with side <span class="tex-span">3</span>. If no such move exists, print -1.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ <i>min</i>(<i>n</i>·<i>n</i>, 10<sup class="upper-index">5</sup>))</span> — the size of the squared piece of paper and the number of moves, correspondingly. </p><p>Then, <span class="tex-span"><i>m</i></span> lines contain the description of the moves. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — the number of row and column of the square that gets painted on the <span class="tex-span"><i>i</i></span>-th move. </p><p>All numbers on the lines are separated by single spaces. It is guaranteed that all moves are different. The moves are numbered starting from <span class="tex-span">1</span> in the order, in which they are given in the input. The columns of the squared piece of paper are numbered starting from <span class="tex-span">1</span>, from the left to the right. The rows of the squared piece of paper are numbered starting from <span class="tex-span">1</span>, from top to bottom.</p>

## Output

<p>On a single line print the answer to the problem — the minimum number of the move after which the piece of paper has a black square with side <span class="tex-span">3</span>. If no such move exists, print -1.</p>





```input1
4 11
1 1
1 2
1 3
2 2
2 3
1 4
2 4
3 4
3 2
3 3
4 1

```




```input2
4 12
1 1
1 2
1 3
2 2
2 3
1 4
2 4
3 4
3 2
4 2
4 1
3 1

```




```output1
10

```




```output2
-1

```


