## Description

<div><p>Sereja and his friends went to a picnic. The guys had <span class="tex-span"><i>n</i></span> soda bottles just for it. Sereja forgot the bottle opener as usual, so the guys had to come up with another way to open bottles.</p><p>Sereja knows that the <span class="tex-span"><i>i</i></span>-th bottle is from brand <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, besides, you can use it to open <span class="tex-font-style-bf">other</span> bottles of brand <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. You can use one bottle to open multiple other bottles. Sereja can open bottle with opened bottle or closed bottle.</p><p>Knowing this, Sereja wants to find out the number of bottles they've got that they won't be able to open in any way. Help him and find this number.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of bottles. The next <span class="tex-span"><i>n</i></span> lines contain the bottles' description. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the description of the <span class="tex-span"><i>i</i></span>-th bottle.</p></div><div class="output-specification"><p>In a single line print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of bottles. The next <span class="tex-span"><i>n</i></span> lines contain the bottles' description. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 1000)</span> — the description of the <span class="tex-span"><i>i</i></span>-th bottle.</p>

## Output

<p>In a single line print a single integer — the answer to the problem.</p>





```input1
4
1 1
2 2
3 3
4 4

```




```input2
4
1 2
2 3
3 4
4 1

```




```output1
4

```




```output2
0

```


