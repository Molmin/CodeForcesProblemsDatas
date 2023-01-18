## Description

<div><p>Vasya adores sport programming. He can't write programs but he loves to watch the contests' progress. Vasya even has a favorite coder and Vasya pays special attention to him.</p><p>One day Vasya decided to collect the results of all contests where his favorite coder participated and track the progress of his coolness. For each contest where this coder participated, he wrote out a single non-negative number — the number of points his favorite coder earned in the contest. Vasya wrote out the points for the contest in the order, in which the contests run (naturally, no two contests ran simultaneously).</p><p>Vasya considers a coder's performance in a contest <span class="tex-font-style-it">amazing</span> in two situations: he can break either his best or his worst performance record. First, it is amazing if during the contest the coder earns strictly <span class="tex-font-style-bf">more</span> points that he earned on each past contest. Second, it is amazing if during the contest the coder earns strictly <span class="tex-font-style-bf">less</span> points that he earned on each past contest. A coder's first contest isn't considered amazing. Now he wants to count the number of amazing performances the coder had throughout his whole history of participating in contests. But the list of earned points turned out long and Vasya can't code... That's why he asks you to help him.</p></div><div class="input-specification"><p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of contests where the coder participated.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated non-negative integer numbers — they are the points which the coder has earned. The points are given in the chronological order. All points do not exceed <span class="tex-span">10000</span>.</p></div><div class="output-specification"><p>Print the single number — the number of amazing performances the coder has had during his whole history of participating in the contests.</p></div>

## Input

<p>The first line contains the single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of contests where the coder participated.</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated non-negative integer numbers — they are the points which the coder has earned. The points are given in the chronological order. All points do not exceed <span class="tex-span">10000</span>.</p>

## Output

<p>Print the single number — the number of amazing performances the coder has had during his whole history of participating in the contests.</p>





```input1
5
100 50 200 150 200

```




```input2
10
4664 6496 5814 7010 5762 5736 6944 4850 3698 7242

```




```output1
2

```




```output2
4

```



## Note

<p>In the first sample the performances number 2 and 3 are amazing.</p><p>In the second sample the performances number 2, 4, 9 and 10 are amazing.</p>
