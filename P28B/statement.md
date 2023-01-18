## Description

<div><p>One day <span class="tex-span"><i>n</i></span> cells of some array decided to play the following game. Initially each cell contains a number which is equal to it's ordinal number (starting from <span class="tex-span">1</span>). Also each cell determined it's favourite number. On it's move <span class="tex-span"><i>i</i></span>-th cell can exchange it's value with the value of some other <span class="tex-span"><i>j</i></span>-th cell, if <span class="tex-span">|<i>i</i> - <i>j</i>| = <i>d</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is a favourite number of <span class="tex-span"><i>i</i></span>-th cell. Cells make moves in any order, the number of moves is unlimited.</p><p>The favourite number of each cell will be given to you. You will also be given a permutation of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. You are to determine whether the game could move to this state.</p></div><div class="input-specification"><p>The first line contains positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of cells in the array. The second line contains <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — permutation. The last line contains <span class="tex-span"><i>n</i></span> integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — favourite numbers of the cells.</p></div><div class="output-specification"><p>If the given state is reachable in the described game, output <span class="tex-font-style-tt">YES</span>, otherwise <span class="tex-font-style-tt">NO</span>.</p></div>

## Input

<p>The first line contains positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of cells in the array. The second line contains <span class="tex-span"><i>n</i></span> distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — permutation. The last line contains <span class="tex-span"><i>n</i></span> integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — favourite numbers of the cells.</p>

## Output

<p>If the given state is reachable in the described game, output <span class="tex-font-style-tt">YES</span>, otherwise <span class="tex-font-style-tt">NO</span>.</p>





```input1
5
5 4 3 2 1
1 1 1 1 1

```




```input2
7
4 3 5 1 2 7 6
4 6 6 1 6 6 1

```




```input3
7
4 2 5 1 3 7 6
4 6 6 1 6 6 1

```




```output1
YES

```




```output2
NO

```




```output3
YES

```


