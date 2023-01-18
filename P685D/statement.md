## Description

<div><p>Snow Queen told Kay to form a word "eternity" using pieces of ice. Kay is eager to deal with the task, because he will then become free, and Snow Queen will give him all the world and a pair of skates.</p><p>Behind the palace of the Snow Queen there is an infinite field consisting of cells. There are <span class="tex-span"><i>n</i></span> pieces of ice spread over the field, each piece occupying exactly one cell and no two pieces occupying the same cell. To estimate the difficulty of the task Kay looks at some squares of size <span class="tex-span"><i>k</i> × <i>k</i></span> cells, with corners located at the corners of the cells and sides parallel to coordinate axis and counts the number of pieces of the ice inside them.</p><p>This method gives an estimation of the difficulty of some part of the field. However, Kay also wants to estimate the total difficulty, so he came up with the following criteria: for each <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>) he wants to count the number of squares of size <span class="tex-span"><i>k</i> × <i>k</i></span>, such that there are exactly <span class="tex-span"><i>x</i></span> pieces of the ice inside.</p><p>Please, help Kay estimate the difficulty of the task given by the Snow Queen.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 300</span>)&nbsp;— the number of pieces of the ice and the value <span class="tex-span"><i>k</i></span>, respectively. Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates of the cell containing <span class="tex-span"><i>i</i></span>-th piece of the ice. It's guaranteed, that no two pieces of the ice occupy the same cell.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers: the number of squares of size <span class="tex-span"><i>k</i> × <i>k</i></span> containing exactly <span class="tex-span">1, 2, ..., <i>n</i></span> pieces of the ice.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 300</span>)&nbsp;— the number of pieces of the ice and the value <span class="tex-span"><i>k</i></span>, respectively. Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— coordinates of the cell containing <span class="tex-span"><i>i</i></span>-th piece of the ice. It's guaranteed, that no two pieces of the ice occupy the same cell.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers: the number of squares of size <span class="tex-span"><i>k</i> × <i>k</i></span> containing exactly <span class="tex-span">1, 2, ..., <i>n</i></span> pieces of the ice.</p>





```input1
5 3
4 5
4 6
5 5
5 6
7 7

```




```output1
10 8 1 4 0 

```


