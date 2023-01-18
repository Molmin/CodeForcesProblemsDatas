## Description

<div><p>Professor Vasechkin is studying evolution of worms. Recently he put forward hypotheses that all worms evolve by division. There are <span class="tex-span"><i>n</i></span> forms of worms. Worms of these forms have lengths <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span>. To prove his theory, professor needs to find 3 different forms that the length of the first form is equal to sum of lengths of the other two forms. Help him to do this.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — amount of worm's forms. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — lengths of worms of each form.</p></div><div class="output-specification"><p>Output 3 distinct integers <span class="tex-span"><i>i</i></span> <span class="tex-span"><i>j</i></span> <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i>, <i>k</i> ≤ <i>n</i></span>) — such indexes of worm's forms that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>j</i></sub> + <i>a</i><sub class="lower-index"><i>k</i></sub></span>. If there is no such triple, output <span class="tex-font-style-tt">-1</span>. If there are several solutions, output any of them. It possible that <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>a</i><sub class="lower-index"><i>k</i></sub></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100</span>) — amount of worm's forms. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>) — lengths of worms of each form.</p>

## Output

<p>Output 3 distinct integers <span class="tex-span"><i>i</i></span> <span class="tex-span"><i>j</i></span> <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>i</i>, <i>j</i>, <i>k</i> ≤ <i>n</i></span>) — such indexes of worm's forms that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>j</i></sub> + <i>a</i><sub class="lower-index"><i>k</i></sub></span>. If there is no such triple, output <span class="tex-font-style-tt">-1</span>. If there are several solutions, output any of them. It possible that <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>a</i><sub class="lower-index"><i>k</i></sub></span>.</p>





```input1
5
1 2 3 5 7

```




```input2
5
1 8 1 5 1

```




```output1
3 2 1

```




```output2
-1

```


